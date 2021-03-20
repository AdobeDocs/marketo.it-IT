---
unique-page-id: 45417125
description: Approfondimenti sulle vendite per integrazioni Salesforce non native - Documenti Marketo - Documentazione del prodotto
title: Approfondimenti vendite per integrazioni Salesforce non native
translation-type: tm+mt
source-git-commit: f3e3efc1cc480e9c6501b7e808f53c3a8bdc93d8
workflow-type: tm+mt
source-wordcount: '1277'
ht-degree: 0%

---


# Approfondimenti vendite per integrazioni Salesforce non native {#sales-insight-for-non-native-salesforce-integrations}

Se il tuo account Marketo è collegato a Salesforce tramite un’integrazione personalizzata o non nativa, utilizza questo documento per configurare Sales Insight.

>[!PREREQUISITES]
>
>* Il flag di funzione &quot;MSI non nativo&quot; abilitato per l’istanza Marketo prima di iniziare a configurare MSI (in caso contrario, contatta il tuo Customer Success Manager).
>* Un account Salesforce con [Configurazione pacchetto MSI](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md).
>* L&#39;API REST di Marketo [è stata configurata](https://developers.marketo.com/rest-api/). Le API CRUD esposte costituiranno la base per l’esecuzione della sincronizzazione non nativa.
>* Leggi [questo post di blog](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/) per avere una comprensione dell&#39;oggetto e delle relazioni.
>* Impostare gli oggetti Salesforce per visualizzare l’identificatore univoco globale senza distinzione tra maiuscole e minuscole a 18 caratteri anziché l’identificatore univoco globale con distinzione tra maiuscole e minuscole a 15 caratteri.


>[!NOTE]
>
>Impossibile utilizzare la configurazione API REST nel pannello di amministrazione Marketo MSI per la sincronizzazione non nativa.

## La sincronizzazione non nativa corretta per MSI richiede quanto segue {#successful-non-native-sync-for-msi-requires-the-following}

1. Sincronizza con Marketo l&#39;utente di vendita Salesforce.

   L&#39;Utente Vendite Salesforce è un utente esterno proprietario dei Lead/Contatti di Salesforce. È necessario che un venditore di Marketo venga aggiornato per l&#39;utente di vendita di Salesforce. Il campo *externalSalesPersonId* è obbligatorio per l&#39;upsert del venditore.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Campo Persona di vendita Marketo</strong></td> 
   <td><strong>Campo utente vendite Salesforce</strong></td> 
   <td><strong>Descrizione</strong></td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole dell'utente di Salesforce Sales</td> 
   <td><p>Identifica il record Persona di vendita Marketo in un oggetto Utente di vendita Salesforce esterno.</p><p>Viene richiesto di sincronizzare prima la persona di vendita prima di sincronizzare gli altri oggetti in modo che vengano create le relazioni corrette.</p></td> 
  </tr> 
 </tbody> 
</table>

Documentazione API per il venditore: [https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/)\
Documentazione API per la sincronizzazione del venditore: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Vendite_Persone/syncVenditePersoneUtilizzandoPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Vendite_Persone/syncVenditePersoneUtilizzandoPOST)

1. Sincronizza gli account Salesforce con Marketo.

   Una società Marketo dovrà essere aggiornata per l&#39;account Salesforce. I campi _externalCompanyId_ e _externalSalesPersonId_ sono obbligatori per l&#39;aggiornamento dell&#39;azienda.

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
   <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole dell'account Salesforce</td> 
   <td>Identifica un record aziendale Marketo in un oggetto account Salesforce esterno.</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole dell'utente di Salesforce Sales</td> 
   <td>Identifica un record della società Marketo in un oggetto dell'utente di vendita Salesforce esterno che è il proprietario dell'account.<br><br>Utilizzato anche in Marketo per associare l'Azienda al Venditore proprietario del record Azienda. Prima di impostare questo campo, è necessario che la persona di vendita sia sincronizzata.</td> 
  </tr> 
 </tbody> 
</table>

Documentazione API per le società: [https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/)\
`API documentation for syncing Companies:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST)`

1. Sincronizza i lead/contatti Salesforce con Marketo.

   Sarà necessario aggiornare un lead Marketo per il lead/contatto Salesforce. I campi _externalPersonId_, _externalSalesPersonId_ e _externalCompanyId_ sono obbligatori per l’aggiornamento del lead.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Campo lead Marketo</strong></td> 
   <td><strong>Campo lead/contatto Salesforce</strong></td> 
   <td><strong>Descrizione</strong></td> 
  </tr> 
  <tr> 
   <td>externalPersonId</td> 
   <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole di Salesforce Lead/Contact</td> 
   <td>Identifica il record Lead di Marketo in un oggetto Lead/Contact di Salesforce esterno.<br><br>Questo è un nuovo campo che viene introdotto per MSI Non-Native.</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole dell'utente di Salesforce Sales</td> 
   <td>Identifica l'oggetto Salesforce Sales User esterno proprietario del lead/contatto.<br><br>Fa anche riferimento al lead con il venditore in Marketo. È necessario che il Venditore sia prima sincronizzato correttamente.</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole dell'account Salesforce</td> 
   <td>Identifica l'oggetto account Salesforce esterno a cui appartiene il lead/contatto.<br><br>Si riferisce anche al record principale di un'azienda a Marketo. È necessario che l’account Salesforce sia prima sincronizzato correttamente.</td> 
  </tr> 
 </tbody> 
</table>

Documentazione API per i lead: [`https://developers.marketo.com/rest-api/lead-database/leads/`](https://developers.marketo.com/rest-api/lead-database/leads/)\
Documentazione API per la sincronizzazione dei lead:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST)

1. Sincronizza le opportunità di Salesforce con Marketo.

   Sarà necessario aggiornare un&#39;opportunità Marketo per l&#39;opportunità Salesforce. I campi _externalOpportunityId_, _externalCompanyId_ e _externalSalesPersonId_ sono obbligatori per l&#39;aggiornamento dell&#39;opportunità.

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
   <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole di Salesforce Lead/Contact</td> 
   <td>Identifica il record Opportunità di Marketo in un oggetto Opportunity esterno di Salesforce.</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole dell'account Salesforce</td> 
   <td>Identifica l'oggetto account Salesforce esterno a cui appartiene l'opportunità. <br><br>È necessario che l’account Salesforce sia prima sincronizzato correttamente.</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole dell'utente di Salesforce Sales</td> 
   <td>Identifica l'oggetto Salesforce Sales User esterno proprietario di questa opportunità. </td> 
  </tr> 
 </tbody> 
</table>

Documentazione API per Opportunità: [`https://developers.marketo.com/rest-api/lead-database/opportunities/`](https://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. Sincronizza i ruoli contatto Salesforce con Marketo.

   I ruoli di contatto di Salesforce per un&#39;opportunità di Salesforce possono quindi essere sincronizzati tramite il ruolo opportunità di Marketo. Il record Ruolo opportunità richiede i campi _externalOpportunityId_, _role_ e _leadId_ .

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Campo ruolo opportunità marketing</strong></td> 
   <td><strong>Campo del ruolo di contatto Salesforce</strong></td> 
   <td><strong>Descrizione</strong></td> 
  </tr> 
  <tr> 
   <td>externalOpportunityId</td> 
   <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole di Salesforce Opportunity</td> 
   <td>Identifica il ruolo opportunità di marketing in un oggetto opportunità di Salesforce esterno.<br><br>È stato richiesto che l’opportunità Salesforce sia sincronizzata correttamente per prima.</td> 
  </tr> 
  <tr> 
   <td>leadId</td> 
   <td>N/D, si tratta di un ID lead Marketo</td> 
   <td>Si tratta dell'ID lead Marketo del contatto Salesforce sincronizzato.<br><br>Una volta sincronizzato il contatto in Marketo, puoi utilizzare l’identificatore univoco globale senza distinzione tra maiuscole e minuscole di Salesforce Contact come externalPersonId e inviare una query per il lead Marketo utilizzando l’API REST di Marketo.</td> 
  </tr> 
  <tr> 
   <td>ruolo</td> 
   <td>Campo Ruolo per il contatto Salesforce</td> 
   <td>Descrive il ruolo del contatto per questa opportunità.</td> 
  </tr> 
 </tbody> 
</table>

Documentazione API per Opportunità: [`https://developers.marketo.com/rest-api/lead-database/opportunities/`](https://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. Sincronizza i campi del punteggio MSI/Momento ultimo interessante all’SFDC.

   Una volta che gli oggetti Salesforce sono correttamente sincronizzati con Marketo, è possibile sfruttare le funzioni MSI. I campi MSI Ultimo momento interessante/Punteggio saranno esposti nell’API REST per i lead. Questi campi sono calcolati da MSI e sono di sola lettura.

   I campi Ultimo momento interessante/Punteggio di un lead Marketo devono essere regolarmente sincronizzati con Salesforce utilizzando l’endpoint Lead API REST. Esegui una query su questo endpoint per un lead Marketo utilizzando _externalPersonId_ come filtroType e passando il GUID lead Salesforce come filtroValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   Puoi quindi utilizzare i valori di questi campi per eseguire la sincronizzazione con l’oggetto Lead/Contatto Salesforce.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Campo lead Marketo</strong></td> 
   <td><strong>Campo lead/contatto Salesforce</strong></td> 
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

Documentazione per l’API REST lead: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET).

L’utilizzo corretto dei campi esterni è fondamentale per una sincronizzazione non nativa corretta. Se non riesci a visualizzare i dati in alcune visualizzazioni, è probabile che un determinato campo non sia stato sincronizzato correttamente. Ad esempio, se le attività di un lead e i momenti interessanti non vengono visualizzati quando si guarda nel widget MSI sotto il proprio account, è probabile che la società del lead o l’account non siano stati sincronizzati correttamente. L’esecuzione di una richiesta di GET per questo lead quando si specificano i campi esterni consente di verificare se il lead è stato sincronizzato correttamente. Inoltre, l&#39;e-mail per il venditore esterno a Marketo deve corrispondere all&#39;e-mail per quell&#39;utente in Salesforce. I dati potrebbero non essere visualizzati nella scheda Marketo in Salesforce se le e-mail non corrispondono.
