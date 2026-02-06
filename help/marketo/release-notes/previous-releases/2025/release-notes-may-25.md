---
description: Note sulla versione - Maggio 2025 - Documentazione di Marketo - Documentazione del prodotto
title: Note sulla versione - Maggio 2025
feature: Release Information
exl-id: 99cd1d54-0a80-40fa-9d0c-1cb437be90f0
source-git-commit: 8e72b24e18ae108ec74e6d4fa6b04f10130439a4
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 40%

---

# Note sulla versione - Maggio 2025 {#release-notes-may-25}

Di seguito sono elencate tutte le funzioni incluse nella versione di maggio 2025. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

Le note sulla versione specifiche per Adobe Dynamic Chat [sono disponibili qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![star](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzioni rientrano nel ciclo di rilascio standard. Inizieranno a essere rilasciate il **sabato 23 maggio 2025**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funzione</th>
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
  <tr>
   <td><strong>Controllo degli accessi basato sul ruolo per e-mail Designer Assets</strong>: un nuovo miglioramento al sistema di controllo degli accessi basato sul ruolo (RBAC) fornisce autorizzazioni più granulari e una migliore gestione degli utenti per le risorse basate sul nuovo Designer e-mail.</td>
   <td>Rilasciato</td>
   <td><a href="https://nation.marketo.com/t5/latest-product-innovations/product-updates-granular-permissions-to-new-email-designer/ba-p/357057">Autorizzazioni granulari per New Email Designer (post di blog)</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Clonazione di e-mail create nel Designer di posta elettronica</strong>: ora puoi clonare un'e-mail esistente creata con il nuovo Designer di posta elettronica.</td>
   <td>Rilasciato</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Token di attivazione per qualsiasi attributo</strong>: elenco esteso di token di attivazione per il supporto dell'utilizzo dei dati di qualsiasi attributo di attività nei campi di Smart Campaign.</td>
   <td>Rilasciato</td>
   <td>n/d</td>
  </tr>
 </tbody>
</table>
<br/>

## Annunci {#announcements}

* **Aggiornamento dell&#39;integrazione della conversione offline di Facebook**: il 29 maggio 2025, l&#39;integrazione [Conversione offline di Facebook](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions){target="_blank"} per Marketo Engage verrà migrata alla nuova API [Conversioni](https://developers.facebook.com/docs/marketing-api/conversions-api){target="_blank"} di Meta, a causa della deprecazione di Meta dell&#39;API [Conversioni offline](https://developers.facebook.com/docs/marketing-api/offline-conversions/){target="_blank"} in linea con il controllo delle versioni dell&#39;API Graph. Per ulteriori informazioni, vedere la guida di Meta per [l&#39;invio di eventi offline tramite Conversions API](https://developers.facebook.com/docs/marketing-api/conversions-api/offline-events/){target="_blank"} (CAPI per offline).

* **Nuova funzionalità di Analytics - Beta pubblico**: [Advanced BI Analytics](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (precedentemente nota come Revenue Explorer e Advanced Report Builder) ha iniziato a essere implementato per tutti gli utenti attuali di Revenue Cycle Explorer a metà aprile. Questo nuovo strumento offre un’interfaccia flessibile per la generazione di rapporti e visualizzazioni sui dati di Marketo Engage, che fornisce dettagli granulari su progressione, prestazioni e altro ancora. Offre maggiore interattività e visualizzazione, prestazioni più veloci e un&#39;esperienza utente più fluida e intuitiva.

Per accedere a questa funzione, è necessario aver acquistato il componente aggiuntivo Advanced BI Analytics. Per ulteriori informazioni, contatta il team dell’account di Adobe (il tuo Account Manager).

* **Deprecazione parametro &#39;access_token&#39; API Rest**: il parametro di query `access_token` utilizzato per autenticare le chiamate API REST di Marketo è obsoleto e non sarà più disponibile dopo il mercoledì 31 marzo 2026. Tutte le integrazioni nuove ed esistenti devono autenticare le chiamate API REST utilizzando l’intestazione “Authorization”, [come descritto qui](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **API SOAP obsolete**: il supporto per le API SOAP di Marketo terminerà il 31 marzo 2026. I servizi che utilizzano le funzionalità API SOAP devono essere migrati alle [API REST](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
