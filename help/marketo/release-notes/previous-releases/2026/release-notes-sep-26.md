---
description: Note sulla versione - Settembre 2026 - Documentazione di Marketo - Documentazione del prodotto
title: Note sulla versione - Settembre 2026
feature: Release Information
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
    internal-label: Resources
subfeature_v2:
  - id: af97ce94-35fa-4fa9-b85a-46b752ac4028
    internal-label: Release information
source-git-commit: 9eb8c0e78a581bc9093f0f017a3ad3525d2b9667
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 14%
---
# Note sulla versione: settembre 2026 {#release-notes-sep-26}

Di seguito sono elencate tutte le funzioni incluse nella versione di settembre 2026. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

Le note sulla versione specifiche per Adobe Dynamic Chat [sono disponibili qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzionalità rientrano nel ciclo di rilascio standard e inizieranno a essere rilasciate il **25 settembre 2026**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funzione</th>
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
  <tr>
   <td><strong>Nuova interfaccia utente di Marketo Engage</strong>: l'interfaccia di Marketo Engage ha un aspetto aggiornato, inclusi menu, icone e layout aggiornati per un'esperienza più pulita e moderna. Questo è solo un aggiornamento visivo; non influisce su alcuna funzionalità o flusso di lavoro esistente. <i>La possibilità di selezionare l'interfaccia utente classica sarà disponibile a partire dalla versione di gennaio 2027</i>.
</td>
   <td>Disponibilità generale entro metà ottobre</td>
   <td><i>n/d</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Seleziona partizione durante l'importazione</strong>: è ora possibile effettuare una selezione dall'elenco di partizioni dell'area di lavoro locale durante l'importazione di record di persone in ambienti in cui sono abilitate aree di lavoro e partizioni.</td>
   <td>Rilasciato</td>
   <td><a href="https://experienceleague.adobe.com/it/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people#step-import-your-spreadsheet-into-marketo:~:text=If%20you%20have%20Person%20Partitions%20set%20up" target="_blank">Importazione elenco</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Passaggi del flusso self-service - Timeout callback aumentato</strong>: il periodo di timeout callback per i passaggi del flusso self-service viene aumentato da un'ora a quattro ore. Non è richiesta alcuna azione da parte tua.</td>
   <td>Rilasciato</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-mail Designer - Tabelle</strong>: ora puoi trascinare e rilasciare il tipo di contenuto "tabella" nel messaggio e-mail, impostando il numero di colonne e righe.</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Annunci {#announcements}

* **Restrizioni nome API per attributi attività personalizzati**: i nomi API per attributi attività personalizzati creati tramite API o interfaccia utente possono ora contenere solo caratteri alfanumerici e trattini bassi e devono iniziare con un carattere alfanumerico.

* **Limiti di dimensione elenco statico per attività Get Lead e modifiche Get Lead**: a partire dal 30 settembre 2026, le chiamate agli endpoint Get Lead Activities o Get Lead Changes che includono il parametro `listId` non riusciranno e restituiranno il codice di errore 1003 (a indicare che l&#39;elenco statico di destinazione contiene troppi record) se gli elenchi di destinazione contengono 10.000 o più lead. Per ulteriori informazioni, consultare la [Guida alla migrazione](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"}.

* **Deprecazione parametro &#39;access_token&#39; REST API**: il parametro di query `access_token` utilizzato per autenticare le chiamate API REST di Marketo è stato dichiarato obsoleto il 31 agosto 2026. Tutte le integrazioni nuove ed esistenti devono autenticare le chiamate API REST utilizzando l’intestazione “Authorization”, [come descritto qui](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **ID esecuzione campagna REST API**: in alcune circostanze, il valore ID esecuzione campagna di un&#39;attività veniva talvolta restituito con una formattazione errata, tra due coppie di virgolette (ad esempio, `"campaignRunId": ""102938""`).<br/>A partire dalla versione di agosto, questo valore verrà sempre restituito con il formato numerico corretto (`"campaignRunId": 102938`).

* **Deprecazione delle immagini di acquisizione dal Web**: per conformarsi alle moderne best practice per la protezione e la privacy, la funzionalità [Immagini di acquisizione dal Web](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/demand-generation/images-and-files/grab-the-images-from-a-web-page){target="_blank"} diventerà obsoleta a partire dalla versione di ottobre.
