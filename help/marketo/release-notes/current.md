---
description: Note sulla versione corrente - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione corrente
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 77008ff8d8f7c577f48b508737e1b8eb2ac1e5ce
workflow-type: ht
source-wordcount: '653'
ht-degree: 100%

---

# Note sulla versione - Settembre 2025 {#release-notes-sep-25}

Di seguito sono disponibili tutte le funzioni incluse nella versione di settembre 2025. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

Le note sulla versione specifiche per Adobe Dynamic Chat [sono disponibili qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![star](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzioni rientrano nel ciclo di rilascio standard e inizieranno a essere rilasciate il **19 settembre 2025** con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funzione</th>
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
  <tr>
   <td><strong>Conservazione dell’attività webinar on-demand</strong>: gli utenti di webinar interattivi hanno ora a disposizione i dati della dashboard dei webinar on-demand per più di 30 giorni (in precedenza era solo fino a 30 giorni dal giorno del webinar).</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-mail designer - Flusso di lavoro di collaborazione sui contenuti</strong>: ora è possibile commentare e collaborare con gli altri utenti di Marketo all’interno di una risorsa e-mail. Assegnando tag ai membri del gruppo (utenti Marketo che dispongono delle autorizzazioni appropriate per la risorsa), questi riceveranno un’e-mail o una notifica Pulse.</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-mail designer - Autorizzazioni Assistente IA</strong>: gli amministratori di Marketo possono fornire a utenti specifici l’accesso alle funzioni GenAI.</td>
   <td>Implementato</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/ai-assistant.md#set-up-permissions">Configurare le autorizzazioni</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-mail Designer - Modalità scura</strong>: ora è possibile utilizzare la modalità scura, che consente ai client e-mail e alle app di supporto di visualizzare e-mail con sfondi più scuri e colori più chiari per testo, pulsanti e altri elementi dell’interfaccia utente.</td>
   <td>Implementato</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/dark-mode.md">Modalità scura</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-mail designer - Correzioni sul reindirizzamento</strong>: alcuni utenti riscontravano problemi di reindirizzamento con gli URL per le e-mail create tramite il nuovo Designer (ad esempio, incollare direttamente gli URL o aggiungere le risorse e-mail ai segnalibri non funzionava sempre come previsto). Questo problema è stato risolto. Inoltre, i collegamenti alle risorse e-mail da <b>Modelli e-mail</b> &gt; <b>Dettagli</b> &gt; <b>Utilizzati da</b> reindirizzeranno alla risorsa e-mail corrispondente.</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Annunci {#announcements}

* **Ripristino dello script Velocity nel nuovo E-mail designer**: lo scorso giugno, in Adobe Marketo Engage è stata rilasciata una funzione denominata _Contenuto condizionale_ per il nuovo E-mail designer. Tale funzione era basata su script Handlebar anziché Velocity, nel tentativo di offrire una maggiore flessibilità dei contenuti dinamici. Tuttavia, quando è stato rilevato che causava la risoluzione errata di alcuni token, è stato deciso di disabilitarla temporaneamente. [Ulteriori informazioni](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Fine del ciclo di vita di Marketo Engage Identity**: ad agosto 2025, Adobe inizierà a eliminare gradualmente il supporto per Marketo Engage Identity (accesso tramite `login.marketo.com`). Per evitare l’interruzione dell’accesso a Marketo Engage, devi passare a [Adobe Identity](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} entro il 30 settembre 2025.

   * _Deprecazione limitazioni IP_: il supporto per [Limitazione degli accessi a Marketo basati su IP](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} è terminato il 30 luglio 2025. La funzione rimarrà operativa fino al completamento della transizione ad Adobe Identity. A breve sarà disponibile una nuova funzione di controllo degli accessi basata sulla posizione per Adobe Identity in Adobe Admin Console.

   * _Deprecazione single sign-on (SSO)_: il supporto per [Marketo Identity SSO](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} è terminato il 30 luglio 2025. La funzione rimarrà operativa fino al completamento della transizione ad Adobe Identity. Il Single Sign-On per Adobe Identity in Adobe Admin Console deve essere configurato separatamente. Per i passaggi di configurazione, vedi [Configurare identità e Single Sign-On](https://helpx.adobe.com/it/enterprise/using/set-up-identity.html){target="_blank"}.

* **Deprecazione della funzionalità _Inoltra a un amico_**: il 29 settembre 2025 la funzionalità _Inoltra a un amico_ nelle e-mail di Marketo Engage 2.0 (l’editor e-mail precedente) diventerà completamente obsoleta per tutti gli abbonamenti. Questo influisce sul token “Inoltra a un amico” e sui collegamenti “Inoltra a un amico” nelle e-mail che sono già state o saranno inviate utilizzando il token. [Ulteriori informazioni](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Deprecazione parametro &#39;access_token&#39; API Rest**: il parametro di query `access_token` utilizzato per autenticare le chiamate API REST di Marketo è obsoleto e non sarà più disponibile dopo il 31 gennaio 2026. Tutte le integrazioni nuove ed esistenti devono autenticare le chiamate API REST utilizzando l’intestazione &#39;Authorization&#39;, [come descritto qui](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Deprecazione API SOAP**: il supporto per l’API SOAP di Marketo terminerà il 31 gennaio 2026. I servizi che utilizzano le funzionalità API SOAP devono effettuare la migrazione all’[API REST](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
