---
description: Note sulla versione - Gennaio 2025 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Gennaio 2025
feature: Release Information
exl-id: fd816b9c-9e06-4292-87d6-9fa991c4681f
source-git-commit: f806c0984cf221bd88fdf50013a8f1d2911b5d86
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 35%

---

# Note sulla versione - Gennaio 2025 {#release-notes-jan-25}

Qui sotto troverai tutte le funzioni incluse nella versione di gennaio 2025. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

Le note sulla versione specifiche per Adobe Dynamic Chat [sono disponibili qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![star](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzioni rientrano nel ciclo di rilascio standard. Inizieranno a essere rilasciate il **sabato 17 gennaio 2025**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Funzione</th>
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
    <tr>
   <td><strong>Nuovo Designer e-mail</strong>: crea e-mail moderne ed efficienti utilizzando il nuovo Designer e-mail nativo in Marketo Engage. Accedi a uno dei modelli e-mail predefiniti oppure creane facilmente uno tuo. Utilizza i contenuti dinamici e accedi alle immagini da Adobe Experience Manager Cloud Services. Utilizza la funzionalità Content Accelerator Gen-AI per creare e-mail innovative e performanti su larga scala.
   <p><img src="assets/note-icon.png" alt="icona nota"> NOTA: per accedere al nuovo e-mail designer, è necessario eseguire la migrazione della sottoscrizione di Marketo Engage a <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview">Adobe Identity Management System (IMS)</a>. Se non lo hai ancora fatto e desideri richiederne la rapidità, contatta il team dell'account Adobe (il tuo account manager) o il <a href="https://nation.marketo.com/t5/support/ct-p/Support">supporto Marketo</a>. Per accedere alla funzionalità Content Accelerator Gen-AI, contatta il team dell’account Adobe.</td>
   <td>Rilasciato</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/overview.md">Panoramica di E-mail designer</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Annulla registrazione partecipanti da un evento nei webinar interattivi</strong>: se non desideri un partecipante al webinar per qualsiasi motivo, puoi annullarne la registrazione. Il flusso di lavoro rimuove il registrante sia dal programma Marketo Event che da Adobe Connect.</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Disabilita campagne nell'archivio</strong>: disabilita le campagne con trigger attivo e annulla eventuali esecuzioni batch pianificate di campagne in una cartella al momento dell'archiviazione. Poiché è in corso un controllo aggiuntivo delle autorizzazioni per l'archiviazione di cartelle che contengono campagne attive (Attiva campagna trigger e Pianifica campagna batch), questa funzione viene disabilitata per impostazione predefinita con questa versione e può essere abilitata passando a <b>Amministratore</b> &gt; <b>Sfondo tesoro</b> nella sottoscrizione Marketo Engage.</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
 </tbody>
</table>
<br/>

## Annunci {#announcements}

* **Funzionalità social obsolete**: mercoledì 31 luglio 2024, Marketo Engage ha iniziato a rendere obsolete le seguenti funzionalità social all&#39;interno del prodotto:

   * Sondaggi
   * Pulsante social
   * Offerta segnalata
   * Condividi video
   * Lotterie

Da allora, gli utenti non sono stati in grado di creare, clonare o incorporare nessuna di queste funzioni Social in Marketo Engage. Le risorse sociali esistenti continuano a funzionare fino al 31 gennaio 2025. Il 1° febbraio 2025 le risorse social cesseranno di funzionare. Le funzioni social incorporate nelle pagine di destinazione dovranno essere rimosse. [Ulteriori informazioni](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **Aggiornamento API Get Program Members**: è stata migliorata l&#39;API [Get Program Members](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/lead-database/program-members#query){target="_blank"} per supportare la possibilità di recuperare l&#39;identificatore dei membri del programma. A questo scopo, aggiungi l’ID all’elenco di campi specificati nel parametro fields della richiesta API.

* **Deprecazione parametro &#39;access_token&#39; API Rest**: il parametro di query `access_token` utilizzato per autenticare le chiamate API REST di Marketo è obsoleto e non sarà più disponibile dopo il mercoledì 31 marzo 2026. Tutte le integrazioni nuove ed esistenti devono autenticare le chiamate API REST utilizzando l’intestazione &#39;Authorization&#39;, [come descritto qui](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Deprecazione API SOAP**: il supporto per l’API SOAP di Marketo terminerà il mercoledì 31 marzo 2026. I servizi che utilizzano le funzionalità API SOAP devono effettuare la migrazione all’[API REST](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
