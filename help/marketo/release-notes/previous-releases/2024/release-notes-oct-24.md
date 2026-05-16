---
description: Note sulla versione - Ottobre 2024 - Documentazione di Marketo - Documentazione del prodotto
title: Note sulla versione - Ottobre 2024
feature: Release Information
exl-id: 2e28ae7f-51de-4510-b3e8-79a989f0daf5
TQID: https://experienceleague.adobe.com/3Qk4bF8OVxVoJYZbtedik6vRsAebYvj-ZMOfxXuzDMk
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
  - id: efc9a24a-a6a4-449d-a3e6-44f6c74dfd46
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 575
ht-degree: 20%

---

# Note sulla versione - Ottobre 2024 {#release-notes-oct-24}

Qui sotto troverai tutte le funzioni incluse nella versione di ottobre 2024. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

Le note sulla versione specifiche per Adobe Dynamic Chat [sono disponibili qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![star](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzioni rientrano nel ciclo di rilascio standard. Inizieranno a essere rilasciate il **sabato 4 ottobre 2024**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Funzione</th>
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
    <tr>
   <td><strong>Tokenization for Interactive Webinars</strong>: ora puoi utilizzare i token per promuovere i webinar interattivi nelle e-mail e nelle pagine di destinazione senza dover aggiungere manualmente i dettagli del webinar.</td>
   <td>Rilasciato</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/promoting-an-interactive-webinar.md#interactive-webinars-tokens" target="_blank">Promozione di un webinar interattivo</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   <tr>
   <td><strong>Conteggio "Influenza" elenco smart</strong>: verifica il numero di persone interessate dalla modifica delle regole di qualifica di una campagna smart.</td>
   <td>Rilasciato</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   <tr>
   <td><strong>Pulsante Account personale nella barra di navigazione</strong>: per coloro che hanno eseguito la migrazione ad Adobe Identity Management System, un nuovo pulsante "Account personale" nella barra di navigazione a sinistra consente di configurare il fuso orario e di accedere ai dettagli dell'abbonamento.</td>
   <td>Rilasciato</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
   <tr>
   <td><strong>Miglioramenti al report delle prestazioni delle e-mail</strong>: sono stati apportati diversi miglioramenti alle metriche di reporting e al tracciamento delle attività e-mail, offrendo ulteriori informazioni e migliorando la precisione.
   <ul>
   <li>Filtrare le persone eliminate e unite dalle metriche delle prestazioni delle e-mail</li>
   <li>Le e-mail sono ora classificate come <i>interrotte</i> dopo tre giorni di attesa per l'attività di risposta</li>
   <li>Le aperture delle e-mail contano come aperture univoche separatamente per ogni Smart Campaign</li>
   </td>
   <td>Rilasciato</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md" target="_blank">Rapporto prestazioni e-mail</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
   <tr>
   <td><strong>Metriche backlog sincronizzazione Salesforce</strong>: monitorare le tendenze della velocità effettiva e del backlog di sincronizzazione per pianificare e pianificare gli aggiornamenti CRM per un'esperienza di sincronizzazione ottimale.
   </td>
   <td>Rilasciato</td>
   <td><a href="/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-backlog-metrics.md" target="_blank">Metriche backlog della sincronizzazione Salesforce</a></td>
  </tr>
 </tbody>
</table>
<br/>

## Annunci {#announcements}

* **Aggiornamento API per estrazione in blocco**: è stato risolto un problema nell&#39;API per estrazione in blocco che interessava l&#39;opzione columnHeaderNames, che consente di specificare nomi di intestazione di colonna personalizzati nel file esportato. In precedenza, i nomi delle intestazioni di colonna contenenti caratteri non ASCII potevano danneggiarsi.

* **Parametro access_token API REST obsoleto**: il parametro di query &#39;access_token&#39; utilizzato per autenticare le chiamate API REST di Marketo è obsoleto e non sarà disponibile dopo il 31 marzo 2026. Tutte le integrazioni nuove ed esistenti devono autenticare le chiamate API REST utilizzando l&#39;intestazione &#39;Authorization&#39; [come descritto qui](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication#using-an-access-token).

* **Deprecazione del codice QR**: il 4 ottobre 2024 la funzione del codice QR utilizzata nelle notifiche push e nelle risorse di messaggistica in-app diventerà obsoleta. Ciò include l&#39;utilizzo di codici QR per un nuovo dispositivo di test e la creazione di nuove risorse con codici QR. Le funzioni obsolete con un utilizzo inferiore ci consentono di riallocare le loro risorse alla manutenzione complessiva di Marketo Engage.

* **Modifiche Munchkin**

   * **Nuova versione**: il 17 settembre 2024, [Munchkin](/help/marketo/product-docs/administration/setup-administration/munchkin.md){target="_blank"} v.164 inizierà il rollout nelle istanze di Marketo Engage in cui l&#39;impostazione &quot;Munchkin Beta&quot; è abilitata in **Admin** > **Treasure Chest**. È pianificato per iniziare il rollout per tutte le altre istanze il 29 ottobre. Questa versione aggiorna la creazione dei cookie di Munchkin. Nessuna modifica nelle funzionalità.

   * **Caratteri rimossi dall&#39;URL**: le attività &#39;Pagina Web visite&#39; e &#39;Collegamento clic&#39; create da Munchkin JS ora rimuoveranno i caratteri di controllo non codificati dall&#39;URL da tutti i campi URL. Questa modifica è stata progettata per evitare errori relativi alla propagazione di questi tipi di caratteri in sistemi che non li supportano e che non sono utilizzati in modo valido in Marketo Engage.
