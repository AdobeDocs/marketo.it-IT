---
description: Note sulla versione corrente - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione corrente
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
TQID: https://experienceleague.adobe.com/QJFy7PeGXlvS3jcJGcZJROlc8c1UvphO-TOOwPUQeX8
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 7853491f53bd2f7d5ec6e63189c1e8b77b4b5349
workflow-type: tm+mt
source-wordcount: 543
ht-degree: 23%

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
   <td><strong>Marketo AI</strong>: utilizza una suite di agenti progettati per automatizzare funzioni di marketing lunghe ma importanti (due agenti disponibili ora e altri in arrivo).
</td>
   <td>Disponibilità limitata (<a href="https://forms.cloud.microsoft/Pages/ResponsePage.aspx?id=Wht7-jR7h0OUrtLBeN7O4Y-uSf63sAxCmWyqMJg8eMFUMVZSVExSNDA3T0I4SEcwRDFSVTBGWU01Uy4u&origin=QRCode">richiedere l'accesso qui</a>)</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-ai/overview">Panoramica di Marketo AI</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <th style="width:65%">Funzione</th>
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
  <tr>
   <td><strong>Server MCP Marketo Engage</strong>: il server MCP Marketo Engage funge da ponte tra l'assistente AI e Marketo Engage. Espone più di 100 operazioni tra moduli, programmi, campagne intelligenti, persone/lead, e-mail, snippet, elenchi e cartelle.</td>
   <td>Disponibilità limitata (<a href="https://forms.cloud.microsoft/Pages/ResponsePage.aspx?id=Wht7-jR7h0OUrtLBeN7O4Y-uSf63sAxCmWyqMJg8eMFUMVZSVExSNDA3T0I4SEcwRDFSVTBGWU01Uy4u&origin=QRCode">richiedere l'accesso qui</a>)</td>
   <td><a href="https://experienceleague.corp.adobe.com/docs/marketo-developer/marketo/mcp-server.html">Server Marketo MCP</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
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
