---
description: Note sulla versione corrente - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione corrente
hide: true
hidefromtoc: true
feature: Release Information
source-git-commit: 7ec3687c0c16738805394377b2080295c2f18032
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 2%

---

# Note sulla versione: maggio 2025 {#release-notes-may-25}

Di seguito sono elencate tutte le funzioni incluse nella versione di maggio 2025. Verifica la disponibilità delle funzioni nella tua edizione di Adobe Marketo Engage.

Le note sulla versione specifiche per Adobe Dynamic Chat [ si trovano qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![stella](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzionalità rientrano nel ciclo di rilascio standard e inizieranno a essere rilasciate il **23 maggio 2025**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto"> 
 <tbody>
  <tr> 
   <td><strong>Token del trigger per qualsiasi attributo</strong>: elenco esteso di token del trigger per supportare l'utilizzo dei dati di qualsiasi attributo di attività nei campi di Smart Campaign.</td> 
   <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Annunci {#announcements}

* **Nuova funzionalità di Analytics - Beta pubblico**: [Advanced BI Analytics](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (precedentemente nota come Revenue Explorer e Advanced Report Builder) ha iniziato a essere implementato per tutti gli utenti attuali di Revenue Cycle Explorer a metà aprile. Questo nuovo strumento offre un’interfaccia flessibile per la generazione di rapporti e visualizzazioni sui dati di Marketo Engage, che fornisce dettagli granulari su progressione, prestazioni e altro ancora. Offre maggiore interattività e visualizzazione, prestazioni più veloci e un&#39;esperienza utente più fluida e intuitiva.

Per accedere a questa funzione, è necessario aver acquistato il componente aggiuntivo Advanced BI Analytics. Per ulteriori informazioni, contatta il team dell’account di Adobe (il tuo Account Manager).

* **Deprecazione parametro &#39;access_token&#39; API REST**: il parametro di query `access_token` utilizzato per autenticare le chiamate API REST di Marketo è obsoleto e non sarà disponibile dopo il 30 giugno 2025. Tutte le integrazioni nuove ed esistenti devono autenticare le chiamate API REST utilizzando l&#39;intestazione &#39;Authorization&#39;, [come descritto qui](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **API SOAP obsoleta**: il supporto per l&#39;API Marketo SOAP terminerà il 31 ottobre 2025. I servizi che utilizzano le funzionalità API di SOAP devono essere migrati all&#39;API [REST](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
