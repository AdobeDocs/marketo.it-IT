---
description: Approfondimenti sulle vendite per le integrazioni MS Dynamics non native - Documenti Marketo - Documentazione del prodotto
title: Approfondimenti sulle vendite per le integrazioni MS Dynamics non native
exl-id: 07613ff8-b197-4a3d-88e9-720b68a6b8da
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1413'
ht-degree: 0%

---

# Approfondimenti sulle vendite per le integrazioni MS Dynamics non native {#sales-insight-for-non-native-ms-dynamics-integrations}

Se il tuo account Adobe Marketo Engage è connesso a MS Dynamics tramite un’integrazione personalizzata o non nativa, utilizza questo articolo per configurare Sales Insight.

>[!PREREQUISITES]
>
>* La funzione &quot;MSI non nativo&quot; è stata abilitata per l’istanza Marketo prima di avviare la configurazione di MSI. In caso contrario, e se hai già acquistato la funzionalità, contatta [Supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Se non hai ancora acquistato questa funzione, contatta l’Adobe Account Team (il tuo Account Manager).
>* Scarica [Pacchetto MSI per sincronizzazione personalizzata](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"}.
>* Una sottoscrizione a MS Dynamics con installazione MSI (supportata solo da [Dynamics Online](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online.md){target="_blank"} in questo momento).
>* API REST di Marketo [configurazione completata](https://developers.marketo.com/rest-api/){target="_blank"}. Le API CRUD esposte costituiranno la base per l’esecuzione della sincronizzazione non nativa.
>* Letto [questo post di blog](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"} per comprendere l&#39;oggetto e le relazioni.

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

   * Documentazione API per il venditore: [https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/){target="_blank"}
   * Documentazione API per la sincronizzazione del venditore: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST){target="_blank"}

1. Sincronizza gli account di MS Dynamics con Marketo.

   Per l’account MS Dynamics sarà necessario eseguire l’upsert di una società Marketo. Il _externalCompanyId_ e _externalSalesPersonId_ I campi sono obbligatori per la parte superiore dell’Azienda.

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
      <td>Identifica un record Società Marketo in un oggetto utente esterno di MS Dynamics Sales proprietario dell'account.<br><br>Utilizzato anche in Marketo per associare l'Azienda al Venditore che è il proprietario del documento aziendale. Prima di impostare questo campo, è necessario sincronizzare il rappresentante commerciale.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentazione API per le aziende: [https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/){target="_blank"}
   * Documentazione API per le società di sincronizzazione: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST){target="_blank"}

1. Sincronizza lead/contatti di MS Dynamics con Marketo.

   È necessario eseguire l’upsert di un lead Marketo per il lead/contatto MS Dynamics. Il _externalPersonId_, _externalSalesPersonId_, e _externalCompanyId_ I campi sono obbligatori per la parte superiore del lead.

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
      <td>Identifica l’oggetto utente esterno di MS Dynamics Sales proprietario di questo lead/contatto.<br><br>Inoltre mette in relazione il lead con il venditore in Marketo. Viene richiesto di sincronizzare correttamente prima il rappresentante commerciale.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole dell’account MS Dynamics</td> 
      <td>Identifica l’oggetto account MS Dynamics esterno a cui appartiene il lead/contatto.<br><br>Inoltre mette in relazione il record del lead con un'Azienda in Marketo. Viene richiesto prima di tutto di sincronizzare correttamente l’account MS Dynamics.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentazione API per lead: [https://developers.marketo.com/rest-api/lead-database/leads/](https://developers.marketo.com/rest-api/lead-database/leads/){target="_blank"}
   * Documentazione API per la sincronizzazione dei lead: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST){target="_blank"}

1. Sincronizza opportunità MS Dynamics con Marketo.

   È necessario eseguire l’upsert di un’opportunità Marketo per l’opportunità MS Dynamics. Il _externalOpportunityId_, _externalCompanyId_, e _externalSalesPersonId_ I campi sono obbligatori per l’upsert dell’opportunità.

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
      <td>Identifica l’oggetto account MS Dynamics esterno a cui appartiene questa opportunità. <br><br>Viene richiesto prima di tutto di sincronizzare correttamente l’account MS Dynamics.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per l’utente di MS Dynamics Sales</td> 
      <td>Identifica l’oggetto utente esterno di MS Dynamics Sales a cui appartiene questa opportunità. </td> 
     </tr> 
    </tbody> 
   </table>

   * Documentazione API per Opportunity: [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target="_blank"}
   * Documentazione API per la sincronizzazione delle opportunità: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST){target="_blank"}

1. Sincronizza i ruoli dei contatti di MS Dynamics con Marketo.

   I ruoli di contatto di MS Dynamics per un’opportunità MS Dynamics possono quindi essere sincronizzati tramite il ruolo Opportunità di Marketo. Il record Ruolo opportunità richiede _externalOpportunityId_, _ruolo_, e _leadId_ campi.

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
      <td>Identifica il ruolo opportunità Marketo in un oggetto opportunità MS Dynamics esterno.<br><br>È necessario innanzitutto sincronizzare correttamente l’opportunità MS Dynamics.</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>N/D, sarebbe un ID lead Marketo</td> 
      <td>Questo sarebbe l’ID lead Marketo del contatto sincronizzato con MS Dynamics.<br><br>Una volta sincronizzato il contatto in Marketo, puoi utilizzare l’identificatore univoco globale senza distinzione tra maiuscole e minuscole di MS Dynamics Contact come externalPersonId e eseguire una query per il lead di Marketo utilizzando l’API REST di Marketo.</td> 
     </tr> 
     <tr> 
      <td>ruolo</td> 
      <td>Campo Ruolo per il contatto MS Dynamics</td> 
      <td>Descrive il ruolo del contatto per questa opportunità.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentazione API per Opportunity: [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target="_blank"}
   * Documentazione API per la sincronizzazione delle opportunità: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST){target="_blank"}

1. Sincronizza i campi Ultimo momento di interesse/Punteggio MSI con MS Dynamics.

   Una volta sincronizzati correttamente gli oggetti MS Dynamics in Marketo, puoi sfruttare le funzioni MSI. I campi MSI Last Interesting Moment/Scoring (Ultimo momento di interesse/Punteggio MSI) verranno esposti nell’API REST per i lead. Questi campi sono calcolati da MSI e sono di sola lettura.

   I campi Last Interesting Moment/Scoring (Ultimo momento di interesse/Punteggio) di un lead Marketo dovranno essere sincronizzati regolarmente con MS Dynamics utilizzando l’endpoint Lead API REST. Eseguire una query su questo endpoint per un lead di Marketo utilizzando _externalPersonId_ come filterType e trasmissione del GUID di MS Dynamics come filterValue.

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
      <td>Etichetta: ultimo tipo di momento di interesse<br>Nome: Last_Interesting_Moment_Type__c</td> 
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
      <td><p>Etichetta: Ultima origine momento di interesse</p><p>Nome: Last_Interesting_Moment_Source__c</p></td> 
      <td>Sorgente dell’ultimo momento interessante per il lead</td> 
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

   * Documentazione per l’API REST lead: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET){target="_blank"}.

   L&#39;utilizzo corretto dei campi esterni è fondamentale per una sincronizzazione non nativa riuscita. Se non riesci a visualizzare i dati in alcune visualizzazioni, è probabile che un determinato campo non sia stato sincronizzato correttamente. Ad esempio, se le attività e i momenti interessanti di un lead non vengono visualizzati quando si cerca nel widget MSI sotto il suo account, è probabile che l’azienda del lead o l’account non sia stato sincronizzato correttamente. L&#39;esecuzione di una richiesta di GET per questo lead durante la specifica dei campi esterni consente di verificare se il lead è stato sincronizzato correttamente. Inoltre, l’e-mail per il venditore esterno in Marketo deve corrispondere a quella per tale utente in MS Dynamics. Se le e-mail non corrispondono, i dati potrebbero non essere visualizzati nella scheda Marketo in MS Dynamics.
