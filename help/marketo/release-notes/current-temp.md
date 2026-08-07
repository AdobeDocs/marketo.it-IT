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
source-git-commit: ebd911b99e1c4c8f8a76db3a14235ee0d4ee0485
workflow-type: tm+mt
source-wordcount: 408
ht-degree: 28%

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
   <td><strong>Nuova interfaccia utente di Marketo Engage</strong>: l'interfaccia di Marketo Engage ha un aspetto aggiornato, inclusi menu, icone e layout aggiornati per un'esperienza più pulita e moderna. Questo è solo un aggiornamento visivo, non influisce su alcuna funzionalità o flusso di lavoro esistente.
</td>
   <td>Rollout graduale nel corso del mese di agosto</td>
   <td><i>n/d</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Invia e-mail a Designer - Generatore di script</strong>: Script Builder è un assistente basato sull'intelligenza artificiale che consente di creare script di personalizzazione più rapidamente.
</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Disabilita campagne nell'archivio</strong>: l'archiviazione di una cartella ora disattiva e depianifica tutte le campagne nella struttura di cartelle, impedendo l'esecuzione imprevista delle campagne Smart archiviate.
</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Annunci {#announcements}

* **Deprecazione parametro &#39;access_token&#39; API REST**: il parametro di query `access_token` utilizzato per autenticare le chiamate API REST di Marketo è obsoleto e non sarà disponibile dopo il 31 agosto 2026. Tutte le integrazioni nuove ed esistenti devono autenticare le chiamate API REST utilizzando l’intestazione “Authorization”, [come descritto qui](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **ID esecuzione campagna REST API**: il supporto per l&#39;API SOAP di Marketo terminerà il 31 luglio 2026. I servizi che utilizzano le funzionalità API SOAP devono essere migrati alle [API REST](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
* **Limiti di dimensioni elenco statico per attività Get Lead e Get Lead Changes**: in alcune circostanze, il valore ID esecuzione campagna di un&#39;attività veniva talvolta restituito con una formattazione errata, tra due coppie di virgolette (ad esempio, `"campaignRunId": ""102938""`).<br/>
A partire dalla versione di agosto, questo valore verrà sempre restituito con il formato numerico corretto (`"campaignRunId": 102938`)

* **Limite dei lead di unione API REST**: a partire dal 31 luglio 2026, le chiamate che includono più di 25 ID nel parametro leadIds di una chiamata API dei lead di unione restituiscono un codice di errore 1080 e la chiamata viene ignorata. I posti di lavoro che richiedono la fusione di più di 25 record in uno dovrebbero essere suddivisi in più lavori per garantire il successo di tali chiamate.
