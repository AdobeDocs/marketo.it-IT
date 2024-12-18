---
description: Note sulla versione corrente - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione corrente
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 4e13fbba90efcecf8f22e4d8cdc5173e6f6f43a4
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 2%

---

# Note sulla versione: gennaio 2025 {#release-notes-jan-25}

Qui sotto troverai tutte le funzioni incluse nella versione di gennaio 2025. Verifica la disponibilità delle funzioni nella tua edizione di Adobe Marketo Engage.

Le note sulla versione specificatamente per l&#39;Adobe Dynamic Chat [ si trovano qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![stella](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzionalità rientrano nel ciclo di rilascio standard e inizieranno a essere rilasciate il **17 gennaio 2025**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funzione</th> 
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
    <tr> 
   <td><strong>Nuovo Designer e-mail</strong>: crea e-mail moderne ed efficienti utilizzando il nuovo Designer e-mail nativo nel Marketo Engage. Accedi a uno dei modelli e-mail predefiniti oppure creane facilmente uno tuo. Utilizza i contenuti dinamici e accedi alle immagini da Adobe Experience Manager Cloud Services.</td> 
   <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
  <tr> 
   <td><strong>Annulla registrazione partecipanti da un evento nei webinar interattivi</strong>: se non desideri un partecipante al webinar per qualsiasi motivo, puoi annullarne la registrazione. Il flusso di lavoro rimuove il registrante sia dal programma Marketo Event che da Adobe Connect.</td> 
   <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  <tr> 
   <td><strong>Disabilita campagne nell'archivio</strong>: disabilita le campagne con trigger attivo e annulla eventuali esecuzioni batch pianificate di campagne in una cartella al momento dell'archiviazione. Poiché è in corso un controllo aggiuntivo delle autorizzazioni per l'archiviazione di cartelle che contengono campagne attive (Attiva campagna trigger e Pianifica campagna batch), questa funzione viene disabilitata per impostazione predefinita con questa versione e può essere abilitata passando a <b>Amministratore</b> &gt; <b>Sfondo tesoro</b> nell'abbonamento di Marketo Engage.</td> 
   <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
  <tr> 
 </tbody> 
</table>
<br/>

## Annunci {#announcements}

* **Aggiornamento API Get Program Members**: è stata migliorata l&#39;API [Get Program Members](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/program-members#query){target="_blank"} per supportare la possibilità di recuperare l&#39;identificatore dei membri del programma. A questo scopo, aggiungi l’ID all’elenco di campi specificati nel parametro fields della richiesta API.

* **Deprecazione parametro &#39;access_token&#39; API REST**: il parametro di query `access_token` utilizzato per autenticare le chiamate API REST di Marketo è obsoleto e non sarà disponibile dopo il 30 giugno 2025. Tutte le integrazioni nuove ed esistenti devono autenticare le chiamate API REST utilizzando l&#39;intestazione &#39;Authorization&#39;, [come descritto qui](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Deprecazione API SOAP**: il supporto per l&#39;API SOAP di Marketo terminerà il 31 ottobre 2025. I servizi che utilizzano le funzionalità API dell&#39;SOAP devono essere migrati all&#39;[API REST](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
