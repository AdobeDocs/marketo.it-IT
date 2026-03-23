---
description: Note sulla versione corrente - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione corrente
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: eb0e23b9f938e813edb90f615a6f1e9d06526dbc
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 40%

---

# Note sulla versione - Marzo 2026 {#release-notes-mar-26}

Qui sotto troverai tutte le funzioni incluse nella versione di marzo 2026. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

Le note sulla versione specifiche per Adobe Dynamic Chat [sono disponibili qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzioni rientrano nel ciclo di rilascio standard. Inizieranno a essere rilasciate il **sabato 27 marzo 2026**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funzione</th>
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
  <tr>
   <td><strong>E-mail Designer - Gestisci marchi (beta)</strong>: genera contenuti e-mail in base alle linee guida specifiche per la scrittura in copia della tua organizzazione o del tuo marchio.</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-mail Designer - Allineamento marchio</strong>: utilizza il controllo qualità contenuto per le e-mail per verificare la leggibilità e la coerenza generali dei messaggi.
   </td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-mail Designer - Correzione rendering di Outlook</strong>: questo aggiornamento risolve alcuni problemi di rendering, in particolare in MS Outlook. La "modalità Expert" consente di apportare modifiche minori a HTML/CSS o di aggiungere tag script all’e-mail (si consiglia di non apportare altre modifiche al HTML dell’e-mail per mantenere gli elementi visivi così come sono).
   </td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-mail Designer - Azioni rapide</strong>: <i>Parità con il vecchio editor e-mail</i>. Le azioni rapide sono ora disponibili per tutte le risorse di E-mail Designer (e-mail, modelli e-mail, frammenti). Le azioni rapide supportate includono: Duplica, Elimina, Sposta, Crea/Modifica bozza.
   </td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Gestione elenchi di controllo</strong>: è ora possibile specificare i valori che possono essere utilizzati nei campi di Marketo Engage.
   </td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Notifiche push</strong>: gli URL di reindirizzamento configurati nei messaggi di notifica push ora supportano i token di Marketo Engage (applicabile solo a <i>URL di app Launch</i>).
   </td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Annunci {#announcements}

* **Funzionalità SEO obsoleta**: martedì 31 marzo 2026, Marketo Engage dichiarerà obsoleta la funzionalità di ottimizzazione per i motori di ricerca (SEO). Se non utilizzi attivamente la SEO (Search Engine Optimization), non devi fare nulla. Se hai utilizzato SEO di recente, puoi esportare i dati. [Ulteriori informazioni](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/seo-feature-deprecation-248617?profile.language=it){target="_blank"}.

* **Limite dei lead di unione API REST**: a partire dal 31 marzo 2026, le chiamate che includono più di 25 ID nel parametro leadIds di una chiamata API dei lead di unione genereranno un codice di errore 1080 e la chiamata verrà ignorata. I posti di lavoro che richiedono la fusione di più di 25 record in uno dovrebbero essere suddivisi in più lavori per garantire il successo di tali chiamate.

* **Parametro “access_token” API Rest obsoleto**: il parametro di query `access_token` utilizzato per autenticare le chiamate API REST di Marketo è ora obsoleto e non sarà più disponibile dopo il sabato 31 luglio 2026. Tutte le integrazioni nuove ed esistenti devono autenticare le chiamate API REST utilizzando l’intestazione “Authorization”, [come descritto qui](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **API SOAP obsolete**: il supporto per le API SOAP di Marketo terminerà il sabato 31 luglio 2026. I servizi che utilizzano le funzionalità API SOAP devono essere migrati alle [API REST](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
