---
description: Note sulla versione corrente - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione corrente
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 433aae54a012e6bbf04c90056d8815a88e76498c
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 2%

---

# Note sulla versione: aprile 2024 {#release-notes-apr-24}

Di seguito sono riportate tutte le funzioni incluse nella versione di aprile 2024. Verifica la disponibilità delle funzioni nella tua edizione di Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Caratteristiche contrassegnate da una stella (![stella](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzioni rientrano nel ciclo di rilascio standard e inizieranno a essere rilasciate il **26 aprile 2024**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funzione</th> 
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
   <tr> 
   <td><strong>Modelli per webinar interattivi</strong>: consente di risparmiare tempo creando modelli personalizzati per i layout delle stanze con specifiche adatte alla propria organizzazione.</td> 
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
   <td><strong>Miglioramenti ai webinar interattivi</strong>: ora puoi fornire a host e relatori la possibilità di aggiungere un titolo del webinar, rinominare una room e sincronizzare manualmente i dati del coinvolgimento dopo la consegna dell’evento.</td> 
   <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Miglioramenti di Audit Trail</strong>: è ora possibile acquisire nuovi tipi di azioni in Audit Trail per le modifiche apportate in Gestione campi, le modifiche apportate a Utenti e ruoli e il numero di persone esportate da elenchi ed elenchi avanzati.</td> 
   <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Nuovi utenti e ruoli - Autorizzazioni</strong>: sono disponibili nuove autorizzazioni che forniscono agli utenti un accesso più granulare al Marketo Engage. Controlla le parti dell’amministratore non gestite in precedenza, ad esempio Nuova esperienza e Predictive Audiences, divide le autorizzazioni per concedere separatamente l’accesso all’Asset Audit Trail e all’Admin Audit Trail e utilizza le nuove autorizzazioni di creazione e spostamento per le risorse e le cartelle per impedire che gli utenti di sola lettura apportino modifiche.</td> 
   <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Annunci {#announcements}

* **Aggiornamento API delle attività**: il 26 aprile, stiamo aggiungendo diversi nuovi attributi alle attività basate su web e e-mail che vengono restituiti quando recuperi le attività utilizzando [API REST di Marketo](https://developers.marketo.com/rest-api/lead-database/activities/){target="_blank"}. The activities listed below will now include Browser, Platform, Device, and User Agent attributes. Call the [Get Activity Types](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Activities/getAllActivityTypesUsingGET){target="_blank"} endpoint per rivedere i dettagli dell&#39;attributo per ogni attività.

**Attività basate sul web**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:30%">Attività</th> 
   <th style="width:70%">Attributi appena aggiunti</th>
   </tr>
  <tr> 
   <td>Visita pagina Web</td> 
   <td>Browser, Platform, Device</td>
  </tr>
   <tr> 
   <td>Compila modulo</td> 
   <td>Browser, Platform, Device</td>
  </tr>
  <tr> 
   <td>Fai clic sul collegamento</td> 
   <td>Browser, Platform, Device</td>
  </tr>
 </tbody> 
</table>

**Attività basate su e-mail**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:30%">Attività</th> 
   <th style="width:70%">Attributi appena aggiunti</th>
  </tr>
   <tr> 
   <td>Invia e-mail</td> 
   <td>Browser, Platform, Device, Agente utente</td>
  </tr>
   </tr>
  <tr> 
   <td>E-mail consegnata</td> 
   <td>Browser, Platform, Device, Agente utente</td>
  </tr>
   <tr> 
   <td>E-mail non recapitata</td> 
   <td>Browser, Platform, Device, Agente utente</td>
  </tr>
  <tr> 
   <td>Annulla iscrizione e-mail</td> 
   <td>Browser, Platform, Device</td>
  </tr>
  <tr> 
   <td>Apri e-mail</td> 
   <td>Browser</td>
  </tr>
   <tr> 
   <td>Fai clic su E-mail</td> 
   <td>Browser</td>
  </tr>
  <tr> 
   <td>E-mail non recapitata temporaneamente</td> 
   <td>Browser, Platform, Device, Agente utente</td>
  </tr>
 </tbody> 
</table>
