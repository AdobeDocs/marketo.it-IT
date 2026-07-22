---
description: Note sulla versione - Maggio 2026 - Documentazione di Marketo - Documentazione del prodotto
title: Note sulla versione - Maggio 2026
feature: Release Information
source-git-commit: e8663ada66948bc30ff7ad90b26f6ba75d670ae8
workflow-type: tm+mt
source-wordcount: '760'
ht-degree: 15%

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
   <td>Beta aperta</td>
   <td><a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/marketo-ai/overview" target="_blank">Panoramica di Marketo AI</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Server MCP Marketo Engage</strong>: il server MCP Marketo Engage funge da ponte tra l'assistente AI e Marketo Engage. Espone più di 100 operazioni tra moduli, programmi, campagne intelligenti, persone/lead, e-mail, snippet, elenchi e cartelle.</td>
   <td>Beta aperta</td>
   <td><a href="https://experienceleague.adobe.com/docs/marketo-developer/marketo/mcp-server.html?lang=it" target="_blank">Server Marketo MCP</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-mail Designer - Contenuto condizionale per frammenti e-mail</strong>: <i>Parità con il vecchio editor e-mail</i>. Il contenuto condizionale è ora supportato per i frammenti.</td>
   <td>Rilasciato</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Gestione elenchi di controllo</strong>: è ora possibile specificare i valori che possono essere utilizzati nei campi di Marketo Engage.
   </td>
   <td>Rilasciato</td>
   <td><a href="/help/marketo/product-docs/administration/field-management/picklist-management.md" target="_blank">Gestione degli elenchi a discesa</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Dynamic Chat - Sta digitando</strong>: il visitatore e l'agente ricevono una notifica "sta digitando..." mentre l'altra parte sta digitando, impedendo a una di interrompere l'altra.
   </td>
   <td>Rilasciato</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Dynamic Chat - Campi elenco a discesa/elenco a discesa di Marketo</strong>: i campi elenco a discesa/elenco a discesa della persona di Marketo (inclusi i valori sincronizzati con Salesforce) sono ora disponibili come valori a discesa nell'editor dei profili di chat.
   </td>
   <td>Rilasciato</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Dynamic Chat - Stato chat non disponibile</strong>: quando un agente non accetta una chat, verrà visualizzato un nuovo stato di "chat non disponibile" nei Dettagli attività nel record della persona che ha effettuato la chat.
   </td>
   <td>Rilasciato</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Dynamic Chat - Nuovo comportamento di sincronizzazione attributi</strong>: in precedenza, l'aggiunta di nuovi attributi bloccava le modifiche nell'ambiente fino a 24 ore al termine della sincronizzazione, impedendo la modifica e la pubblicazione delle finestre di dialogo. Ora, mentre l’aggiunta di un nuovo attributo richiede ancora una sincronizzazione dati completa (che può richiedere ancora fino a 24 ore), l’ambiente non viene più bloccato durante il processo.
   </td>
   <td>Rilasciato</td>
   <td>n/d</td>
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

* **Funzionalità di unione API per campi booleani**: il comportamento dei campi booleani in un&#39;unione API è stato modificato nella versione di marzo 2026. Ora, un valore False viene trattato correttamente come se avesse un valore per quel campo. Solo un valore nullo viene considerato &quot;vuoto&quot; durante la valutazione dei campi in conflitto. Vedi [questo post della community](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/api-merge-functionality-for-boolean-fields-251219?profile.language=it){target="_blank"} per ulteriori dettagli.

* **Deprecazione parametro &#39;access_token&#39; API REST**: il parametro di query `access_token` utilizzato per autenticare le chiamate API REST di Marketo è obsoleto e non sarà disponibile dopo il 31 agosto 2026. Tutte le integrazioni nuove ed esistenti devono autenticare le chiamate API REST utilizzando l’intestazione “Authorization”, [come descritto qui](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Limite dei lead di unione API REST**: a partire dal 31 luglio 2026, le chiamate che includono più di 25 ID nel parametro leadIds di una chiamata API dei lead di unione genereranno un codice di errore 1080 e la chiamata verrà ignorata. I posti di lavoro che richiedono la fusione di più di 25 record in uno dovrebbero essere suddivisi in più lavori per garantire il successo di tali chiamate.

* **API SOAP obsoleta**: il supporto per l&#39;API Marketo SOAP terminerà il 31 luglio 2026. I servizi che utilizzano le funzionalità API SOAP devono essere migrati alle [API REST](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Limiti di dimensione elenco statico per attività Get Lead e modifiche Get Lead**: a partire dal 30 settembre 2026, le chiamate agli endpoint Get Lead Activities e Get Lead Changes che includono il parametro `listId` restituiranno un codice di errore 1003 se l&#39;elenco statico di destinazione contiene 10.000 o più lead. Per ulteriori informazioni, consultare la [Guida alla migrazione](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"}.
