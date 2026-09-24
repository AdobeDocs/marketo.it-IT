---
description: Note sulla versione - Luglio 2026 - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione - Luglio 2026
feature: Release Information
source-git-commit: 15308a78867253ae6c54faa8e77c2cf7eb68b9a5
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 13%
---
# Note sulla versione: agosto 2026 {#release-notes-aug-26}

Qui sotto trovi tutte le funzioni incluse nella versione di agosto 2026. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

Le note sulla versione specifiche per Adobe Dynamic Chat [sono disponibili qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzionalità rientrano nel ciclo di rilascio standard e inizieranno a essere rilasciate il **14 agosto 2026**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funzione</th>
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
  <tr>
   <td><strong>Nuova interfaccia utente di Marketo Engage</strong>: l'interfaccia di Marketo Engage ha un aspetto aggiornato, inclusi menu, icone e layout aggiornati per un'esperienza più pulita e moderna. Questo è solo un aggiornamento visivo; non influisce su alcuna funzionalità o flusso di lavoro esistente.
</td>
   <td>Rollout graduale nei mesi di agosto e settembre</td>
   <td><i>n/d</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Server MCP Marketo Engage</strong>: il server MCP Marketo Engage funge da ponte tra l'assistente AI e Marketo Engage. Espone più di 100 operazioni tra moduli, programmi, campagne intelligenti, persone/lead, e-mail, snippet, elenchi e cartelle.</td>
   <td>Generalmente disponibile</td>
   <td><a href="https://experienceleague.adobe.com/docs/marketo-developer/marketo/mcp-server.html?lang=it" target="_blank">Server Marketo MCP</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Disabilita campagne nell'archivio</strong>: l'archiviazione di una cartella ora disattiva e depianifica tutte le campagne nella struttura di cartelle, impedendo l'esecuzione imprevista delle campagne Smart archiviate.
</td>
   <td>Rilasciato</td>
   <td><a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-folders#disable-campaigns-archive" target="_blank">Disabilita campagne nell'archivio</a></td>
  </tr>
    <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer e-mail - Genera contenuto menu contestuale</strong>: le funzioni "Genera contenuto" di Designer e-mail sono ora accessibili dal menu contestuale (la barra nera). Ad esempio, quando selezioni il contenuto di testo, l’icona Genera contenuto viene visualizzata nel menu contestuale, consentendo di eseguire azioni rapide.</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Annunci {#announcements}

* **Marketo AI è ora Coworker per Marketo Engage**: Coworker per Marketo Engage fornisce competenze di agente progettate per automatizzare le funzioni di marketing che richiedono tempo. Nuovo nome, stesse funzioni, disponibile per tutti gli utenti. [Ulteriori informazioni](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/coworker-for-marketo/overview){target="_blank"}

* **Deprecazione parametro &#39;access_token&#39; REST API**: il parametro di query `access_token` utilizzato per autenticare le chiamate API REST di Marketo è obsoleto e non sarà disponibile dopo il 31 agosto 2026. Tutte le integrazioni nuove ed esistenti devono autenticare le chiamate API REST utilizzando l’intestazione “Authorization”, [come descritto qui](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **ID esecuzione campagna REST API**: in alcune circostanze, il valore ID esecuzione campagna di un&#39;attività veniva talvolta restituito con una formattazione errata, tra due coppie di virgolette (ad esempio, `"campaignRunId": ""102938""`).<br/>A partire dalla versione di agosto, questo valore verrà sempre restituito con il formato numerico corretto (`"campaignRunId": 102938`)

* **Limiti di dimensione elenco statico per attività Get Lead e modifiche Get Lead**: a partire dal 30 settembre 2026, le chiamate agli endpoint Get Lead Activities o Get Lead Changes che includono il parametro `listId` non riusciranno e restituiranno il codice di errore 1003 (a indicare che l&#39;elenco statico di destinazione contiene troppi record) se gli elenchi di destinazione contengono 10.000 o più lead. Per ulteriori informazioni, consultare la [Guida alla migrazione](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"}.

* **Limite dei lead di unione API REST**: a partire dal 31 luglio 2026, le chiamate che includono più di 25 ID nel parametro leadIds di una chiamata API dei lead di unione restituiscono un codice di errore 1080 e la chiamata viene ignorata. I posti di lavoro che richiedono la fusione di più di 25 record in uno dovrebbero essere suddivisi in più lavori per garantire il successo di tali chiamate.
