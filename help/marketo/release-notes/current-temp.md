---
description: Note sulla versione corrente - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione corrente
hide: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
TQID: https://experienceleague.adobe.com/RZsCx9HAyJuDLO46WfshT30be-rMMDZjnygvU32NGfk
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: f71e690b-4480-4b67-9ef5-88f42f9cdfdbid: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2: id: c942e9f6-ed06-481a-abdd-1195363d1452
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a04ec3931933c8e6cc0a0ffc26b1b559cd7cc9ce
workflow-type: tm+mt
source-wordcount: 421
ht-degree: 28%

---

# Note sulla versione: maggio 2026 {#release-notes-may-26}

Di seguito sono elencate tutte le funzioni incluse nella versione di maggio 2026. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

Le note sulla versione specifiche per Adobe Dynamic Chat [sono disponibili qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzionalità rientrano nel ciclo di rilascio standard e inizieranno a essere rilasciate il **22 maggio 2026**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funzione</th>
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
  <tr>
   <td><strong>E-mail Designer - Contenuto condizionale per frammenti e-mail</strong>: <i>Parità con il vecchio editor e-mail</i>. Il contenuto condizionale è ora supportato per i frammenti.</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Gestione elenchi di controllo</strong>: è ora possibile specificare i valori che possono essere utilizzati nei campi di Marketo Engage.
   </td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Annunci {#announcements}

* **Campi obsoleti per funzionalità social**: nel 2025, Marketo Engage ha dichiarato obsolete le seguenti funzionalità social:

   * Sondaggi
   * Pulsante social
   * Offerta segnalata
   * Condividi video
   * Lotterie

All&#39;inizio di quest&#39;anno, i campi correlati che erano stati lasciati indietro sono stati rimossi da Marketo. Poco dopo, le richieste API che facevano riferimento a determinati campi lead correlati a Social hanno restituito un errore &quot;campo non trovato&quot;, causando interruzioni. Il servizio è stato ripristinato dopo che i campi interessati sono stati resi nuovamente disponibili, quindi per evitare ulteriori interruzioni, Marketo ha definitivamente scollegato i campi Social dalla rimozione delle funzioni Social (e come tale saranno disponibili nel tuo account Marketo). Gli utenti sono invitati a rivedere le query API e le integrazioni che fanno riferimento a campi correlati a Marketo Social e a determinare se tali campi sono ancora necessari per i processi aziendali in corso.

* **Deprecazione parametro &#39;access_token&#39; API REST**: il parametro di query `access_token` utilizzato per autenticare le chiamate API REST di Marketo è obsoleto e non sarà disponibile dopo il 31 luglio 2026. Tutte le integrazioni nuove ed esistenti devono autenticare le chiamate API REST utilizzando l’intestazione “Authorization”, [come descritto qui](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **API SOAP obsoleta**: il supporto per l&#39;API Marketo SOAP terminerà il 31 luglio 2026. I servizi che utilizzano le funzionalità API SOAP devono essere migrati alle [API REST](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Limiti di dimensione elenco statico per attività Get Lead e modifiche Get Lead**: a partire dal 30 settembre 2026, le chiamate agli endpoint Get Lead Activities e Get Lead Changes che includono il parametro `listId` restituiranno un codice di errore 1003 se l&#39;elenco statico di destinazione contiene 10.000 o più lead. Per ulteriori informazioni, consultare la [Guida alla migrazione](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"}.
