---
description: Approfondimenti sulle vendite per le integrazioni MS Dynamics non native - Documenti Marketo - Documentazione del prodotto
title: Approfondimenti sulle vendite per le integrazioni MS Dynamics non native
exl-id: 07613ff8-b197-4a3d-88e9-720b68a6b8da
feature: Marketo Sales Insights
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 0%

---

# Approfondimenti sulle vendite per le integrazioni MS Dynamics non native {#sales-insight-for-non-native-ms-dynamics-integrations}

Se il tuo account Adobe Marketo Engage è connesso a MS Dynamics tramite un’integrazione personalizzata o non nativa, utilizza questo articolo per configurare Sales Insight.

>[!PREREQUISITES]
>
>* La funzione &quot;MSI non nativo&quot; è stata abilitata per l’istanza Marketo prima di avviare la configurazione di MSI. In caso contrario, e la funzionalità è già stata acquistata, contatta il [supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Se non hai ancora acquistato questa funzione, contatta l’Adobe Account Team (il tuo Account Manager).
>* Scarica [pacchetto MSI per sincronizzazione personalizzata](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"}.
>* Una sottoscrizione a MS Dynamics con installazione MSI (al momento sono supportati solo [Dynamics Online](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online.md){target="_blank"}).
>* Configurazione dell&#39;API REST di Marketo [completata](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}. Le API CRUD esposte costituiranno la base per l’esecuzione della sincronizzazione non nativa.
>* Leggi [questo post di blog](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"} per comprendere l&#39;oggetto e le relazioni.

## Una corretta sincronizzazione non nativa per MSI richiede quanto segue {#successful-non-native-sync-for-msi-requires-the-following}

1. Sincronizzare l&#39;utente di MS Dynamics Sales con Marketo.

   L’utente di MS Dynamics Sales è un utente esterno proprietario di lead/contatti in MS Dynamics. È necessario eseguire l&#39;upsert di un addetto alle vendite Marketo per l&#39;utente di vendita MS Dynamics. Il campo externalSalesPersonId è obbligatorio per l&#39;upsert del venditore.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo Marketo Sales Person</strong></td> 
      <td><strong>Campo utente MS Dynamics</strong></td> 
      <td><strong>Descrizione</strong></td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per l’utente di MS Dynamics</td> 
      <td><p>Identifica il record Marketo Sales Person in un oggetto utente esterno di MS Dynamics.</p><p>Viene richiesto che il venditore venga sincronizzato prima di sincronizzare gli altri oggetti in modo da creare le relazioni appropriate.</p></td> 
     </tr> 
    </tbody> 
   </table>

   * [Documentazione API per il venditore](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/lead-database/sales-persons){target="_blank"}
   * [Documentazione API per la sincronizzazione del venditore](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. Sincronizza gli account di MS Dynamics con Marketo.

   Per l’account MS Dynamics sarà necessario eseguire l’upsert di una società Marketo. I campi _externalCompanyId_ e _externalSalesPersonId_ sono obbligatori per l&#39;upsert della società.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo società Marketo</strong></td> 
      <td><strong>Campo account MS Dynamics</strong></td> 
      <td><strong>Descrizione</strong></td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole dell’account MS Dynamics</td> 
      <td>Identifica un record Società Marketo in un oggetto account MS Dynamics esterno.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per l’utente di MS Dynamics Sales</td> 
      <td>Identifica un record Società Marketo in un oggetto utente esterno di MS Dynamics Sales proprietario dell'account.<br><br>Utilizzato anche in Marketo per associare l'azienda al venditore proprietario del record dell'azienda. Prima di impostare questo campo, è necessario sincronizzare il rappresentante commerciale.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentazione API per le società: [https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/lead-database/companies](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/lead-database/companies){target="_blank"}
   * Documentazione API per la sincronizzazione delle società: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. Sincronizza lead/contatti di MS Dynamics con Marketo.

   È necessario eseguire l’upsert di un lead Marketo per il lead/contatto MS Dynamics. I campi _externalPersonId_, _externalSalesPersonId_ e _externalCompanyId_ sono obbligatori per l&#39;upsert del lead.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo lead Marketo</strong></td> 
      <td><strong>Campo contatto/lead di MS Dynamics</strong></td> 
      <td><strong>Descrizione</strong></td> 
     </tr> 
     <tr> 
      <td>externalPersonId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per lead/contatti di MS Dynamics</td> 
      <td>Identifica il record Lead di Marketo in un oggetto contatto/lead di MS Dynamics esterno.<br><br>Questo è un nuovo campo introdotto per MSI non nativo.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per l’utente di MS Dynamics Sales</td> 
      <td>Identifica l’oggetto utente esterno di MS Dynamics Sales proprietario di questo lead/contatto.<br><br>Collega inoltre il lead con il rappresentante commerciale di Marketo. Viene richiesto di sincronizzare correttamente prima il rappresentante commerciale.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole dell’account MS Dynamics</td> 
      <td>Identifica l’oggetto account MS Dynamics esterno a cui appartiene il lead/contatto.<br><br>Collega inoltre il record del lead a un'azienda in Marketo. Viene richiesto prima di tutto di sincronizzare correttamente l’account MS Dynamics.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentazione API per lead: [https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/lead-database/lead-database](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/lead-database/lead-database){target="_blank"}
   * Documentazione API per la sincronizzazione dei lead: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST){target="_blank"}

1. Sincronizza opportunità MS Dynamics con Marketo.

   È necessario eseguire l’upsert di un’opportunità Marketo per l’opportunità MS Dynamics. I campi _externalOpportunityId_, _externalCompanyId_ e _externalSalesPersonId_ sono obbligatori per l&#39;aggiornamento dell&#39;opportunità.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo oggetto opportunità Marketo</strong></td> 
      <td><strong>Campo oggetto opportunità MS Dynamics</strong></td> 
      <td><strong>Descrizione</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per lead/contatti di MS Dynamics</td> 
      <td>Identifica il record Opportunità Marketo in un oggetto Opportunità MS Dynamics esterno.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole dell’account MS Dynamics</td> 
      <td>Identifica l’oggetto account MS Dynamics esterno a cui appartiene questa opportunità. <br><br>È necessario che prima l'account MS Dynamics sia sincronizzato correttamente.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per l’utente di MS Dynamics Sales</td> 
      <td>Identifica l’oggetto utente esterno di MS Dynamics Sales a cui appartiene questa opportunità. </td> 
     </tr> 
    </tbody> 
   </table>

   * Documentazione API per l&#39;opportunità: [https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * Documentazione API per la sincronizzazione delle opportunità: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Sincronizza i ruoli dei contatti di MS Dynamics con Marketo.

   I ruoli di contatto di MS Dynamics per un’opportunità MS Dynamics possono quindi essere sincronizzati tramite il ruolo Opportunità di Marketo. Il record Ruolo opportunità richiede i campi _externalOpportunityId_, _role_ e _leadId_.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo ruolo opportunità Marketo</strong></td> 
      <td><strong>Campo ruolo contatto MS Dynamics</strong></td> 
      <td><strong>Descrizione</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per l’opportunità MS Dynamics</td> 
      <td>Identifica il ruolo opportunità Marketo in un oggetto opportunità MS Dynamics esterno.<br><br>È necessario prima sincronizzare correttamente l'opportunità MS Dynamics.</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>N/D, sarebbe un ID lead Marketo</td> 
      <td>Questo sarebbe l’ID lead Marketo del contatto sincronizzato con MS Dynamics.<br><br>Una volta sincronizzato il contatto in Marketo, puoi utilizzare l'identificatore univoco globale senza distinzione tra maiuscole e minuscole di MS Dynamics Contact come externalPersonId e eseguire una query per il lead di Marketo utilizzando l'API REST di Marketo.</td> 
     </tr> 
     <tr> 
      <td>ruolo</td> 
      <td>Campo Ruolo per il contatto MS Dynamics</td> 
      <td>Descrive il ruolo del contatto per questa opportunità.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentazione API per l&#39;opportunità: [https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * Documentazione API per la sincronizzazione delle opportunità: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Sincronizza i campi Ultimo momento di interesse/Punteggio MSI con MS Dynamics.

   Una volta sincronizzati correttamente gli oggetti MS Dynamics in Marketo, puoi sfruttare le funzioni MSI. I campi MSI Last Interesting Moment/Scoring (Ultimo momento di interesse/Punteggio MSI) verranno esposti nell’API REST per i lead. Questi campi sono calcolati da MSI e sono di sola lettura.

   I campi Last Interesting Moment/Scoring (Ultimo momento di interesse/Punteggio) di un lead Marketo dovranno essere sincronizzati regolarmente con MS Dynamics utilizzando l’endpoint Lead API REST. Eseguire una query su questo endpoint per un lead di Marketo utilizzando _externalPersonId_ come filterType e passando il GUID lead di MS Dynamics come filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=MS DynamicsLeadId1,MS DynamicsLeadId2 |
   |---|

   Puoi quindi utilizzare i valori di questi campi per sincronizzarli con l’oggetto contatto/lead di MS Dynamics.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo lead Marketo</strong></td> 
      <td><strong>Campo contatto/lead di MS Dynamics</strong></td> 
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

   * Documentazione per API REST lead: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET){target="_blank"}.

   L&#39;utilizzo corretto dei campi esterni è fondamentale per una sincronizzazione non nativa riuscita. Se non riesci a visualizzare i dati in alcune visualizzazioni, è probabile che un determinato campo non sia stato sincronizzato correttamente. Ad esempio, se le attività e i momenti interessanti di un lead non vengono visualizzati quando si cerca nel widget MSI sotto il suo account, è probabile che l’azienda del lead o l’account non sia stato sincronizzato correttamente. L&#39;esecuzione di una richiesta di GET per questo lead durante la specifica dei campi esterni consente di verificare se il lead è stato sincronizzato correttamente. Inoltre, l’e-mail per il venditore esterno in Marketo deve corrispondere a quella per tale utente in MS Dynamics. Se le e-mail non corrispondono, i dati potrebbero non essere visualizzati nella scheda Marketo in MS Dynamics.
