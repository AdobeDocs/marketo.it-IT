---
description: Note sulla versione - Marzo 2024 - Documentazione di Marketo - Documentazione del prodotto
title: Note sulla versione - Marzo 2024
feature: Release Information
exl-id: d8bc7f88-a77b-4b49-aed5-aceab9e639f0
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---

# Note sulla versione: marzo 2024 {#release-notes-mar-24}

Qui sotto troverai tutte le funzioni incluse nella versione di marzo 2024. Verifica la disponibilità delle funzioni nella tua edizione di Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Caratteristiche contrassegnate da una stella (![stella](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzioni rientrano nel ciclo di rilascio standard e inizieranno a essere rilasciate il **8 marzo 2024**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funzione</th> 
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
  <tr> 
   <td><strong>Logica di flusso conversazionale avanzata</strong>: aggiungi ulteriori campi per la valutazione in un’unica scelta per il follow-up del flusso conversazionale.</td> 
   <td>Spedito</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Impostazioni di flusso conversazionale per Forms Marketo Engage</a></td>
  </tr>
   <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr> 
   <td><strong>Riordina logica di flusso conversazionale</strong>: in Forms per Marketi Engage, è ora possibile riordinare le scelte di Flusso conversazionale, invece di dover eliminare e aggiungere di nuovo.</td> 
   <td>Spedito</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Impostazioni di flusso conversazionale per Forms Marketo Engage</a></td>
   </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Metadati attività API</strong>: i metadati come Agente utente, Platform e Device sono ora inclusi nelle attività web ed e-mail, consentendo di ottenere informazioni coerenti su queste attività tramite l’API REST di Marketo.</td> 
   <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Annunci {#announcements}

* **Recupera correzione API membro del programma**: di recente è stata apportata una modifica per correggere il comportamento di [Ottieni membri del programma](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Program-Members/operation/getProgramMembersUsingGET){target="_blank"} endpoint. In precedenza, quando si utilizzava `updatedAt` tipo di filtro per specificare un intervallo di date, è stato possibile che i record di iscrizione al programma aggiornati all’interno di tale intervallo non venissero inclusi nella risposta. Inoltre, è possibile che i record di iscrizione al programma aggiornati al di fuori dell’intervallo di date specificato non vengano inclusi correttamente nella risposta. Entrambi i problemi sono stati risolti.

* **Plug-in di Account Insight Browser obsoleto**: l’Adobe sta rimuovendo la gestione dell’account Target [Plug-in del browser Account Insight](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"} dal Chrome Web Store il 8 aprile 2024. Utenti esistenti: puoi continuare a utilizzare il plug-in fino a quando non esegui la migrazione dell’istanza di Marketo Engage a Adobe Identity e Admin Console. Questa modifica **non influirà** qualsiasi altra funzione/dato TAM all’interno di Marketi Engage o i plug-in e-mail di Chrome e Outlook che funzionano con Sales Insight. [Ulteriori informazioni](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}.
