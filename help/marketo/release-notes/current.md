---
description: Note sulla versione corrente - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione corrente
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: ea9bf2a002415936cdfb5bfb723ce80723003da5
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 2%

---

# Note sulla versione: luglio 2024 {#release-notes-july-24}

Qui sotto troverai tutte le funzioni incluse nella versione di giugno 2024. Verifica la disponibilità delle funzioni nella tua edizione di Adobe Marketo Engage.

Le Note sulla versione, ad Adobe Dynamic Chat [si trova qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Caratteristiche contrassegnate da una stella (![stella](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzioni rientrano nel ciclo di rilascio standard e inizieranno a essere rilasciate il **26 luglio 2024**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funzione</th> 
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
     <tr> 
   <td><strong>Modifica API REST di Marketo</strong>: stiamo introducendo una modifica minore al <a href="https://developers.marketo.com/rest-api/user-management/">API User Management</a>. Entrambe <a href="https://developers.marketo.com/rest-api/user-management/#browse_users">Sfoglia utenti</a> e <a href="https://developers.marketo.com/rest-api/user-management/#delete_user">Elimina utente</a> gli endpoint ora supportano <a href="/help/marketo/product-docs/target-account-management/setup-tam/target-account-management-overview.md">Gestione account di destinazione</a> utenti.</td> 
   <td><i>in arrivo</i></td>
   <td><i>in arrivo</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Annunci {#announcements}

* **Nuovo sito di documentazione per sviluppatori**: come parte del nostro impegno continuo per migliorare l’esperienza utente del Marketo Engage, a luglio 2024 eseguiremo la migrazione di tutta la documentazione per sviluppatori al sito web Adobe Experience League e Adobe Developer. [Ulteriori informazioni](https://nation.marketo.com/t5/employee-blogs/new-developer-documentation-website/ba-p/351055){target="_blank"}

* **Token di accesso in Query Parameter Deprecation**: il supporto per l’autenticazione tramite token di accesso in un parametro di query di una chiamata API REST di Marketo Engage verrà rimosso in una versione futura (data specifica TBD). Le integrazioni esistenti devono migrare all’utilizzo dell’intestazione Autorizzazione [descritto qui](https://developers.marketo.com/rest-api/authentication/){target="_blank"}. Per i nuovi sviluppi, utilizza solo l’intestazione Autorizzazione per l’autenticazione con il Marketo Engage.

* **È necessaria la riautenticazione di linkedIn**: LinkedIn sta aggiornando le API di marketing utilizzate dalle integrazioni Marketo Engage LinkedIn. Queste modifiche richiederanno la riautenticazione di tutti i servizi LinkedIn LaunchPoint nel tuo **Amministratore** > **LaunchPoint** tra il 26 luglio e il 15 dicembre 2024, per evitare interruzioni del servizio. Puoi trovare istruzioni su come eseguire questa operazione [qui per Lead Gen Forms](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md){target="_blank"} e [qui per tipi di pubblico corrispondenti](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md){target="_blank"}. Il servizio Modulo generazione lead ha un tipo di &quot;LinkedIn Lead Gen&quot; e il servizio Pubblico abbinato ha il tipo di &quot;LinkedIn Matched Audiences&quot;. Per ulteriori informazioni, vedere [Domande frequenti sulla migrazione](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.
