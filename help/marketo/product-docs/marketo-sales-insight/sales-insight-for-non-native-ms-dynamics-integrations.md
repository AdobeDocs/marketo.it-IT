---
description: Approfondimenti sulle vendite per integrazioni MS Dynamics non native - Documentazione Marketo - Documentazione del prodotto
title: Approfondimenti vendite per integrazioni di MS Dynamics non native
exl-id: 07613ff8-b197-4a3d-88e9-720b68a6b8da
source-git-commit: ff076d66a193664aa6ec05cf940143cebdd2d942
workflow-type: tm+mt
source-wordcount: '1439'
ht-degree: 0%

---

# Approfondimenti vendite per integrazioni di MS Dynamics non native {#sales-insight-for-non-native-ms-dynamics-integrations}

Se il tuo account Adobe Marketo Engage è connesso a MS Dynamics tramite un’integrazione personalizzata o non nativa, utilizza questo articolo per configurare Sales Insight.

>[!PREREQUISITES]
>
>* La funzione &quot;MSI non nativa&quot; abilitata per la tua istanza Marketo prima di iniziare a configurare MSI (se non lo è e hai già acquistato la funzione, contatta [Supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target=&quot;_blank&quot;} - se non hai ancora acquistato questa funzionalità, contatta il tuo Customer Success Manager).
>* Scarica [Pacchetto MSI per sincronizzazione personalizzata](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target=&quot;_blank&quot;}.
>* Una sottoscrizione a MS Dynamics con configurazione MSI ([On-Prem](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-365.md){target=&quot;_blank&quot;}, [Dynamics Online](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online.md){target=&quot;_blank&quot;}).
>* API REST di Marketo [configurazione completata](https://developers.marketo.com/rest-api/){target=&quot;_blank&quot;}. Le API CRUD esposte costituiranno la base per l’esecuzione della sincronizzazione non nativa.
>* Leggi [questo post di blog](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target=&quot;_blank&quot;} per comprendere l&#39;oggetto e le relazioni.


## La sincronizzazione non nativa corretta per MSI richiede quanto segue {#successful-non-native-sync-for-msi-requires-the-following}

1. Sincronizza l’utente di vendita di MS Dynamics con Marketo.

   L’utente di vendita di MS Dynamics è un utente esterno proprietario dei lead/contatti in MS Dynamics. È necessario aggiornare un venditore Marketo per l’utente di vendite di MS Dynamics. Il campo externalSalesPersonId è obbligatorio per l&#39;upsert della persona di vendita.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo Persona di vendita Marketo</strong></td> 
      <td><strong>Campo utente di MS Dynamics</strong></td> 
      <td><strong>Descrizione</strong></td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per l’utente di MS Dynamics</td> 
      <td><p>Identifica il record Marketo Sales Person in un oggetto MS Dynamics User esterno.</p><p>È necessario che il Venditore sia sincronizzato prima di sincronizzare gli altri oggetti in modo che vengano create le relazioni corrette.</p></td> 
     </tr> 
    </tbody> 
   </table>

   * Documentazione API per il venditore: [https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/){target=&quot;_blank&quot;}
   * Documentazione API per la sincronizzazione del venditore: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Vendite_Persone/syncVenditePersoneUtilizzandoPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Vendite_Persone/syncVenditePersoneUtilizzandoPOST){target=&quot;_blank&quot;}

1. Sincronizza gli account di MS Dynamics con Marketo.

   Sarà necessario aggiornare una società Marketo per l’account MS Dynamics. La _externalCompanyId_ e _externalSalesPersonId_ i campi sono obbligatori per l&#39;utente dell&#39;Azienda.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo società Marketo</strong></td> 
      <td><strong>Campo account di MS Dynamics</strong></td> 
      <td><strong>Descrizione</strong></td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole dell’account di MS Dynamics</td> 
      <td>Identifica un record aziendale Marketo in un oggetto account MS Dynamics esterno.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per l'utente di MS Dynamics Sales</td> 
      <td>Identifica un record aziendale Marketo in un oggetto utente di vendita MS Dynamics esterno proprietario dell'account.<br><br>Utilizzato anche all'interno di Marketo per associare l'Azienda al Venditore proprietario del record Azienda. Prima di impostare questo campo, è necessario che la persona di vendita sia sincronizzata.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentazione API per le società: [https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/){target=&quot;_blank&quot;}
   * Documentazione API per le società di sincronizzazione: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST){target=&quot;_blank&quot;}

1. Sincronizza i lead/contatti di MS Dynamics con Marketo.

   Sarà necessario aggiornare un lead Marketo per MS Dynamics Lead/Contact. La _externalPersonId_, _externalSalesPersonId_ e _externalCompanyId_ I campi sono obbligatori per l’aggiornamento del lead.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo lead Marketo</strong></td> 
      <td><strong>Campo lead/contatto di MS Dynamics</strong></td> 
      <td><strong>Descrizione</strong></td> 
     </tr> 
     <tr> 
      <td>externalPersonId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole di MS Dynamics Lead/Contact</td> 
      <td>Identifica il record Lead di Marketo in un oggetto Lead/Contact di MS Dynamics esterno.<br><br>Questo è un nuovo campo che viene introdotto per MSI Non-Native.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per l'utente di MS Dynamics Sales</td> 
      <td>Identifica l’oggetto utente di vendita MS Dynamics esterno proprietario del lead/contatto.<br><br>Fa anche riferimento al lead con il venditore in Marketo. È necessario che il Venditore sia prima sincronizzato correttamente.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole dell’account di MS Dynamics</td> 
      <td>Identifica l’oggetto account MS Dynamics esterno a cui appartiene il lead/contatto.<br><br>Si riferisce anche al record principale di un'azienda in Marketo. È necessario che l’account MS Dynamics sia prima sincronizzato correttamente.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentazione API per i lead: [https://developers.marketo.com/rest-api/lead-database/leads/](https://developers.marketo.com/rest-api/lead-database/leads/){target=&quot;_blank&quot;}
   * Documentazione API per la sincronizzazione dei lead: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST){target=&quot;_blank&quot;}

1. Sincronizza le opportunità di MS Dynamics con Marketo.

   Sarà necessario aggiornare un’opportunità Marketo per MS Dynamics. La _externalOpportunityId_, _externalCompanyId_ e _externalSalesPersonId_ I campi sono obbligatori per l&#39;upsert dell&#39;opportunità.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo oggetto opportunità Marketo</strong></td> 
      <td><strong>Campo oggetto opportunità per MS Dynamics</strong></td> 
      <td><strong>Descrizione</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole di MS Dynamics Lead/Contact</td> 
      <td>Identifica il record Opportunità di Marketo in un oggetto Opportunity di MS Dynamics esterno.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole dell’account di MS Dynamics</td> 
      <td>Identifica l’oggetto account MS Dynamics esterno a cui appartiene l’opportunità. <br><br>È necessario che l’account MS Dynamics sia prima sincronizzato correttamente.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per l'utente di MS Dynamics Sales</td> 
      <td>Identifica l’oggetto utente di vendita di MS Dynamics esterno proprietario di questa opportunità. </td> 
     </tr> 
    </tbody> 
   </table>

   * Documentazione API per Opportunità: [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target=&quot;_blank&quot;}
   * Documentazione API per le opportunità di sincronizzazione: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunità/sincrOpportunitàUtilizzo di POST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunità/sincrOpportunitàUtilizzo di POST){target=&quot;_blank&quot;}

1. Sincronizza i ruoli del contatto di MS Dynamics con Marketo.

   I ruoli di contatto di MS Dynamics per un’opportunità di MS Dynamics possono quindi essere sincronizzati tramite il ruolo opportunità di Marketo. Il record Ruolo opportunità richiede il _externalOpportunityId_, _ruolo_ e _leadId_ campi.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo ruolo opportunità Marketo</strong></td> 
      <td><strong>Campo del ruolo di contatto di MS Dynamics</strong></td> 
      <td><strong>Descrizione</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per MS Dynamics Opportunity</td> 
      <td>Identifica il ruolo opportunità di Marketo in un oggetto opportunità di MS Dynamics esterno.<br><br>È stato richiesto che l’opportunità di MS Dynamics sia sincronizzata correttamente per prima.</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>N/D, si tratta di un Marketo Lead ID</td> 
      <td>Si tratta dell’ID lead Marketo del contatto con MS Dynamics sincronizzato.<br><br>Una volta sincronizzato il contatto in Marketo, è possibile utilizzare l’identificatore univoco globale senza distinzione tra maiuscole e minuscole di MS Dynamics Contact come externalPersonId ed eseguire una query per il lead Marketo utilizzando l’API REST di Marketo.</td> 
     </tr> 
     <tr> 
      <td>ruolo</td> 
      <td>Campo Ruolo per il contatto MS Dynamics</td> 
      <td>Descrive il ruolo del contatto per questa opportunità.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentazione API per Opportunità: [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target=&quot;_blank&quot;}
   * Documentazione API per le opportunità di sincronizzazione: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunità/sincrOpportunitàUtilizzo di POST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunità/sincrOpportunitàUtilizzo di POST){target=&quot;_blank&quot;}

1. Sincronizza i campi del punteggio MSI/Momento più interessante in MS Dynamics.

   Una volta sincronizzati correttamente gli oggetti MS Dynamics in Marketo, è possibile sfruttare le funzioni MSI. I campi MSI Ultimo momento interessante/Punteggio saranno esposti nell’API REST per i lead. Questi campi sono calcolati da MSI e sono di sola lettura.

   I campi Ultimo momento interessante/Punteggio di un lead Marketo devono essere regolarmente sincronizzati in MS Dynamics utilizzando l’endpoint REST API Lead. Eseguire una query dell’endpoint per un lead Marketo utilizzando _externalPersonId_ come filterType e passando il GUID di MS Dynamics come filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=MS DynamicsLeadId1,MS DynamicsLeadId2 |
   |---|

   È quindi possibile utilizzare i valori di questi campi per eseguire la sincronizzazione con l’oggetto MS Dynamics Lead/Contact.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo lead Marketo</strong></td> 
      <td><strong>Campo lead/contatto di MS Dynamics</strong></td> 
      <td><strong>Descrizione</strong></td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentType</td> 
      <td>Etichetta: Ultimo tipo di momento interessante<br>Nome: Last_Interesting_Moment_Type_c</td> 
      <td>Tipo dell'ultimo momento interessante per il lead</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentDate</td> 
      <td><p>Etichetta: Data ultimo momento interessante</p><p>Nome: Last_Interesting_Moment_Date__c</p></td> 
      <td>Data dell'ultimo momento interessante per il lead</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentDesc</td> 
      <td><p>Etichetta: Descrizione dell'ultimo momento interessante</p><p>Nome: Last_Interesting_Moment_Desc_c</p></td> 
      <td>Descrizione dell'ultimo momento interessante per il lead</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentSource</td> 
      <td><p>Etichetta: Ultima origine momento interessante</p><p>Nome: Last_Interesting_Moment_Source_c</p></td> 
      <td>Fonte dell'ultimo momento interessante per il piombo</td> 
     </tr> 
     <tr> 
      <td>priorità</td> 
      <td><p>Etichetta: Coinvolgimento</p><p>Nome: Priority_c</p></td> 
      <td>Priorità del lead</td> 
     </tr> 
     <tr> 
      <td>relativaUrgenza</td> 
      <td><p>Etichetta: Valore di urgenza relativo</p><p>Nome: Urgenza_Valore_c</p></td> 
      <td>Urgenza relativa del lead</td> 
     </tr> 
     <tr> 
      <td>relativeScoring</td> 
      <td><p>Etichetta: Valore di punteggio relativo</p><p>Nome: Relative_Score_Value_c</p></td> 
      <td>Punteggio relativo del lead</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentazione per l’API REST lead: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET){target=&quot;_blank&quot;}.
   L’utilizzo corretto dei campi esterni è fondamentale per una sincronizzazione non nativa corretta. Se non riesci a visualizzare i dati in alcune visualizzazioni, è probabile che un determinato campo non sia stato sincronizzato correttamente. Ad esempio, se le attività di un lead e i momenti interessanti non vengono visualizzati quando si guarda nel widget MSI sotto il proprio account, è probabile che la società del lead o l’account non siano stati sincronizzati correttamente. L’esecuzione di una richiesta di GET per questo lead quando si specificano i campi esterni consente di verificare se il lead è stato sincronizzato correttamente. Inoltre, l’e-mail per il venditore esterno in Marketo deve corrispondere all’e-mail per tale utente in MS Dynamics. I dati potrebbero non essere visualizzati nella scheda Marketo di MS Dynamics se le e-mail non corrispondono.
