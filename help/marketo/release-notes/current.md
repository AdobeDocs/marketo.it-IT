---
description: Note sulla versione corrente - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione corrente
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
TQID: 'https://experienceleague.adobe.com/QJFy7PeGXlvS3jcJGcZJROlc8c1UvphO-TOOwPUQeX8'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
    internal-label: Forms
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
    internal-label: Resources
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
    internal-label: Templates
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
    internal-label: Dynamic Chat
  - id: af97ce94-35fa-4fa9-b85a-46b752ac4028
    internal-label: Release information
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 29aa413a7346a79906f4021dedc79e8e48170c69
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 15%
---
# Note sulla versione: ottobre 2026 {#release-notes-oct-26}

Qui sotto troverai tutte le funzioni incluse nella versione di ottobre 2026. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

Le note sulla versione specifiche per Adobe Dynamic Chat [sono disponibili qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzionalità rientrano nel ciclo di rilascio standard e inizieranno a essere rilasciate il **23 ottobre 2026**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funzione</th>
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
  <tr>
   <td><strong>Pianifica abilità campagne</strong>: CX Enterprise Coworker per Marketo Engage ora può trasformare una descrizione della campagna in un documento completo di configurazione del programma Marketo Engage. Il documento include una struttura di cartelle, campagne avanzate, configurazioni e-mail, token e un elenco di controllo del controllo qualità. In questo modo i team possono lanciare campagne più rapidamente e standardizzare la configurazione del programma. L’abilità è configurabile tramite markdown.</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Agenti chiamabili</strong>: crea agenti di intelligenza artificiale che vengono eseguiti come un passaggio di flusso nelle campagne intelligenti e che agiscono su un record di lead in base alle istruzioni scritte in linguaggio semplice. Ad esempio, un agente può normalizzare i dati di un lead o contrassegnare i probabili bot, quindi riscrivere il risultato nei campi del lead. In questo modo l’elaborazione dei lead basata sul giudizio viene inserita nelle campagne senza codice personalizzato.</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Clona in questo programma/cartella</strong>: le operazioni di clonazione in Marketo Engage offrono ora in modo coerente l'opzione "Questa cartella" o "Questo programma" come prima scelta quando si sceglie la destinazione della risorsa clonata. Scegliendo questa opzione, la risorsa viene clonata nel programma o nella cartella principale della risorsa corrente.</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <tr>
   <td><strong>Avviso immediato sulla sincronizzazione CRM</strong>: l'attivazione o la disattivazione della sincronizzazione CRM nativa per un ambiente attiva ora una notifica agli utenti abbonati al canale di notifica CRM.</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  </tr>
  </tbody>
</table>
<br/>

## Annunci {#announcements}

* **Deprecazione delle immagini di acquisizione dal Web**: per conformarsi alle moderne best practice per la protezione e la privacy, la funzionalità [Immagini di acquisizione dal Web](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/images-and-files/grab-the-images-from-a-web-page){target="_blank"} diventerà obsoleta a partire dalla versione di ottobre.

* **Restrizioni nome API per attributi attività personalizzati**: i nomi API per attributi attività personalizzati creati tramite API o interfaccia utente possono ora contenere solo caratteri alfanumerici e trattini bassi e devono iniziare con un carattere alfanumerico.

* **Limiti di dimensione elenco statico per attività Get Lead e modifiche Get Lead**: a partire dal 30 settembre 2026, le chiamate agli endpoint Get Lead Activities o Get Lead Changes che includono il parametro `listId` hanno avuto esito negativo con un codice di errore 1003 (che indica che l&#39;elenco statico di destinazione contiene troppi record) se gli elenchi di destinazione contengono 10.000 o più lead. Per ulteriori informazioni, consultare la [Guida alla migrazione](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"}.
