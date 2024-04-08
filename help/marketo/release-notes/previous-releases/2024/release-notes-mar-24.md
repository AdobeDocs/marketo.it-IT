---
description: Note sulla versione - Marzo 2024 - Documentazione di Marketo - Documentazione del prodotto
title: Note sulla versione - Marzo 2024
feature: Release Information
exl-id: d8bc7f88-a77b-4b49-aed5-aceab9e639f0
source-git-commit: fd92f5307880019f54bb2f1778093c110a53ed2c
workflow-type: tm+mt
source-wordcount: '297'
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

* **Recupera correzione API membro del programma**: di recente è stata apportata una modifica per correggere il comportamento di [Ottieni membri del programma](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Program_Members/getProgramMembersUsingGET){target="_blank"} endpoint. In precedenza, quando si utilizzava `updatedAt` tipo di filtro per specificare un intervallo di date, è stato possibile che i record di iscrizione al programma aggiornati all’interno di tale intervallo non venissero inclusi nella risposta. Inoltre, è possibile che i record di iscrizione al programma aggiornati al di fuori dell’intervallo di date specificato non vengano inclusi correttamente nella risposta. Entrambi i problemi sono stati risolti.

* **Plug-in di Account Insight Browser obsoleto**: l’Adobe sta rimuovendo la gestione dell’account Target [Plug-in del browser Account Insight](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"} from the Chrome Web Store on April 8, 2024. Existing users: you can continue to use the plug-in until you migrate your Marketo Engage instance to Adobe Identity and Admin Console. This change **will not impact** any other TAM features/data within Marketo Engage or the Chrome and Outlook email plug-ins that work with Sales Insight. [Learn more](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}.
