---
description: Note sulla versione - Aprile 2024 - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione - Aprile 2024
feature: Release Information
exl-id: d87474f8-fc47-407b-bc97-e343b56c1f8f
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 3%

---

# Note sulla versione: aprile 2024 {#release-notes-apr-24}

Di seguito sono riportate tutte le funzioni incluse nella versione di aprile 2024. Verifica la disponibilità delle funzioni nella tua edizione di Adobe Marketo Engage.

Le note sulla versione specifiche per Adobe Dynamic Chat [ si trovano qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![stella](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzionalità rientrano nel ciclo di rilascio standard e inizieranno a essere rilasciate il **26 aprile 2024**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Funzione</th>
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
     <tr>
   <td><strong>Miglioramenti ai webinar interattivi</strong>: è ora possibile consentire a host e relatori di aggiungere un titolo al webinar, rinominare una room e sincronizzare manualmente i dati di coinvolgimento dopo la consegna dell'evento.</td>
   <td>Spedito</td>
   <td><li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/create-an-interactive-webinar.md">Creare un webinar interattivo</a></li>
   <li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/event-workflows.md#manual-sync">Sincronizzazione manuale</a></li></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>Miglioramenti Audit Trail</strong>:
   È ora possibile acquisire nuovi tipi di azioni in Audit Trail per le modifiche apportate in Gestione campi, per le modifiche apportate a Utenti e ruoli e per il numero di persone esportate da elenchi ed elenchi avanzati.</td>
   <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>Autorizzazioni nuovi utenti e ruoli</strong>: sono disponibili nuove autorizzazioni che forniscono agli utenti un accesso più granulare a Marketo Engage. Controlla le parti dell’amministratore non gestite in precedenza, ad esempio Nuova esperienza e Predictive Audiences, divide le autorizzazioni per concedere separatamente l’accesso all’Asset Audit Trail e all’Admin Audit Trail e utilizza le nuove autorizzazioni di creazione e spostamento per le risorse e le cartelle per impedire che gli utenti di sola lettura apportino modifiche.
   <p>Le nuove autorizzazioni appariranno nell’istanza di Marketo Engage a partire dal 26 aprile, ma per il momento sono passive e diventeranno accessibili più avanti nel corso del trimestre.
   <li>Accedere a Adobe Experience Manager</li>
   <li>Accedere ad Adobe Organization Mapping</li>
   <li>Accedi ad Admin Audit Trail</li>
   <li>Accedere ad Asset Audit Trail</li>
   <li>Accedi a nuova esperienza</li>
   <li>Accedere a Predictive Audiences</li>
   <li>Crea rapporto</li>
   <li>Crea elenco</li>
   <li>Esporta attività campagna</li>
   </td>
   <td>Spedito</td>
   <td><a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md">Descrizioni delle autorizzazioni per il ruolo</a></td>
  </tr>
 </tbody>
</table>
<br/>

## Annunci {#announcements}

* **Aggiornamento API attività**: il 26 aprile verranno aggiunti diversi nuovi attributi alle attività basate su Web e posta elettronica restituiti quando si recuperano attività tramite l&#39;API REST [Marketo](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities){target="_blank"}. Le attività elencate di seguito ora includono gli attributi Browser, Platform, Device e User Agent. Chiamare l&#39;endpoint [Get Activity Types](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities/operation/getAllActivityTypesUsingGET){target="_blank"} per rivedere i dettagli degli attributi di ogni attività.

**Attività basate sul Web**

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
   <td>Fai clic sull’e-mail</td>
   <td>Browser</td>
  </tr>
  <tr>
   <td>E-mail non recapitata temporaneamente</td>
   <td>Browser, Platform, Device, Agente utente</td>
  </tr>
 </tbody>
</table>
