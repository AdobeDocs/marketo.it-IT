---
description: Note sulla versione corrente - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione corrente
hide: true
hidefromtoc: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
source-git-commit: 96050d108aae64bbdab377cf5e31392df177b363
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 61%

---

# Note sulla versione - Gennaio 2026 {#release-notes-jan-26}

Qui sotto troverai tutte le funzioni incluse nella versione di gennaio 2026. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

Le note sulla versione specifiche per Adobe Dynamic Chat [sono disponibili qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![star](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzioni rientrano nel ciclo di rilascio standard. Inizieranno a essere rilasciate il **sabato 30 gennaio 2026**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funzione</th>
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
  <tr>
   <td><strong>TITOLO FUNZIONE</strong>: descrizione funzione.</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>TITOLO FUNZIONE</strong>: descrizione funzione.</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>TITOLO FUNZIONE</strong>: descrizione funzione.</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>TITOLO FUNZIONE</strong>: descrizione funzione.</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>TITOLO FUNZIONE</strong>: descrizione funzione.</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>TITOLO FUNZIONE</strong>: descrizione funzione.</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>TITOLO FUNZIONE</strong>: descrizione funzione.</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Funzioni di Adobe Connect {#adobe-connect-features}

Queste funzioni sono già state rilasciate dal team Adobe Connect. I [webinar interattivi](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/interactive-webinars-overview){target="_blank"} di Marketo Engage sono basati su Adobe Connect. Di conseguenza, le funzioni riportate di seguito sono applicabili solo agli utenti dei webinar interattivi.

* **Pod sondaggio**: Adobe Connect 12.11 introduce un nuovo Pod sondaggio che consente agli host di progettare e consegnare moduli di feedback strutturati direttamente all&#39;interno di una sessione live.

* **Pod risorse**: il nuovo pod risorse sostituisce i pod precedenti File e Collegamenti Web, fornendo un unico modo unificato per condividere le risorse durante le sessioni live.

* **Esperienza avanzata dell&#39;interfaccia della stanza**: Adobe Connect 12.11 introduce un&#39;interfaccia della stanza aggiornata e più moderna, basata sull&#39;ultimo framework di progettazione Spectrum 2 di Adobe, in linea con il linguaggio visivo utilizzato in altri prodotti Adobe come Creative Cloud e Experience Cloud.

Per informazioni dettagliate, consulta le [Note sulla versione di Adobe Connect 12.11](https://helpx.adobe.com/it/adobe-connect/release-note/adobe-connect-12-11-release-notes.html){target="_blank"}.

## Annunci {#announcements}

* **Deprecazione parametro &#39;access_token&#39; API Rest**: il parametro di query `access_token` utilizzato per autenticare le chiamate API REST di Marketo è obsoleto e non sarà più disponibile dopo il mercoledì 31 marzo 2026. Tutte le integrazioni nuove ed esistenti devono autenticare le chiamate API REST utilizzando l’intestazione &#39;Authorization&#39;, [come descritto qui](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Deprecazione API SOAP**: il supporto per l’API SOAP di Marketo terminerà il mercoledì 31 marzo 2026. I servizi che utilizzano le funzionalità API SOAP devono effettuare la migrazione all’[API REST](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Fine del ciclo di vita dell&#39;identità di Marketo Engage**:

   * _Deprecazione limitazioni IP_: il supporto per [Limitazione degli accessi a Marketo basati su IP](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} è terminato il 30 luglio 2025. La funzione rimarrà operativa fino al completamento della transizione ad Adobe Identity. A breve sarà disponibile una nuova funzione di controllo degli accessi basata sulla posizione per Adobe Identity in Adobe Admin Console.

   * _Deprecazione single sign-on (SSO)_: il supporto per [Marketo Identity SSO](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} è terminato il 30 luglio 2025. La funzione rimarrà operativa fino al completamento della transizione ad Adobe Identity. Il Single Sign-On per Adobe Identity in Adobe Admin Console deve essere configurato separatamente. Per i passaggi di configurazione, vedi [Configurare identità e Single Sign-On](https://helpx.adobe.com/it/enterprise/using/set-up-identity.html){target="_blank"}.
