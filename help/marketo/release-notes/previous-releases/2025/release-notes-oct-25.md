---
description: Note sulla versione - Ottobre 2025 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Ottobre 2025
feature: Release Information
exl-id: 9c668de0-14d0-4d2e-8ea6-dc7db5be3ea7
source-git-commit: 6b8733e8b67ef9f93ba16cd1589de93fe45ceb25
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 93%

---

# Note sulla versione - Ottobre 2025 {#release-notes-oct-25}

Di seguito sono riportate tutte le funzioni incluse nella versione di ottobre 2025. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

Le note sulla versione specifiche per Adobe Dynamic Chat [sono disponibili qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![star](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzioni rientrano nel ciclo di rilascio standard. Inizieranno a essere rilasciate il **31 ottobre 2025**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funzione</th>
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
  <tr>
   <td><strong>E-mail designer - Importazione modelli (Beta)</strong>: importa i modelli e-mail dall’editor e-mail classico per creare modelli compatibili con il nuovo E-mail designer in Design Studio.</td>
   <td>Rilasciato</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/import-template.md" target="_blank">Importazione di modelli</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-mail designer - Temi brand</strong>: ora puoi definire i temi del brand in Marketo Engage. Le configurazioni di stile possono essere riutilizzate e applicate ai modelli per e-mail e ad altre risorse e-mail al fine di mantenere la coerenza del brand.</td>
   <td>Rilasciato</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/brand-themes.md" target="_blank">Temi del brand</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-mail designer - Contenuto condizionale</strong>: funzione di parità per il nuovo E-mail designer, che estende la personalizzazione delle e-mail oltre l’utilizzo dei token.</td>
   <td>Rilasciato</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/conditional-content.md" target="_blank">Contenuti condizionali</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
 <tr>
   <td><strong>E-mail designer - Convertitore da immagine a HTML</strong>: carica un file immagine PNG/JPEG conforme di un’e-mail che verrà automaticamente convertito in HTML da utilizzare nel nuovo E-mail designer.</td>
   <td>Rilasciato</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/image-to-html.md" target="_blank">Convertire immagini in modelli HTML</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-mail designer - Azione Clona e-mail</strong>: ora puoi clonare un’e-mail in un’altra cartella di programmi nelle attività di marketing e riutilizzare rapidamente le e-mail esistenti.</td>
   <td>Rilasciato</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-mail designer - Test A/B</strong>: funzione di parità per il nuovo E-mail designer, che consente di eseguire test A/B per individuare i tipi di contenuto da cui è possibile ottenere risultati di risposta migliori.</td>
   <td>Rilasciato</td>
   <td>n/d</td>
  </tr>
  </tbody>
</table>
<br/>

## Annunci {#announcements}

* **Aggiornamento dell’integrazione CRM Salesforce**: una nuova versione dell’integrazione CRM nativa verrà implementata nelle sandbox attive in cui è abilitato il connettore nativo. L’implementazione avverrà a partire dal 13 novembre 2025, e sarà completata entro sette giorni. Ottieni dettagli completi in [questo post community](https://nation.marketo.com/t5/product-blogs/salesforce-crm-integration-upgrade/ba-p/358702){target="_blank"}

* **Deprecazione della doppia barra nell’API REST**: il 16 settembre 2025 Adobe è passato a un’infrastruttura di hosting più moderna per gli URL delle API REST che sfrutta la tecnologia più recente, aggiungendo sicurezza e scalabilità. Se il tuo abbonamento utilizza API con una doppia barra (//) nell&#39;URL, leggi [questo post della community](https://nation.marketo.com/t5/product-blogs/rest-api-double-slash-deprecation/ba-p/358616){target="_blank"} per i passaggi successivi.

* **Ripristino dello script Velocity nel nuovo E-mail designer**: lo scorso giugno, in Adobe Marketo Engage è stata rilasciata una funzione denominata _Contenuto condizionale_ per il nuovo E-mail designer. Tale funzione era basata su script Handlebar anziché Velocity, nel tentativo di offrire una maggiore flessibilità dei contenuti dinamici. Tuttavia, quando è stato rilevato che causava la risoluzione errata di alcuni token, è stato deciso di disabilitarla temporaneamente. [Ulteriori informazioni](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Fine del ciclo di vita di Marketo Engage Identity**: ad agosto 2025, Adobe inizierà a eliminare gradualmente il supporto per Marketo Engage Identity (accesso tramite `login.marketo.com`). Per evitare l’interruzione dell’accesso a Marketo Engage, devi passare a [Adobe Identity](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} entro il 30 settembre 2025.

   * _Deprecazione limitazioni IP_: il supporto per [Limitazione degli accessi a Marketo basati su IP](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} è terminato il 30 luglio 2025. La funzione rimarrà operativa fino al completamento della transizione ad Adobe Identity. A breve sarà disponibile una nuova funzione di controllo degli accessi basata sulla posizione per Adobe Identity in Adobe Admin Console.

   * _Deprecazione single sign-on (SSO)_: il supporto per [Marketo Identity SSO](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} è terminato il 30 luglio 2025. La funzione rimarrà operativa fino al completamento della transizione ad Adobe Identity. Il Single Sign-On per Adobe Identity in Adobe Admin Console deve essere configurato separatamente. Per i passaggi di configurazione, vedi [Configurare identità e Single Sign-On](https://helpx.adobe.com/it/enterprise/using/set-up-identity.html){target="_blank"}.

* **Rimozione della funzione _Inoltra a un amico_**: il 29 settembre 2025 la funzione _Inoltra a un amico_ nelle e-mail di Marketo Engage 2.0 (l’editor e-mail precedente) diventerà obsoleta e verrà rimossa per tutti gli abbonamenti. Questo influisce sul token “Inoltra a un amico” e sui collegamenti “Inoltra a un amico” nelle e-mail che sono già state inviate o che erano pianificate per l’invio tramite token. [Ulteriori informazioni](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Parametro “access_token” API Rest obsoleto**: il parametro di query `access_token` utilizzato per autenticare le chiamate API REST di Marketo è ora obsoleto e non sarà più disponibile dopo il 31 marzo 2026. Tutte le integrazioni nuove ed esistenti devono autenticare le chiamate API REST utilizzando l’intestazione “Authorization”, [come descritto qui](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **API SOAP obsolete**: il supporto per le API SOAP di Marketo terminerà il 31 marzo 2026. I servizi che utilizzano le funzionalità API SOAP devono essere migrati alle [API REST](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
