---
description: Note sulla versione corrente - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione corrente
feature: Release Information
source-git-commit: 7ec3687c0c16738805394377b2080295c2f18032
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 4%

---

# Note sulla versione: aprile 2025 {#release-notes-apr-25}

Di seguito trovi tutte le funzioni incluse nella versione di aprile 2025. Verifica la disponibilità delle funzioni nella tua edizione di Adobe Marketo Engage.

Le note sulla versione specifiche per Adobe Dynamic Chat [ si trovano qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![stella](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzionalità rientrano nel ciclo di rilascio standard e inizieranno a essere rilasciate il **25 aprile 2025**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funzione</th> 
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
  <tr> 
   <td><strong>Compatibilità dei modelli per Designer e-mail</strong>: i modelli e-mail dall'editor e-mail classico sono ora compatibili con il nuovo <a href="/help/marketo/product-docs/email-marketing/email-designer/overview.md">Designer e-mail</a>.</td>
   <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>SSL (Secure Socket Layer) Self Service</strong>: la crittografia SSL consente di rendere sicure le pagine di destinazione per un'istanza di Marketo Engage. L’abilitazione di questa funzione veniva utilizzata per richiedere assistenza al team di supporto Adobe. Gli utenti di Marketo possono ora abilitarla da soli, risparmiando tempo prezioso.</td> 
   <td>Spedito</td>
   <td><a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/add-ssl-to-your-landing-pages.md">Aggiungere SSL alle pagine di destinazione</a></td>
  </tr>
 </tbody> 
</table>
<br/>

## Annunci {#announcements}

* **Nuova funzionalità di Analytics - Beta pubblico**: [Advanced BI Analytics](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (precedentemente nota come Revenue Explorer e Advanced Report Builder) inizia il rollout per tutti gli utenti correnti di Revenue Cycle Explorer a metà aprile. Questo nuovo strumento offre un’interfaccia flessibile per la generazione di rapporti e visualizzazioni sui dati di Marketo Engage, che fornisce dettagli granulari su progressione, prestazioni e altro ancora. Offre maggiore interattività e visualizzazione, prestazioni più veloci e un&#39;esperienza utente più fluida e intuitiva.

Per accedere a questa funzione, è necessario aver acquistato il componente aggiuntivo Advanced BI Analytics. Per ulteriori informazioni, contatta il team dell’account di Adobe (il tuo Account Manager).

* **Deprecazione parametro &#39;access_token&#39; API REST**: il parametro di query `access_token` utilizzato per autenticare le chiamate API REST di Marketo è obsoleto e non sarà disponibile dopo il 30 giugno 2025. Tutte le integrazioni nuove ed esistenti devono autenticare le chiamate API REST utilizzando l&#39;intestazione &#39;Authorization&#39;, [come descritto qui](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **API SOAP obsoleta**: il supporto per l&#39;API Marketo SOAP terminerà il 31 ottobre 2025. I servizi che utilizzano le funzionalità API di SOAP devono essere migrati all&#39;API [REST](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Funzionalità social obsolete**: mercoledì 31 luglio 2024, Marketo Engage ha iniziato a rendere obsolete le seguenti funzionalità social all&#39;interno del prodotto:

   * Sondaggi
   * Pulsante social
   * Offerta segnalata
   * Condividi video
   * Lotterie

Da allora, gli utenti non sono stati in grado di creare, clonare o incorporare nessuna di queste funzioni Social in Marketo Engage. Le risorse sociali esistenti continuano a funzionare fino al 31 gennaio 2025. Il 1° febbraio 2025 le attività social hanno cessato di funzionare. Tutte le funzioni social incorporate nelle pagine di destinazione dovranno essere rimosse. [Ulteriori informazioni](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}
