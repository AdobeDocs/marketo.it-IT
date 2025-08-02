---
description: Note sulla versione - Luglio 2024 - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione - Luglio 2024
feature: Release Information
exl-id: ff63af41-2d33-40f8-abca-3fd9493e7916
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 3%

---

# Note sulla versione: luglio 2024 {#release-notes-july-24}

Di seguito trovi tutte le funzioni incluse nella versione di luglio 2024. Verifica la disponibilità delle funzioni nella tua edizione di Adobe Marketo Engage.

Le note sulla versione specifiche per Adobe Dynamic Chat [ si trovano qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![stella](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzionalità rientrano nel ciclo di rilascio standard e inizieranno a essere rilasciate il **26 luglio 2024**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Funzione</th>
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
     <tr>
   <td><strong>Dashboard di coinvolgimento per i webinar interattivi</strong>: ottieni una visualizzazione delle prestazioni del webinar aggregato e una visualizzazione completa del coinvolgimento per ogni partecipante durante il webinar in modo da poter decidere quali lead indirizzare a Target tramite gli strumenti di orchestrazione di Marketo Engage.</td>
    <td>Spedito</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/engagement-dashboard.md" target="_blank">Dashboard di coinvolgimento</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr>
   <td><strong>Room Management per webinar interattivi</strong>: accedere alle singole room create (e apportare modifiche se necessario), nonché accedere al contenuto e alla registrazione (e cancellarle se necessario per ottimizzare lo storage).</td>
    <td>Spedito</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/room-management.md" target="_blank">Gestione della stanza</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr>
   <td><strong>Personalizzazione dei webinar interattivi</strong>: fornisci un'esperienza uniforme approvata dall'organizzazione tramite l'utilizzo di un'interfaccia comune per la sala riunioni, schermate intermedie (come gli sfondi delle schermate di ingresso dei partecipanti) e sfondi video personalizzati, in modo che la strategia del webinar possa allinearsi più facilmente alla strategia del marchio.</td>
    <td>Spedito</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/customization.md" target="_blank">Personalizzazione dei webinar interattivi</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr>
   <td><strong>Modifica API REST di Marketo</strong>: verrà introdotta una modifica minore alla <a href="https://developers.marketo.com/rest-api/user-management/">API di gestione utenti</a>. Entrambi gli endpoint <a href="https://developers.marketo.com/rest-api/user-management/#browse_users">Sfoglia utenti</a> e <a href="https://developers.marketo.com/rest-api/user-management/#delete_user">Elimina utente</a> supportano ora <a href="/help/marketo/product-docs/target-account-management/setup-tam/target-account-management-overview.md">Gestione account di destinazione</a> utenti.</td>
   <td>Spedito</td>
   <td>n/d</td>
  </tr>
 </tbody>
</table>
<br/>

## Annunci {#announcements}

* **Nuovo sito di documentazione per sviluppatori**: nell&#39;ambito del nostro impegno continuo per migliorare l&#39;esperienza utente di Marketo Engage, a luglio 2024 eseguiremo la migrazione di tutta la documentazione per sviluppatori ad Adobe Experience League e al sito web di Adobe Developer. [Ulteriori informazioni](https://nation.marketo.com/t5/employee-blogs/new-developer-documentation-website/ba-p/351055){target="_blank"}

* **Funzionalità social obsolete**: mercoledì 31 luglio 2024, Marketo Engage inizierà a rendere obsolete le seguenti funzionalità social all&#39;interno del prodotto:

   * Sondaggi
   * Pulsante social
   * Offerta segnalata
   * Condividi video
   * Lotterie

Gli utenti non potranno più creare, clonare o incorporare nessuna di queste funzioni social in Marketo Engage. Le risorse sociali esistenti continueranno a funzionare fino al 31 gennaio 2025. [Ulteriori informazioni](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **Token di accesso in Query Parameter Deprecation**: il supporto per l&#39;autenticazione tramite token di accesso in un parametro di query di una chiamata API REST di Marketo Engage verrà rimosso in una versione futura (data specifica da definire). Le integrazioni esistenti devono migrare all&#39;utilizzo dell&#39;intestazione Autorizzazione [qui](https://developers.marketo.com/rest-api/authentication/){target="_blank"}. Per i nuovi sviluppi, utilizza solo l’intestazione Autorizzazione per l’autenticazione con Marketo Engage.

* **È necessaria la riautenticazione di LinkedIn**: LinkedIn sta aggiornando le API marketing utilizzate dalle integrazioni LinkedIn di Marketo Engage. Per evitare interruzioni del servizio, queste modifiche richiederanno la riautenticazione di tutti i servizi LinkedIn LaunchPoint nel menu **Amministratore** > **LaunchPoint** tra il 26 luglio e il 15 dicembre 2024. Le istruzioni su come eseguire [qui per Lead Gen Forms](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md){target="_blank"} e [qui per Matched Audiences](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md){target="_blank"}. Il servizio Modulo generazione lead ha un tipo &quot;Generazione lead LinkedIn&quot; e il servizio Pubblico abbinato ha il tipo &quot;Tipi di pubblico abbinati LinkedIn&quot;. Per ulteriori informazioni, visita [Domande frequenti sulla migrazione](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.
