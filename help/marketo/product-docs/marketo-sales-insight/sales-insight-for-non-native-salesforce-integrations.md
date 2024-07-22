---
unique-page-id: 45417125
description: Informazioni sulle vendite per integrazioni Salesforce non native - Documenti Marketo - Documentazione del prodotto
title: Informazioni sulle vendite per integrazioni Salesforce non native
exl-id: a771ecdf-c610-44e4-9e93-7fdcc9d79f4b
feature: Marketo Sales Insights
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '1230'
ht-degree: 0%

---

# Informazioni sulle vendite per integrazioni Salesforce non native {#sales-insight-for-non-native-salesforce-integrations}

Se il tuo account Adobe Marketo Engage è connesso a Salesforce tramite un’integrazione personalizzata o non nativa, utilizza questo articolo per configurare Sales Insight.

>[!PREREQUISITES]
>
>* La funzione &quot;MSI non nativo&quot; è stata abilitata per l’istanza Marketo prima di avviare la configurazione di MSI. In caso contrario, e la funzionalità è già stata acquistata, contatta il [supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Se non hai ancora acquistato questa funzione, contatta l’Adobe Account Team (il tuo Account Manager).
>* Un account Salesforce con [pacchetto MSI configurato](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.
>* Configurazione dell&#39;API REST di Marketo [completata](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}. Le API CRUD esposte costituiranno la base per l’esecuzione della sincronizzazione non nativa.
>* Leggi [questo post di blog](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"} per comprendere l&#39;oggetto e le relazioni.
>* Imposta gli oggetti Salesforce per visualizzare l’identificatore univoco globale senza distinzione tra maiuscole e minuscole di 18 caratteri anziché l’identificatore univoco globale con distinzione tra maiuscole e minuscole di 15 caratteri.

>[!NOTE]
>
>Impossibile utilizzare la configurazione REST API nel pannello di amministrazione di Marketo MSI per la sincronizzazione non nativa.

## Una corretta sincronizzazione non nativa per MSI richiede quanto segue {#successful-non-native-sync-for-msi-requires-the-following}

1. Sincronizza l&#39;utente Salesforce Sales con Marketo.

   L&#39;utente di vendita Salesforce è un utente esterno proprietario dei lead/contatti in Salesforce. È necessario eseguire l&#39;upsert di un venditore Marketo per l&#39;utente Salesforce Sales. Il campo *externalSalesPersonId* è obbligatorio per l&#39;upsert del venditore.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo Marketo Sales Person</strong></td> 
      <td><strong>Campo utente vendite Salesforce</strong></td> 
      <td><strong>Descrizione</strong></td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per l'utente di vendita Salesforce</td> 
      <td><p>Identifica il record Marketo Sales Person in un oggetto esterno Salesforce Sales User.</p><p>Viene richiesto che il venditore venga sincronizzato prima di sincronizzare gli altri oggetti in modo da creare le relazioni appropriate.</p></td> 
     </tr> 
    </tbody> 
   </table>

   * Documentazione API per il venditore: [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/sales-persons](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/sales-persons){target="_blank"}
   * Documentazione API per la sincronizzazione del venditore: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. Sincronizza gli account Salesforce con Marketo.

   Per l’account Salesforce è necessario eseguire l’upsert di un’azienda Marketo. I campi _externalCompanyId_ e _externalSalesPersonId_ sono obbligatori per l&#39;upsert della società.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo società Marketo</strong></td> 
      <td><strong>Campo account Salesforce</strong></td> 
      <td><strong>Descrizione</strong></td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole dell’account Salesforce</td> 
      <td>Identifica un record di Marketo Company in un oggetto account Salesforce esterno.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per l'utente di vendita Salesforce</td> 
      <td>Identifica un record Società Marketo in un oggetto utente vendite Salesforce esterno proprietario dell'account.<br><br>Utilizzato anche in Marketo per associare l'azienda al venditore proprietario del record dell'azienda. Prima di impostare questo campo, è necessario sincronizzare il rappresentante commerciale.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentazione API per le società: [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/companies](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/companies){target="_blank"}
   * Documentazione API per la sincronizzazione delle società: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Companies/operation/syncCompaniesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Companies/operation/syncCompaniesUsingPOST){target="_blank"}

1. Sincronizza lead/contatti Salesforce con Marketo.

   Dovrai inserire un lead Marketo per il lead/contatto Salesforce. I campi _externalPersonId_, _externalSalesPersonId_ e _externalCompanyId_ sono obbligatori per l&#39;upsert del lead.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo lead Marketo</strong></td> 
      <td><strong>Campo contatto/lead Salesforce</strong></td> 
      <td><strong>Descrizione</strong></td> 
     </tr> 
     <tr> 
      <td>externalPersonId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per lead/contatti Salesforce</td> 
      <td>Identifica il record Lead Marketo in un oggetto Salesforce Lead/Contact esterno.<br><br>Questo è un nuovo campo introdotto per MSI non nativo.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per l'utente di vendita Salesforce</td> 
      <td>Identifica l'oggetto utente Salesforce Sales esterno proprietario di questo lead/contatto.<br><br>Collega inoltre il lead con il rappresentante commerciale di Marketo. Viene richiesto di sincronizzare correttamente prima il rappresentante commerciale.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole dell’account Salesforce</td> 
      <td>Identifica l’oggetto account Salesforce esterno a cui appartiene il lead/contatto.<br><br>Collega inoltre il record del lead a un'azienda in Marketo. È obbligatorio che prima l’account Salesforce sia sincronizzato correttamente.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentazione API per lead: [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/leads](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/leads)
   * Documentazione API per la sincronizzazione dei lead: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST)

1. Sincronizza opportunità Salesforce con Marketo.

   Sarà necessario eseguire l’upsert di un’opportunità Marketo per l’opportunità Salesforce. I campi _externalOpportunityId_, _externalCompanyId_ e _externalSalesPersonId_ sono obbligatori per l&#39;aggiornamento dell&#39;opportunità.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo oggetto opportunità Marketo</strong></td> 
      <td><strong>Campo oggetto opportunità Salesforce</strong></td> 
      <td><strong>Descrizione</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per lead/contatti Salesforce</td> 
      <td>Identifica il record Opportunità Marketo in un oggetto Opportunità Salesforce esterno.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole dell’account Salesforce</td> 
      <td>Identifica l’oggetto account Salesforce esterno a cui appartiene questa opportunità. <br><br>Viene richiesto che l'account Salesforce venga prima sincronizzato correttamente.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per l'utente di vendita Salesforce</td> 
      <td>Identifica l'oggetto utente vendite Salesforce esterno a cui appartiene questa opportunità. </td> 
     </tr> 
    </tbody> 
   </table>

   * Documentazione API per l&#39;opportunità: [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * Documentazione API per la sincronizzazione delle opportunità: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Sincronizza i ruoli dei contatti Salesforce con Marketo.

   I ruoli di contatto Salesforce per un’opportunità Salesforce possono quindi essere sincronizzati tramite il ruolo Opportunità Marketo. Il record Ruolo opportunità richiede i campi _externalOpportunityId_, _role_ e _leadId_.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo ruolo opportunità Marketo</strong></td> 
      <td><strong>Campo per ruolo contatto Salesforce</strong></td> 
      <td><strong>Descrizione</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per l’opportunità Salesforce</td> 
      <td>Identifica il ruolo opportunità Marketo in un oggetto opportunità Salesforce esterno.<br><br>È necessario prima sincronizzare correttamente l'opportunità Salesforce.</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>N/D, sarebbe un ID lead Marketo</td> 
      <td>Questo sarebbe l’ID lead Marketo del contatto Salesforce sincronizzato.<br><br>Una volta sincronizzato il contatto in Marketo, puoi utilizzare l'identificatore univoco globale senza distinzione tra maiuscole e minuscole del contatto Salesforce come externalPersonId e eseguire una query per il lead di Marketo utilizzando l'API REST di Marketo.</td> 
     </tr> 
     <tr> 
      <td>ruolo</td> 
      <td>Campo Ruolo per il contatto Salesforce</td> 
      <td>Descrive il ruolo del contatto per questa opportunità.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentazione API per l&#39;opportunità: [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * Documentazione API per la sincronizzazione delle opportunità: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Sincronizza i campi Ultimo momento di interesse/Punteggio MSI con SFDC.

   Una volta sincronizzati correttamente gli oggetti Salesforce in Marketo, puoi sfruttare le funzioni MSI. I campi MSI Last Interesting Moment/Scoring (Ultimo momento di interesse/Punteggio MSI) verranno esposti nell’API REST per i lead. Questi campi sono calcolati da MSI e sono di sola lettura.

   I campi Last Interesting Moment/Scoring (Ultimo momento di interesse/Punteggio) di un lead Marketo dovranno essere sincronizzati regolarmente con Salesforce utilizzando l’endpoint Lead API REST. Eseguire una query su questo endpoint per un lead di Marketo utilizzando _externalPersonId_ come filterType e passando il GUID lead di Salesforce come filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   Puoi quindi utilizzare i valori di questi campi per sincronizzarli con l’oggetto contatto/lead Salesforce.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo lead Marketo</strong></td> 
      <td><strong>Campo contatto/lead Salesforce</strong></td> 
      <td><strong>Descrizione</strong></td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentType</td> 
      <td>Etichetta: Ultimo tipo di momento di interesse<br>Nome: Last_Interesting_Moment_Type__c</td> 
      <td>Tipo dell’ultimo momento di interesse per il lead</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentDate</td> 
      <td><p>Etichetta: data ultimo momento di interesse</p><p>Nome: Last_Interesting_Moment_Date__c</p></td> 
      <td>Data dell’ultimo momento di interesse del lead</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentDesc</td> 
      <td><p>Etichetta: Descrizione ultimo momento di interesse</p><p>Nome: Last_Interesting_Moment_Desc__c</p></td> 
      <td>Descrizione dell’ultimo momento di interesse per il lead</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentSource</td> 
      <td><p>Etichetta: Last Interesting Moment Source</p><p>Nome: Last_Interesting_Moment_Source__c</p></td> 
      <td>Source dell'ultimo momento di interesse per il lead</td> 
     </tr> 
     <tr> 
      <td>priorità</td> 
      <td><p>Etichetta: Coinvolgimento</p><p>Nome: Priority__c</p></td> 
      <td>Priorità del lead</td> 
     </tr> 
     <tr> 
      <td>relativeUrgency</td> 
      <td><p>Etichetta: valore di urgenza relativa</p><p>Nome: Urgency_Value__c</p></td> 
      <td>Urgenza relativa del lead</td> 
     </tr> 
     <tr> 
      <td>relativeScoring</td> 
      <td><p>Etichetta: valore punteggio relativo</p><p>Nome: Relative_Score_Value__c</p></td> 
      <td>Punteggio relativo del lead</td> 
     </tr> 
    </tbody> 
   </table>

   Documentazione per API REST lead: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET){target="_blank"}.

   L&#39;utilizzo corretto dei campi esterni è fondamentale per una sincronizzazione non nativa riuscita. Se non riesci a visualizzare i dati in alcune visualizzazioni, è probabile che un determinato campo non sia stato sincronizzato correttamente. Ad esempio, se le attività e i momenti interessanti di un lead non vengono visualizzati quando si cerca nel widget MSI sotto il suo account, è probabile che l’azienda del lead o l’account non sia stato sincronizzato correttamente. L&#39;esecuzione di una richiesta di GET per questo lead durante la specifica dei campi esterni consente di verificare se il lead è stato sincronizzato correttamente. Inoltre, l’e-mail del venditore esterno in Marketo deve corrispondere a quella dell’utente in Salesforce. Se le e-mail non corrispondono, i dati potrebbero non essere visualizzati nella scheda Marketo di Salesforce.
