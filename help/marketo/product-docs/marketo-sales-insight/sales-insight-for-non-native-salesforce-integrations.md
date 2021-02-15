---
unique-page-id: 45417125
description: Informazioni sulle vendite per integrazioni Salesforce non native - Documenti Marketo - Documentazione prodotto
title: Informazioni sulle vendite per integrazioni Salesforce non native
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '1269'
ht-degree: 0%

---


# Informazioni sulle vendite per integrazioni Salesforce non native {#sales-insight-for-non-native-salesforce-integrations}

Se il tuo account Marketo è connesso a Salesforce tramite un&#39;integrazione personalizzata o non nativa, usa questo documento per configurare Vendite Insight.

>[!PREREQUISITES]
>
>* Rivolgiti al tuo Customer Success Manager per abilitare la funzionalità &quot;MSI non nativa&quot; per l&#39;istanza di Marketo.
>* Un account Salesforce con configurazione pacchetto MSI.
>* Impostazione dell&#39;API REST di Marketo [completata](https://developers.marketo.com/rest-api/). Le API CRUD esposte costituiranno la base per eseguire la sincronizzazione non nativa.
>* Leggi [questo post di blog](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/) per conoscere l&#39;oggetto e le relazioni.
>* Configurate gli oggetti Salesforce per visualizzare l&#39;identificatore univoco globale senza distinzione tra maiuscole e minuscole di 18 caratteri anziché l&#39;identificatore univoco globale con distinzione tra maiuscole e minuscole di 15 caratteri.

>



>[!NOTE]
>
>La configurazione REST API nel pannello di amministrazione MSI di Marketo non può essere utilizzata per la sincronizzazione non nativa.

## La sincronizzazione non nativa corretta per MSI richiede quanto segue{#successful-non-native-sync-for-msi-requires-the-following}

1. Sincronizza l’utente di vendita Salesforce con il marketing.

   L&#39;utente di vendita Salesforce è un utente esterno proprietario dei lead/contatti in Salesforce. È necessario aggiornare un addetto alle vendite marketing per l&#39;utente delle vendite Salesforce. Il campo *externalSalesPersonId* è obbligatorio per l&#39;upsert del Sales Person.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Campo Persona di vendita Marketo</strong></td> 
   <td><strong>Campo Utente Vendite Salesforce</strong></td> 
   <td><strong>Descrizione</strong></td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per l'utente di Salesforce Sales</td> 
   <td><p>Identifica il record Persona di vendita Marketo in un oggetto Vendite Salesforce esterno.</p><p>Viene richiesto di sincronizzare prima la Persona di vendita prima di sincronizzare gli altri oggetti in modo da creare le relazioni corrette.</p></td> 
  </tr> 
 </tbody> 
</table>

Documentazione API per il venditore: [https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/)\
Documentazione API per la sincronizzazione della persona di vendita: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Person/syncSalesPersonUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Person/syncSalesPersonUsingPOST)

1. Sincronizza gli account Salesforce con Marketo.

   Per l&#39;account Salesforce sarà necessario aggiornare una società Marketing. I campi *externalCompanyId* e *externalSalesPersonId* sono obbligatori per l&#39;aggiornamento della Società.

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
   <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per l'account Salesforce</td> 
   <td>Identifica un record Marketing Company in un oggetto Salesforce Account esterno.</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per l'utente di Salesforce Sales</td> 
   <td>Identifica un record Marketing Company con un oggetto Salesforce Sales User esterno proprietario dell'account.<br><br>Utilizzata anche all'interno di Marketo per associare la Società alla Persona di vendita che possiede il record della Società. Prima di impostare questo campo è necessario che il Sales Person sia sincronizzato.</td> 
  </tr> 
 </tbody> 
</table>

Documentazione API per le aziende: [https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/)\
`API documentation for syncing Companies:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST)`

1. Sincronizza i lead/contatti Salesforce con Marketo.

   Dovrai aggiornare un lead marketing per il lead/contatto Salesforce. I campi *externalPersonId*, *externalSalesPersonId* e *externalCompanyId* sono obbligatori per l&#39;aggiornamento del lead.

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
   <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole in Salesforce Lead/Contact</td> 
   <td>Identifica il record Marketo Lead su un oggetto Lead/Contatto Salesforce esterno.<br><br>Questo è un nuovo campo che viene introdotto per MSI non-Native.</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per l'utente di Salesforce Sales</td> 
   <td>Identifica l'oggetto Salesforce Sales User esterno proprietario di questo lead/contatto.<br><br>Collega inoltre il lead al venditore in Marketo. È stato imposto di far sì che il Sales Person sia sincronizzato correttamente per primo.</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per l'account Salesforce</td> 
   <td>Identifica l’oggetto Account Salesforce esterno a cui appartiene il lead/contatto.<br><br>Si riferisce anche al record principale di un'azienda di Marketo. Viene richiesto di sincronizzare per primo l'account Salesforce correttamente.</td> 
  </tr> 
 </tbody> 
</table>

Documentazione API per i lead: [`https://developers.marketo.com/rest-api/lead-database/leads/`](https://developers.marketo.com/rest-api/lead-database/leads/)\
Documentazione API per la sincronizzazione dei lead:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST)

1. Sincronizza opportunità Salesforce con Marketing.

   Dovrai aumentare un&#39;opportunità di marketing per l&#39;opportunità di Salesforce. I campi *externalOpportunityId*, *externalCompanyId* e *externalSalesPersonId* sono obbligatori per l&#39;aggiornamento dell&#39;opportunità.

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
   <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole in Salesforce Lead/Contact</td> 
   <td>Identifica il record Opportunità di marketing in un oggetto Opportunità Salesforce esterno.</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per l'account Salesforce</td> 
   <td>Identifica l'oggetto Account Salesforce esterno a cui appartiene l'opportunità. <br><br>Viene richiesto di sincronizzare per primo l'account Salesforce correttamente.</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per l'utente di Salesforce Sales</td> 
   <td>Identifica l'oggetto Salesforce Sales User esterno proprietario di questa opportunità. </td> 
  </tr> 
 </tbody> 
</table>

Documentazione API per Opportunità: [`https://developers.marketo.com/rest-api/lead-database/opportunities/`](https://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. Sincronizza i ruoli dei contatti Salesforce con Marketo.

   I ruoli dei contatti di Salesforce per un&#39;opportunità Salesforce possono essere quindi sincronizzati tramite il ruolo opportunità di marketing. Il record Ruolo opportunità richiede i campi *externalOpportunityId*, *role* e *leadId*.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Campo ruolo opportunità marketing</strong></td> 
   <td><strong>Campo ruolo contatto Salesforce</strong></td> 
   <td><strong>Descrizione</strong></td> 
  </tr> 
  <tr> 
   <td>externalOpportunityId</td> 
   <td>Identificatore univoco globale senza distinzione tra maiuscole e minuscole per Salesforce Opportunity</td> 
   <td>Identifica il ruolo opportunità di marketing per un oggetto Opportunità Salesforce esterno.<br><br>Viene richiesto di sincronizzare per primo l’opportunità Salesforce correttamente.</td> 
  </tr> 
  <tr> 
   <td>leadId</td> 
   <td>N/D: si tratta di un ID lead Marketo</td> 
   <td>Si tratta dell'ID lead Marketo del contatto Salesforce sincronizzato.<br><br>Una volta che il contatto è sincronizzato in Marketo, puoi utilizzare l’identificatore univoco globale senza distinzione tra maiuscole e minuscole di Salesforce Contact come identificatore esternoPersonId e query per il lead Marketo tramite l’API REST di Marketo.</td> 
  </tr> 
  <tr> 
   <td>role</td> 
   <td>Campo Ruolo per il contatto Salesforce</td> 
   <td>Descrive il ruolo del contatto per questa opportunità.</td> 
  </tr> 
 </tbody> 
</table>

Documentazione API per Opportunità: [`https://developers.marketo.com/rest-api/lead-database/opportunities/`](https://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. Sincronizza i campi Momento/Punteggio MSI più interessanti in SFDC.

   Una volta che gli oggetti Salesforce sono stati sincronizzati correttamente su Marketo, potete sfruttare le funzioni MSI. I campi MSI Last Interesting Moment/Scoring (Ultimo momento/punteggio) saranno esposti nell&#39;API REST per i lead. Questi campi sono calcolati da MSI e sono di sola lettura.

   I campi Momento/Punteggio ultimo interesse di un lead Marketo dovranno essere sincronizzati regolarmente con Salesforce utilizzando l’endpoint Lead API REST. Esegui una query su questo endpoint per un lead Marketo utilizzando *externalPersonId* come filterType e trasferendo il GUID del lead Salesforce come filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   Puoi quindi utilizzare i valori di questi campi per sincronizzare l&#39;oggetto Lead/Contatto di Salesforce.

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
   <td><p>Etichetta: Data ultimo momento interessante</p><p>Nome: Last_Interesting_Moment_Date_c</p></td> 
   <td>Data dell'ultimo momento interessante per il lead</td> 
  </tr> 
  <tr> 
   <td>msiLastInterestingMomentDesc</td> 
   <td><p>Etichetta: Descrizione ultimo momento interessante</p><p>Nome: Last_Interesting_Moment_Desc_c</p></td> 
   <td>Descrizione dell'ultimo momento interessante per il lead</td> 
  </tr> 
  <tr> 
   <td>msiLastInterestingMomentSource</td> 
   <td><p>Etichetta: Ultima origine momento interessante</p><p>Nome: Last_Interesting_Moment_Source_c</p></td> 
   <td>Fonte dell'ultimo momento interessante per il lead</td> 
  </tr> 
  <tr> 
   <td>priority</td> 
   <td><p>Etichetta: Coinvolgimento</p><p>Nome: Priority_c</p></td> 
   <td>Priorità del lead</td> 
  </tr> 
  <tr> 
   <td>relativeUrency</td> 
   <td><p>Etichetta: Valore di urgenza relativo</p><p>Nome: Urency_Value_c</p></td> 
   <td>Urgenza relativa del lead</td> 
  </tr> 
  <tr> 
   <td>relativeScoring</td> 
   <td><p>Etichetta: Valore punteggio relativo</p><p>Nome: Relative_Score_Value_c</p></td> 
   <td>Punteggio relativo del lead</td> 
  </tr> 
 </tbody> 
</table>

Documentazione per l’API REST principale:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET).

L&#39;uso corretto dei campi esterni è fondamentale per una sincronizzazione non nativa di successo. Se in alcune viste i dati non vengono visualizzati, è probabile che un determinato campo non sia stato sincronizzato correttamente. Ad esempio, se le attività di un lead e i momenti interessanti non vengono visualizzati quando si guarda nel widget MSI sotto il proprio account, è probabile che la società del lead o l’account non siano stati sincronizzati correttamente. L’esecuzione di una richiesta di GET per questo lead mentre si specificano i campi esterni consente di verificare se il lead è stato sincronizzato correttamente. Inoltre, l&#39;e-mail per il venditore esterno a Marketo deve corrispondere all&#39;e-mail per quell&#39;utente in Salesforce. I dati potrebbero non essere visualizzati nella scheda Marketo di Salesforce se le e-mail non corrispondono.

