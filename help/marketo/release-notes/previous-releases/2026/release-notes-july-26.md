---
description: Note sulla versione - Luglio 2026 - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione - Luglio 2026
feature: Release Information
source-git-commit: 093bb2edda0a9c70bf45462fc8a67c45bda9b4e1
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 19%

---

# Note sulla versione: luglio 2026 {#release-notes-july-26}

Di seguito trovi tutte le funzioni incluse nella versione di luglio 2026. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

Le note sulla versione specifiche per Adobe Dynamic Chat [sono disponibili qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzionalità rientrano nel ciclo di rilascio standard e inizieranno a essere rilasciate il **10 luglio 2026**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funzione</th>
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
  <tr>
   <td><strong>Competenza Marketo AI - Conoscenza del prodotto</strong>: la conoscenza del prodotto consente l'accesso on-demand alle competenze Marketo senza uscire dalla piattaforma. Poni una domanda in un linguaggio semplice e l’intelligenza artificiale di Marketo si basa sulla documentazione ufficiale di Adobe per fornire una risposta.
</td>
   <td>Rilasciato</td>
   <td><a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/marketo-ai/skills/product-knowledge" target="_blank">Conoscenza del prodotto</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Abilità di Marketo AI - Indagine sui lead</strong>: scopri perché una persona/un lead specifico non ha raggiunto una fase cardine (come MQL, qualificazione del programma o una campagna) e ottieni una spiegazione semplice di ciò che è successo.
</td>
   <td>Rilasciato</td>
   <td><a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/marketo-ai/skills/investigate-leads" target="_blank">Indagare sui lead</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-mail Designer - Moduli</strong>: ora puoi accedere a blocchi di contenuto pronti all'uso e completamente strutturati progettati per accelerare l'assembly delle e-mail.</td>
   <td>Rilasciato</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/email-modules.md" target="_blank">Utilizzare i moduli in E-mail Designer</a></td>
  </tr>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer e-mail - Genera contenuto menu contestuale</strong>: le funzioni "Genera contenuto" di Designer e-mail sono ora accessibili dal menu contestuale (la barra nera). Ad esempio, quando selezioni il contenuto di testo, l’icona Genera contenuto viene visualizzata nel menu contestuale, consentendo di eseguire azioni rapide da lì.</td>
   <td><i>Disponibile a breve</i></td>
<td><i>Disponibile a breve</i></td>
  </tr>
  </tr>
  </tbody>
</table>
<br/>



## Annunci {#announcements}

* **Deprecazione parametro &#39;access_token&#39; API REST**: il parametro di query `access_token` utilizzato per autenticare le chiamate API REST di Marketo è obsoleto e non sarà disponibile dopo il 31 agosto 2026. Tutte le integrazioni nuove ed esistenti devono autenticare le chiamate API REST utilizzando l’intestazione “Authorization”, [come descritto qui](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.
* **Limite dei lead di unione API REST**: a partire dal 31 luglio 2026, le chiamate che includono più di 25 ID nel parametro leadIds di una chiamata API dei lead di unione genereranno un codice di errore 1080 e la chiamata verrà ignorata. I posti di lavoro che richiedono la fusione di più di 25 record in uno dovrebbero essere suddivisi in più lavori per garantire il successo di tali chiamate.
* **API SOAP obsoleta**: il supporto per l&#39;API Marketo SOAP terminerà il 31 luglio 2026. I servizi che utilizzano le funzionalità API SOAP devono essere migrati alle [API REST](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
* **Limiti di dimensione elenco statico per attività Get Lead e modifiche Get Lead**: a partire dal 30 settembre 2026, le chiamate agli endpoint Get Lead Activities e Get Lead Changes che includono il parametro `listId` restituiranno un codice di errore 1003 se l&#39;elenco statico di destinazione contiene 10.000 o più lead. Per ulteriori informazioni, consultare la [Guida alla migrazione](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"}.
