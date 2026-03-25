---
description: Note sulla versione - Febbraio 2026 - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione - Febbraio 2026
feature: Release Information
exl-id: 679d2fca-99ba-4321-ad0d-a297b7f193fc
source-git-commit: 70939d387dcfe6064e179e4e7e91b16c6baa7b8b
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 41%

---

# Note sulla versione - Febbraio 2026 {#release-notes-feb-26}

Qui sotto troverai tutte le funzioni incluse nella versione di febbraio 2026. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

Le note sulla versione specifiche per Adobe Dynamic Chat [sono disponibili qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzioni rientrano nel ciclo di rilascio standard. Inizieranno a essere rilasciate il **sabato 20 febbraio 2026**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funzione</th>
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
  <tr>
   <td><strong>Designer e-mail - Azioni cartella</strong>: parità con il vecchio editor e-mail.
   <ul>
   <li>Condivisione e archiviazione delle azioni cartella per le risorse di E-mail Designer.</li>
   <li>Condividi le cartelle nelle aree di lavoro, fai clic con il pulsante destro del mouse su una cartella per creare una nuova risorsa e sposta le risorse tramite trascinamento.</li>
   </ul>
   </td>
   <td>Rilasciato</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-mail Designer - API</strong>: ora puoi utilizzare le chiamate API per E-mail Designer.</td>
   <td>Rilasciato</td>
   <td><a href="https://developer.adobe.com/marketo-apis/api/asset#">Marketo Asset API</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer e-mail - Generazione immagini Assistente AI</strong>: ora, oltre a Firefly, puoi utilizzare modelli Nano Banana per generare immagini con l'Assistente AI per contenuti e-mail.</td>
   <td>Rilasciato</td>
   <td><a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/email-marketing/email-designer/ai-assistant#create-content-for-a-specific-section">Creare contenuti per una sezione specifica dell’e-mail</a></td>
  </tr>
  </tbody>
</table>
<br/>

## Annunci {#announcements}

* **Funzionalità SEO obsoleta**: martedì 31 marzo 2026, Marketo Engage dichiarerà obsoleta la funzionalità di ottimizzazione per i motori di ricerca (SEO). Se non utilizzi attivamente la SEO (Search Engine Optimization), non devi fare nulla. Se hai utilizzato SEO di recente, puoi esportare i dati. [Ulteriori informazioni](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/seo-feature-deprecation-248617?profile.language=it){target="_blank"}.

* **Limite dei lead di unione API REST**: a partire dal 31 marzo 2026, le chiamate che includono più di 25 ID nel parametro leadIds di una chiamata API dei lead di unione genereranno un codice di errore 1080 e la chiamata verrà ignorata. I posti di lavoro che richiedono la fusione di più di 25 record in uno dovrebbero essere suddivisi in più lavori per garantire il successo di tali chiamate.

* **Parametro “access_token” API Rest obsoleto**: il parametro di query `access_token` utilizzato per autenticare le chiamate API REST di Marketo è ora obsoleto e non sarà più disponibile dopo il sabato 31 luglio 2026. Tutte le integrazioni nuove ed esistenti devono autenticare le chiamate API REST utilizzando l’intestazione “Authorization”, [come descritto qui](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **API SOAP obsolete**: il supporto per le API SOAP di Marketo terminerà il sabato 31 luglio 2026. I servizi che utilizzano le funzionalità API SOAP devono essere migrati alle [API REST](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
