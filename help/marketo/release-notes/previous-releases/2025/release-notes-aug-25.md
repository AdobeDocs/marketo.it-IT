---
description: Note sulla versione - Agosto 2025 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Agosto 2025
feature: Release Information
exl-id: f4f71a77-d0c0-41c3-9362-afbfb467cc7a
TQID: https://experienceleague.adobe.com/Tt3KgAUlQd8oBN2KV-dFUQdEPmlZ-3tOzQ8T-EaCTfI
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: ea90ebee-5c84-42d9-8b21-006bdabc95a3id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bccid: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2: id: c942e9f6-ed06-481a-abdd-1195363d1452
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: cdd65e7e-8839-44a2-bc21-0e03623b5dd1id: e0eb8757-182f-49f3-94a4-1587d16f5094id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 680
ht-degree: 98%

---

# Note sulla versione - Agosto 2025 {#release-notes-aug-25}

Di seguito sono disponibili tutte le funzioni incluse nella versione di agosto 2025. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

Le note sulla versione specifiche per Adobe Dynamic Chat [sono disponibili qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![star](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzionalità rientrano nel ciclo di rilascio standard e inizieranno a essere rilasciate il giorno **22 agosto 2025** con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funzione</th>
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
  <tr>
   <td><strong>E-mail designer - Reporting</strong>: i rapporti sulle prestazioni dei collegamenti e-mail e sulle prestazioni delle e-mail ora mostrano i dati delle e-mail create utilizzando il nuovo E-mail designer.</td>
   <td>Rilasciato</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-mail designer - Rimozione completamento automatico</strong>: l’opzione completamento automatico nell’editor di personalizzazione dei token indicava oggetti errati ed è stata rimossa. Al momento non ne è prevista la reimplementazione.</td>
   <td>Rilasciato</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-mail designer - Ottimizzazione anteprima e-mail</strong>: alcuni utenti hanno riscontrato tempi di caricamento più lenti durante il tentativo di visualizzare l’anteprima del messaggio e-mail nella pagina dei dettagli dell’e-mail, del modello e del frammento. Questa esperienza è stata ottimizzata per tempi di caricamento fino al 60% più rapidi.</td>
   <td>Rilasciato</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-mail designer - Correzioni di modelli</strong>: alcuni modelli preconfigurati presentavano problemi di rendering (ad esempio, rendering non corretto in alcuni browser/modalità scura, immagini non allineate, pulsanti di CTA posizionati in modo errato e altri). In questa versione tali problemi sono stati risolti.</td>
   <td>Rilasciato</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-mail designer - Correzione blocco contenuto</strong>: in precedenza, se veniva creato un modello di e-mail con blocco del contenuto e il modello veniva utilizzato per creare un’e-mail, il blocco del contenuto persisteva anche quando l’e-mail veniva reimpostata o veniva selezionato “modifica progettazione”. In questa versione tale problema è stato risolto.</td>
   <td>Rilasciato</td>
   <td>n/d</td>
  </tr>
  </tbody>
</table>
<br/>

## Annunci {#announcements}

* **Fine del ciclo di vita di Marketo Engage Identity**: ad agosto 2025, Adobe inizierà a eliminare gradualmente il supporto per Marketo Engage Identity (accesso tramite `login.marketo.com`). Per evitare l’interruzione dell’accesso a Marketo Engage, devi passare a [Adobe Identity](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} entro il 30 settembre 2025.

   * _Deprecazione limitazioni IP_: il supporto per [Limitazione degli accessi a Marketo basati su IP](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} è terminato il 30 luglio 2025. La funzione rimarrà operativa fino al completamento della transizione ad Adobe Identity. A breve sarà disponibile una nuova funzione di controllo degli accessi basata sulla posizione per Adobe Identity in Adobe Admin Console.

   * _Deprecazione single sign-on (SSO)_: il supporto per [Marketo Identity SSO](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} è terminato il 30 luglio 2025. La funzione rimarrà operativa fino al completamento della transizione ad Adobe Identity. Il Single Sign-On per Adobe Identity in Adobe Admin Console deve essere configurato separatamente. Per i passaggi di configurazione, vedi [Configurare identità e Single Sign-On](https://helpx.adobe.com/it/enterprise/using/set-up-identity.html){target="_blank"}.

* **Deprecazione della funzionalità _Inoltra a un amico_**: il 29 settembre 2025 la funzionalità _Inoltra a un amico_ nelle e-mail di Marketo Engage 2.0 (l’editor e-mail precedente) diventerà completamente obsoleta per tutti gli abbonamenti. Questo influisce sul token “Inoltra a un amico” e sui collegamenti “Inoltra a un amico” nelle e-mail che sono già state o saranno inviate utilizzando il token. [Ulteriori informazioni](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Parametro “access_token” API Rest obsoleto**: il parametro di query `access_token` utilizzato per autenticare le chiamate API REST di Marketo è ora obsoleto e non sarà più disponibile dopo il 31 marzo 2026. Tutte le integrazioni nuove ed esistenti devono autenticare le chiamate API REST utilizzando l’intestazione “Authorization”, [come descritto qui](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **API SOAP obsolete**: il supporto per le API SOAP di Marketo terminerà il 31 marzo 2026. I servizi che utilizzano le funzionalità API SOAP devono essere migrati alle [API REST](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
