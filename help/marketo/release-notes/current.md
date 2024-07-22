---
description: Note sulla versione corrente - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione corrente
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: cb69844d8e9e25cae19bc2d4a91c28376f58eadb
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 1%

---

# Note sulla versione: luglio 2024 {#release-notes-july-24}

Di seguito trovi tutte le funzioni incluse nella versione di luglio 2024. Verifica la disponibilità delle funzioni nella tua edizione di Adobe Marketo Engage.

Le note sulla versione specificatamente per l&#39;Adobe Dynamic Chat [ si trovano qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![stella](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

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
   <td><strong>Dashboard di coinvolgimento per i webinar interattivi</strong>: ottieni una visualizzazione delle prestazioni del webinar aggregato e una visualizzazione completa del coinvolgimento per ogni partecipante durante il webinar in modo da poter decidere quali lead indirizzare a target tramite gli strumenti di orchestrazione del Marketo Engage.</td> 
    <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>Room Management per webinar interattivi</strong>: accedere alle singole room create (e apportare modifiche se necessario), nonché accedere al contenuto e alla registrazione (e cancellarle se necessario per ottimizzare lo storage).</td> 
    <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>Personalizzazione dei webinar interattivi</strong>: fornisci un'esperienza uniforme approvata dall'organizzazione tramite l'utilizzo di un'interfaccia comune per la sala riunioni, schermate intermedie (come gli sfondi delle schermate di ingresso dei partecipanti) e sfondi video personalizzati, in modo che la strategia del webinar possa allinearsi più facilmente alla strategia del marchio.</td> 
    <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>Modifica API REST di Marketo</strong>: verrà introdotta una modifica minore alla <a href="https://developers.marketo.com/rest-api/user-management/">API di gestione utenti</a>. Entrambi gli endpoint <a href="https://developers.marketo.com/rest-api/user-management/#browse_users">Sfoglia utenti</a> e <a href="https://developers.marketo.com/rest-api/user-management/#delete_user">Elimina utente</a> supportano ora <a href="/help/marketo/product-docs/target-account-management/setup-tam/target-account-management-overview.md">Gestione account di destinazione</a> utenti.</td> 
   <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Annunci {#announcements}

* **Nuovo sito di documentazione per sviluppatori**: nell&#39;ambito del nostro impegno continuo per migliorare l&#39;esperienza utente del Marketo Engage, a luglio 2024 eseguiremo la migrazione di tutta la documentazione per sviluppatori al sito Web Adobe Experience League e Adobe Developer. [Ulteriori informazioni](https://nation.marketo.com/t5/employee-blogs/new-developer-documentation-website/ba-p/351055){target="_blank"}

* **Token di accesso in Query Parameter Deprecation**: il supporto per l&#39;autenticazione tramite token di accesso in un parametro di query di una chiamata API REST di Marketo Engage verrà rimosso in una versione futura (data specifica da definire). Le integrazioni esistenti devono migrare all&#39;utilizzo dell&#39;intestazione Autorizzazione [qui](https://developers.marketo.com/rest-api/authentication/){target="_blank"}. Per i nuovi sviluppi, utilizza solo l’intestazione Autorizzazione per l’autenticazione con il Marketo Engage.

* **È richiesta la riautenticazione di LinkedIn**: LinkedIn sta aggiornando le API marketing utilizzate dalle integrazioni LinkedIn di Marketo Engage. Per evitare interruzioni del servizio, queste modifiche richiederanno la riautenticazione di tutti i servizi LinkedIn LaunchPoint nel menu **Amministratore** > **LaunchPoint** tra il 26 luglio e il 15 dicembre 2024. Le istruzioni su come eseguire [qui per Lead Gen Forms](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md){target="_blank"} e [qui per Matched Audiences](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md){target="_blank"}. Il servizio Modulo generazione lead ha un tipo di &quot;LinkedIn Lead Gen&quot; e il servizio Pubblico abbinato ha il tipo di &quot;LinkedIn Matched Audiences&quot;. Per ulteriori informazioni, vedere le [Domande frequenti sulla migrazione](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.
