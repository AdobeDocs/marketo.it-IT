---
description: Note sulla versione corrente - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione corrente
hide: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
TQID: https://experienceleague.adobe.com/RZsCx9HAyJuDLO46WfshT30be-rMMDZjnygvU32NGfk
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
source-git-commit: e8663ada66948bc30ff7ad90b26f6ba75d670ae8
workflow-type: tm+mt
source-wordcount: 466
ht-degree: 23%

---

# Note sulla versione: #1 del 2 luglio 2026 {#release-notes-july-26-one}

Di seguito trovi tutte le funzioni incluse nella prima versione del 26 luglio. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

Le note sulla versione specifiche per Adobe Dynamic Chat [sono disponibili qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzionalità rientrano nel ciclo di rilascio standard e inizieranno a essere rilasciate il **10 luglio 2026**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funzione</th>
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
  <tr>
   <td><strong>Competenza Marketo AI - Conoscenza del prodotto</strong>: la conoscenza del prodotto consente l'accesso on-demand alle competenze Marketo senza uscire dalla piattaforma. Poni una domanda in un linguaggio semplice e l’intelligenza artificiale di Marketo si basa sulla documentazione ufficiale di Adobe per rispondere.
</td>
   <td>Beta aperta</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-ai/skills/product-knowledge" target="_blank">Panoramica di Marketo AI</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Abilità di Marketo AI - Indagine sui lead</strong>: scopri perché una persona/un lead specifico non ha raggiunto una fase cardine (come MQL, qualificazione del programma o una campagna) e ottieni una spiegazione semplice di ciò che è successo.
</td>
   <td>Beta aperta</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-ai/skills/investigate-leads" target="_blank">Panoramica di Marketo AI</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer e-mail - Menu contestuale dell'Assistente di intelligenza artificiale</strong>: è ora possibile accedere alle funzioni dell'Assistente di intelligenza artificiale di E-mail Designer dal menu contestuale (la barra nera). Ad esempio, quando selezioni il contenuto di testo, nel menu contestuale viene visualizzata l’icona Assistente IA, che consente di eseguire azioni rapide da lì.</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  </tr>
  </tbody>
</table>
<br/>

## Annunci {#announcements}

* **Deprecazione parametro &#39;access_token&#39; API REST**: il parametro di query `access_token` utilizzato per autenticare le chiamate API REST di Marketo è obsoleto e non sarà disponibile dopo il 31 agosto 2026. Tutte le integrazioni nuove ed esistenti devono autenticare le chiamate API REST utilizzando l’intestazione “Authorization”, [come descritto qui](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Limite dei lead di unione API REST**: a partire dal 31 luglio 2026, le chiamate che includono più di 25 ID nel parametro leadIds di una chiamata API dei lead di unione genereranno un codice di errore 1080 e la chiamata verrà ignorata. I posti di lavoro che richiedono la fusione di più di 25 record in uno dovrebbero essere suddivisi in più lavori per garantire il successo di tali chiamate.

* **API SOAP obsoleta**: il supporto per l&#39;API Marketo SOAP terminerà il 31 luglio 2026. I servizi che utilizzano le funzionalità API SOAP devono essere migrati alle [API REST](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Limiti di dimensione elenco statico per attività Get Lead e modifiche Get Lead**: a partire dal 30 settembre 2026, le chiamate agli endpoint Get Lead Activities e Get Lead Changes che includono il parametro `listId` restituiranno un codice di errore 1003 se l&#39;elenco statico di destinazione contiene 10.000 o più lead. Per ulteriori informazioni, consultare la [Guida alla migrazione](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"}.
