---
unique-page-id: 45417125
description: '[!DNL Sales Insight] per integrazioni non native [!DNL Salesforce] Documenti Marketo - Documentazione del prodotto'
title: '[!DNL Sales Insight] per integrazioni non native [!DNL Salesforce] '
exl-id: a771ecdf-c610-44e4-9e93-7fdcc9d79f4b
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '1200'
ht-degree: 0%

---

# [!DNL Sales Insight] per integrazioni [!DNL Salesforce] non native {#sales-insight-for-non-native-salesforce-integrations}

Se l&#39;account Adobe Marketo Engage è connesso a [!DNL Salesforce] tramite un&#39;integrazione personalizzata o non nativa, utilizzare questo articolo per configurare [!DNL Sales Insight].

>[!PREREQUISITES]
>
>* La funzione &quot;MSI non nativo&quot; è stata abilitata per l’istanza Marketo prima di avviare la configurazione di MSI. In caso contrario, e la funzionalità è già stata acquistata, contattare il [supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Se non hai ancora acquistato questa funzione, contatta il team dell’account di Adobe (il tuo Account Manager).
>* Un account Salesforce con [pacchetto MSI configurato](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.
>* Configurazione dell&#39;API REST di Marketo [completata](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}. Le API CRUD esposte costituiranno la base per l’esecuzione della sincronizzazione non nativa.
>* Leggi [questo post di blog](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"} per comprendere l&#39;oggetto e le relazioni.
>* Impostare [!DNL Salesforce] oggetti per visualizzare l&#39;identificatore univoco globale senza distinzione tra maiuscole e minuscole a 18 caratteri anziché l&#39;identificatore univoco globale con distinzione tra maiuscole e minuscole a 15 caratteri.

>[!NOTE]
>
>Impossibile utilizzare la configurazione REST API nel pannello di amministrazione di Marketo MSI per la sincronizzazione non nativa.

## Una corretta sincronizzazione non nativa per MSI richiede quanto segue {#successful-non-native-sync-for-msi-requires-the-following}

1. Sincronizzare l&#39;utente di vendita [!DNL Salesforce] con Marketo.

   L&#39;utente di vendita [!DNL Salesforce] è un utente esterno proprietario di lead/contatti in [!DNL Salesforce]. È necessario eseguire l&#39;upsert di un venditore Marketo per l&#39;utente di vendita [!DNL Salesforce]. Il campo *externalSalesPersonId* è obbligatorio per l&#39;upsert del venditore.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo Marketo Sales Person</strong></td> 
        <td><strong>Campo utente vendite <span class="dnl">Salesforce</span></strong></td> 
      <td><strong>Descrizione</strong></td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
        <td>Identificatore univoco globale di <span class="dnl">Salesforce</span> Sales User senza distinzione tra maiuscole e minuscole</td> 
      <td><p>Identifica il record Marketo Sales Person in un oggetto esterno <span class="dnl">Salesforce</span> Sales User.</p><p>Viene richiesto che il venditore venga sincronizzato prima di sincronizzare gli altri oggetti in modo da creare le relazioni appropriate.</p></td> 
     </tr> 
    </tbody> 
   </table>

   * Documentazione API per il venditore: [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/sales-persons](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/sales-persons){target="_blank"}
   * Documentazione API per la sincronizzazione del venditore: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. Sincronizza gli account [!DNL Salesforce] con Marketo.

   Per l&#39;account [!DNL Salesforce] sarà necessario eseguire l&#39;upsert di una società Marketo. I campi _externalCompanyId_ e _externalSalesPersonId_ sono obbligatori per l&#39;upsert della società.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo società Marketo</strong></td> 
        <td><strong>Campo account <span class="dnl">Salesforce</span></strong></td> 
      <td><strong>Descrizione</strong></td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
        <td>Identificatore univoco globale dell'account <span class="dnl">Salesforce</span> senza distinzione tra maiuscole e minuscole</td> 
        <td>Identifica un record società Marketo in un oggetto account <span class="dnl">Salesforce</span> esterno.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
        <td>Identificatore univoco globale di <span class="dnl">Salesforce</span> Sales User senza distinzione tra maiuscole e minuscole</td> 
        <td>Identifica un record società Marketo in un oggetto utente vendite <span class="dnl">Salesforce</span> esterno proprietario dell'account.<br><br>Utilizzato anche in Marketo per associare l'azienda al venditore proprietario del record dell'azienda. Prima di impostare questo campo, è necessario sincronizzare il rappresentante commerciale.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentazione API per le società: [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/companies](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/companies){target="_blank"}
   * Documentazione API per la sincronizzazione delle società: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Companies/operation/syncCompaniesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Companies/operation/syncCompaniesUsingPOST){target="_blank"}

1. Sincronizza lead/contatti [!DNL Salesforce] con Marketo.

   Sarà necessario eseguire l&#39;upsert di un lead Marketo per il lead/contatto [!DNL Salesforce]. I campi _externalPersonId_, _externalSalesPersonId_ e _externalCompanyId_ sono obbligatori per l&#39;upsert del lead.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo lead Marketo</strong></td> 
        <td><strong><span class="dnl">Campo contatto/lead Salesforce</span></strong></td> 
      <td><strong>Descrizione</strong></td> 
     </tr> 
     <tr> 
      <td>externalPersonId</td> 
        <td><span class="dnl">Identificatore univoco globale senza distinzione tra maiuscole e minuscole per lead/contatti di Salesforce</span></td> 
        <td>Identifica il record del lead Marketo in un oggetto <span class="dnl">lead/contatto Salesforce</span> esterno.<br><br>Questo è un nuovo campo introdotto per MSI non nativo.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
        <td>Identificatore univoco globale di <span class="dnl">Salesforce</span> Sales User senza distinzione tra maiuscole e minuscole</td> 
        <td>Identifica l'oggetto utente di vendita <span class="dnl">Salesforce</span> esterno a cui appartiene il lead/contatto.<br><br>Collega inoltre il lead con il rappresentante commerciale di Marketo. Viene richiesto di sincronizzare correttamente prima il rappresentante commerciale.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
        <td>Identificatore univoco globale dell'account <span class="dnl">Salesforce</span> senza distinzione tra maiuscole e minuscole</td> 
        <td>Identifica l'oggetto account <span class="dnl">Salesforce</span> esterno a cui appartiene il lead/contatto.<br><br>Collega inoltre il record del lead a un'azienda in Marketo. Viene richiesto prima di tutto che l’account Salesforce sia sincronizzato correttamente.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentazione API per lead: [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/leads](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/leads)
   * Documentazione API per la sincronizzazione dei lead: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST)

1. Sincronizza [!DNL Salesforce] opportunità con Marketo.

   Sarà necessario eseguire l&#39;upsert di un&#39;opportunità Marketo per l&#39;opportunità [!DNL Salesforce]. I campi _externalOpportunityId_, _externalCompanyId_ e _externalSalesPersonId_ sono obbligatori per l&#39;aggiornamento dell&#39;opportunità.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo oggetto opportunità Marketo</strong></td> 
        <td><strong>Campo oggetto opportunità <span class="dnl">Salesforce</span></strong></td> 
      <td><strong>Descrizione</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per lead/contatti di Salesforce</td> 
      <td>Identifica il record Opportunità Marketo in un oggetto Opportunità Salesforce esterno.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
        <td>Identificatore univoco globale dell'account <span class="dnl">Salesforce</span> senza distinzione tra maiuscole e minuscole</td> 
        <td>Identifica l'oggetto account <span class="dnl">Salesforce</span> esterno a cui appartiene questa opportunità. <br><br>È necessario che prima l'account <span class="dnl">Salesforce</span> sia sincronizzato correttamente.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
        <td>Identificatore univoco globale di <span class="dnl">Salesforce</span> Sales User senza distinzione tra maiuscole e minuscole</td> 
        <td>Identifica l'oggetto utente di vendita <span class="dnl">Salesforce</span> esterno a cui appartiene l'opportunità. </td> 
     </tr> 
    </tbody> 
   </table>

   * Documentazione API per l&#39;opportunità: [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * Documentazione API per la sincronizzazione delle opportunità: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Sincronizza i ruoli dei contatti di [!DNL Salesforce] con Marketo.

   È quindi possibile sincronizzare i ruoli di contatto [!DNL Salesforce] per un&#39;opportunità [!DNL Salesforce] tramite il ruolo Opportunità Marketo. Il record Ruolo opportunità richiede i campi _externalOpportunityId_, _role_ e _leadId_.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo ruolo opportunità Marketo</strong></td> 
      <td><strong>Campo ruolo contatto Salesforce</strong></td> 
      <td><strong>Descrizione</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
        <td>Identificatore univoco globale dell'opportunità <span class="dnl">Salesforce</span> senza distinzione tra maiuscole e minuscole</td> 
        <td>Identifica il ruolo opportunità Marketo in un oggetto opportunità <span class="dnl">Salesforce</span> esterno.<br><br>È necessario che prima l'opportunità <span class="dnl">Salesforce</span> sia sincronizzata correttamente.</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>N/D, sarebbe un ID lead Marketo</td> 
        <td>ID lead Marketo del contatto <span class="dnl">Salesforce</span> sincronizzato.<br><br>Una volta sincronizzato il contatto in Marketo, puoi utilizzare l'identificatore univoco globale senza distinzione tra maiuscole e minuscole di <span class="dnl">Salesforce</span> Contact come externalPersonId e eseguire una query per il lead di Marketo utilizzando l'API REST di Marketo.</td> 
     </tr> 
     <tr> 
      <td>ruolo</td> 
        <td>Campo Ruolo per il contatto <span class="dnl">Salesforce</span></td> 
      <td>Descrive il ruolo del contatto per questa opportunità.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentazione API per l&#39;opportunità: [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * Documentazione API per la sincronizzazione delle opportunità: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Sincronizza i campi Last Interesting Moment/MSI Scoring (Ultimo momento di interesse/Punteggio MSI) con SFDC.

   Dopo aver sincronizzato correttamente gli oggetti [!DNL Salesforce] in Marketo, puoi sfruttare le funzionalità MSI. I campi MSI Last Interesting Moment/Scoring (Ultimo momento di interesse/Punteggio MSI) verranno esposti nell’API REST per i lead. Questi campi sono calcolati da MSI e sono di sola lettura.

   I campi Last Interesting Moment/Scoring (Ultimo momento di interesse/Punteggio) di un lead Marketo dovranno essere sincronizzati regolarmente in [!DNL Salesforce] utilizzando l’endpoint Lead API REST. Eseguire una query su questo endpoint per un lead di Marketo utilizzando _externalPersonId_ come filterType e passando il GUID lead [!DNL Salesforce] come filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   È quindi possibile utilizzare i valori di questi campi per eseguire la sincronizzazione con l&#39;oggetto contatto/lead [!DNL Salesforce].

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo lead Marketo</strong></td> 
        <td><strong><span class="dnl">Campo contatto/lead Salesforce</span></strong></td> 
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

   L&#39;utilizzo corretto dei campi esterni è fondamentale per una sincronizzazione non nativa riuscita. Se non riesci a visualizzare i dati in alcune visualizzazioni, è probabile che un determinato campo non sia stato sincronizzato correttamente. Ad esempio, se le attività e i momenti interessanti di un lead non vengono visualizzati quando si cerca nel widget MSI sotto il suo account, è probabile che l’azienda del lead o l’account non sia stato sincronizzato correttamente. L&#39;esecuzione di una richiesta GET per questo lead durante la specifica dei campi esterni consente di verificare se il lead è stato sincronizzato correttamente. Inoltre, l’e-mail del venditore esterno in Marketo deve corrispondere a quella dell’utente in Salesforce. Se le e-mail non corrispondono, i dati potrebbero non essere visualizzati nella scheda Marketo di Salesforce.
