---
description: Note sulla versione corrente - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione corrente
hide: true
hidefromtoc: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
source-git-commit: 29c1b59c9d2598626f546554a8bdc1b26b9e1590
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 51%

---

# Note sulla versione - Settembre 2025 {#release-notes-sep-25}

Di seguito sono elencate tutte le funzioni incluse nella versione di settembre 2025. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

Le note sulla versione specifiche per Adobe Dynamic Chat [sono disponibili qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![star](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzionalità rientrano nel ciclo di rilascio standard e inizieranno a essere rilasciate il giorno **sabato 19 settembre 2025** con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funzione</th>
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
  <tr>
   <td><strong>Conservazione attività webinar on demand</strong>: gli utenti di webinar interattivi ora dispongono di dati del dashboard webinar on demand disponibili per più di 30 giorni (in precedenza era solo fino a 30 giorni dal giorno del webinar).</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Annunci {#announcements}

* **Ripristino dello script Velocity nel nuovo Designer e-mail**: Adobe Marketo Engage ha rilasciato una funzionalità denominata _Contenuto condizionale_ per il nuovo Designer e-mail lo scorso giugno. La funzione si basa su script Handlebar anziché Velocity, nel tentativo di fornire un po’ più di flessibilità nel contenuto dinamico. Ma quando abbiamo scoperto che causava la risoluzione errata di alcuni token, abbiamo deciso di disattivarlo temporaneamente. [Ulteriori informazioni](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Fine del ciclo di vita di Marketo Engage Identity**: ad agosto 2025, Adobe ha iniziato a eliminare gradualmente il supporto per Marketo Engage Identity (accesso tramite `login.marketo.com`). Per evitare l&#39;interruzione dell&#39;accesso a Marketo Engage, devi passare a [Adobe Identity](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} entro il 30 settembre 2025.

   * _Deprecazione restrizioni IP_: supporto per [Limitazione degli accessi a Marketo in base all&#39;IP](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} terminato il 30 luglio 2025. La funzione rimarrà operativa fino al completamento della transizione ad Adobe Identity. Presto sarà disponibile una nuova funzione di controllo degli accessi basati sulla posizione per Adobe Identity in Adobe Admin Console.

   * _Obsolescenza Single Sign-On (SSO)_: supporto per [Marketo Identity SSO](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} terminato il 30 luglio 2025. La funzione rimarrà operativa fino al completamento della transizione ad Adobe Identity. Il Single Sign-On per Adobe Identity in Adobe Admin Console deve essere configurato separatamente. Per i passaggi di configurazione, vedi [Configurare identità e Single Sign-On](https://helpx.adobe.com/it/enterprise/using/set-up-identity.html){target="_blank"}.

* **Obsolescenza di _Inoltra a un amico_ funzionalità**: il 29 settembre 2025 la funzionalità _Inoltra a un amico_ nelle e-mail di Marketo Engage 2.0 (l&#39;editor e-mail legacy) diventerà completamente obsoleta per tutti gli abbonamenti. Questo influisce sul token &quot;Inoltra a un amico&quot; e sui collegamenti &quot;Inoltra a un amico&quot; nelle e-mail che sono già state o saranno inviate utilizzando il token. [Ulteriori informazioni](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Deprecazione parametro &#39;access_token&#39; API Rest**: il parametro di query `access_token` utilizzato per autenticare le chiamate API REST di Marketo è obsoleto e non sarà disponibile dopo il 31 ottobre 2025. Tutte le integrazioni nuove ed esistenti devono autenticare le chiamate API REST utilizzando l&#39;intestazione &#39;Authorization&#39;, [come descritto qui](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Deprecazione API SOAP**: il supporto per l&#39;API SOAP di Marketo terminerà il 31 ottobre 2025. I servizi che utilizzano le funzionalità API SOAP devono essere migrati all&#39;[API REST](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
