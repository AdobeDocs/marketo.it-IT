---
description: Note sulla versione corrente - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione corrente
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 6da797bc91de018e789f1e5980523a02e38eba30
workflow-type: tm+mt
source-wordcount: '517'
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
   <th style="width:65%">Funzione</th> 
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
  <tr> 
   <td><strong>Contenuto e-mail Personalization</strong>: Marketo Engage ora segue la stessa sintassi delle maiuscole/minuscole degli altri token dell'applicazione AEP, in modo da fornire un'esperienza coerente tra i prodotti Adobe DX. Tutti i token standard e i token specifici di Marketo Engage come Membro, Programma e I miei token sono disponibili nel nuovo Designer e-mail.</td> 
   <td>Spedito</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/personalization-tokens.md">Token Personalization</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Controllo degli accessi basato sul ruolo per e-mail Designer Assets</strong>: un nuovo miglioramento al sistema di controllo degli accessi basato sul ruolo (RBAC) fornisce autorizzazioni più granulari e una migliore gestione degli utenti per le risorse basate sul nuovo Designer e-mail.</td> 
   <td>Spedito</td>
   <td><a href="https://nation.marketo.com/t5/latest-product-innovations/product-updates-granular-permissions-to-new-email-designer/ba-p/357057">Autorizzazioni granulari per New Email Designer (post di blog)</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Clonazione di e-mail create nel Designer di posta elettronica</strong>: ora puoi clonare un'e-mail esistente creata con il nuovo Designer di posta elettronica.</td> 
   <td>Spedito</td>
   <td>n/d</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Integrazione di GenStudio nel Designer e-mail</strong>: integra GenStudio per il marketing delle prestazioni dalle e-mail per migliorare l'efficienza del marketing e mantenere la coerenza del brand.</td> 
   <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Token di attivazione per qualsiasi attributo</strong>: elenco esteso di token di attivazione per il supporto dell'utilizzo dei dati di qualsiasi attributo di attività nei campi di Smart Campaign.</td> 
   <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Annunci {#announcements}

* **Aggiornamento dell&#39;integrazione della conversione offline di Facebook**: il 29 maggio 2025 verrà effettuata la migrazione dell&#39;integrazione della [conversione offline di Facebook](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions){target="_blank"} per Marketo Engage alla nuova Meta [API delle conversioni](https://developers.facebook.com/docs/marketing-api/conversions-api){target="_blank"}, a causa della rimozione da parte di Meta della [API delle conversioni offline](https://developers.facebook.com/docs/marketing-api/offline-conversions/){target="_blank"} in linea con il controllo delle versioni dell&#39;API grafica. Per ulteriori informazioni, vedere la guida di Meta per [l&#39;invio di eventi offline tramite Conversions API](https://developers.facebook.com/docs/marketing-api/conversions-api/offline-events/){target="_blank"} (CAPI per offline).

* **Nuova funzionalità di Analytics - Beta pubblico**: [Advanced BI Analytics](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (precedentemente nota come Revenue Explorer e Advanced Report Builder) ha iniziato a essere implementato per tutti gli utenti attuali di Revenue Cycle Explorer a metà aprile. Questo nuovo strumento offre un’interfaccia flessibile per la generazione di rapporti e visualizzazioni sui dati di Marketo Engage, che fornisce dettagli granulari su progressione, prestazioni e altro ancora. Offre maggiore interattività e visualizzazione, prestazioni più veloci e un&#39;esperienza utente più fluida e intuitiva.

Per accedere a questa funzione, è necessario aver acquistato il componente aggiuntivo Advanced BI Analytics. Per ulteriori informazioni, contatta il team dell’account di Adobe (il tuo Account Manager).

* **Deprecazione parametro &#39;access_token&#39; API REST**: il parametro di query `access_token` utilizzato per autenticare le chiamate API REST di Marketo è obsoleto e non sarà disponibile dopo il 31 ottobre 2025. Tutte le integrazioni nuove ed esistenti devono autenticare le chiamate API REST utilizzando l&#39;intestazione &#39;Authorization&#39;, [come descritto qui](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **API SOAP obsoleta**: il supporto per l&#39;API Marketo SOAP terminerà il 31 ottobre 2025. I servizi che utilizzano le funzionalità API di SOAP devono essere migrati all&#39;API [REST](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
