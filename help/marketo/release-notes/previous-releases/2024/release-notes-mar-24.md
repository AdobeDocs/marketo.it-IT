---
description: Note sulla versione - Marzo 2024 - Documentazione di Marketo - Documentazione del prodotto
title: Note sulla versione - Marzo 2024
feature: Release Information
exl-id: d8bc7f88-a77b-4b49-aed5-aceab9e639f0
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 3%

---

# Note sulla versione: marzo 2024 {#release-notes-mar-24}

Qui sotto troverai tutte le funzioni incluse nella versione di marzo 2024. Verifica la disponibilità delle funzioni nella tua edizione di Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![stella](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzionalità rientrano nel ciclo di rilascio standard e inizieranno a essere rilasciate il **8 marzo 2024**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Funzione</th>
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
  <tr>
   <td><strong>Logica di flusso conversazionale avanzata</strong>: aggiungere ulteriori campi per la valutazione in un'unica scelta per il follow-up del flusso conversazionale.</td>
   <td>Spedito</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Impostazioni del flusso conversazionale per Marketo Engage Forms</a></td>
  </tr>
   <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr>
   <td><strong>Riordina logica di flusso conversazionale</strong>: in Marketo Engage Forms è ora possibile riordinare le scelte di flusso conversazionale, invece di dover eliminare e aggiungere di nuovo.</td>
   <td>Spedito</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Impostazioni del flusso conversazionale per Marketo Engage Forms</a></td>
   </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>Metadati attività API</strong>:
   I metadati come Agente utente, Platform e Device sono ora inclusi nelle attività web ed e-mail, consentendo di ottenere informazioni coerenti su queste attività tramite l’API REST di Marketo.</td>
   <td>Spedito</td>
   <td>n/d</td>
  </tr>
 </tbody>
</table>
<br/>

## Annunci {#announcements}

* **Correzione API Get Program Member**: di recente è stata apportata una modifica per correggere il comportamento dell&#39;endpoint [Get Program Members](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Program-Members/operation/getProgramMembersUsingGET){target="_blank"}. In precedenza, quando si utilizzava il tipo di filtro `updatedAt` per specificare un intervallo di date, era possibile che i record di appartenenza al programma aggiornati all&#39;interno di tale intervallo non venissero inclusi nella risposta. Inoltre, è possibile che i record di iscrizione al programma aggiornati al di fuori dell’intervallo di date specificato non vengano inclusi correttamente nella risposta. Entrambi i problemi sono stati risolti.

* **Deprecazione plug-in del browser Insight per account**: Adobe rimuoverà il plug-in del browser Insight per la gestione degli account di Target [dal Web store di Chrome l&#39;8 aprile 2024. ](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"} Utenti esistenti: puoi continuare a utilizzare il plug-in fino a quando non esegui la migrazione dell’istanza Marketo Engage ad Adobe Identity e Admin Console. Questa modifica **non influirà** su altre funzionalità/dati TAM all&#39;interno di Marketo Engage o dei plug-in e-mail di Chrome e Outlook che funzionano con Sales Insight. [Ulteriori informazioni](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}.
