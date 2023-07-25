---
unique-page-id: 13795395
description: Note sulla versione -Inverno '18 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Inverno '18
exl-id: f08bdc91-86d3-4ea2-a74a-1398ed525bbb
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 0%

---

# Note sulla versione: inverno 2018 {#release-notes-winter}

Le seguenti funzioni sono incluse nella versione invernale del 18. Verifica la disponibilità delle funzioni nella tua edizione di Marketo.

Fai clic sui collegamenti del titolo per visualizzare articoli dettagliati per ciascuna funzione. **Nota**: ad alcune funzioni incluse in questa versione non sono associati articoli. Se un argomento ha più sottotitoli, i collegamenti sono posizionati lì.

## Miglioramenti a livello di prestazioni e velocità effettiva delle campagne {#campaign-performance-and-throughput-enhancements}

Marketo sfrutta la nostra architettura dei big data per aumentare la velocità effettiva delle campagne trigger e migliorare l’elaborazione delle attività web, in modo da poter reagire più rapidamente alle azioni del pubblico.

## Miglioramenti all’integrazione con Salesforce CRM di Marketo {#enhancements-to-marketo-s-salesforce-crm-integration}

Abbiamo due miglioramenti alla nostra integrazione con la gestione delle relazioni con i clienti Salesforce:

* [Notifiche dell’amministratore di Marketo](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md) per alcuni errori di sincronizzazione CRM (credenziali scadute, limiti API raggiunti, ecc.)

* [Possibilità di disattivare le notifiche e-mail](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/turn-off-email-notifications-to-lead-owner.md) a Proprietari lead all&#39;assegnazione del lead

Questi miglioramenti verranno implementati nel corso del 2018.

## [Informazioni sulle prestazioni di Marketo](/help/marketo/product-docs/reporting/performance-insights/performance-insights-overview.md) {#marketo-performance-insights}

>[!AVAILABILITY]
>
>Performance Insights è un prodotto aggiuntivo. Contatta il tuo Account Manager o Account Executive Marketo per richiedere un preventivo.

Scopri in che modo le campagne e i canali influiscono sui risultati aziendali con analisi dell’attribuzione, visualizzazioni interattive e una tabella di dati dettagliata.

![](assets/image2018-2-5-7-3a55-3a46.png)

## Miglioramenti del marketing basato sull’account {#account-based-marketing-enhancements}

**[Gerarchie ABM](/help/marketo/product-docs/target-account-management/target/named-accounts/tam-hierarchies.md)**

Per i clienti ABM con Salesforce o Microsoft Dynamics, ABM ora erediterà automaticamente (e visualizzerà) le relazioni padre-figlio stabilite nel CRM. Potrai utilizzare queste relazioni sia nel reporting aggregato che nell’esecuzione della campagna.

## E-mail marketing {#email-marketing}

**[Script e-mail dinamico](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)**

Lo script Velocity è ora supportato nelle e-mail che utilizzano il contenuto dinamico. Combina velocità e contenuti dinamici basati sulla segmentazione per creare e-mail altamente personalizzate.

**Fuso orario destinatario**

* **[Cadenza dell&#39;allattamento mensile](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)**: abbiamo aggiunto la possibilità di pianificare programmi di sviluppo per un mese.

* **[Interrompi consegna](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)**: ora puoi interrompere gli invii rimanenti a metà dell’esecuzione.

## Integrazioni di reti pubblicitarie {#ad-network-integrations}

**[Integrazione Customer Match di Google](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-google-customer-match-as-a-launchpoint-service.md)**

Con questa integrazione, puoi inviare un pubblico Marketo a Google per il targeting utilizzando Google AdWords, nonché per il re-targeting del pubblico in YouTube, Search e Gmail.

**[Miglioramento dell’API di linkedIn Matched Audiences](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md)**

La nuova API di LinkedIn ora consente di eseguire il targeting delle persone nel database di Marketo tra più account di LinkedIn Campaign Manager.

## Personalizzazione web {#web-personalization}

**Origine dati giapponese per la personalizzazione web**

Marketo sta aggiungendo un’ulteriore origine dati giapponese per la personalizzazione web per migliorare l’identificazione dei visitatori web (ricerca IP inversa) e la personalizzazione per i visitatori provenienti dal Giappone. I nomi delle organizzazioni verranno visualizzati in giapponese.

**[Creare un segmento web utilizzando elenchi statici](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-a-static-list.md)**

La personalizzazione web può ora personalizzare il contenuto per un visitatore web noto che fa parte di un elenco statico definito in Attività di marketing (MLM). Con questo miglioramento, ora puoi vendere a elenchi statici tra canali diversi e indirizzare le persone in tali elenchi con contenuti personalizzati sul tuo sito web.

## ContentAI {#contentai}

**Miglioramento dell’algoritmo predittivo**

Il contenuto consigliato tramite gli algoritmi ContentAI ottimizzati di Marketo genera fino al doppio di clic rispetto al contenuto casuale.

## Integrazione {#integration}

**[Attivare/disattivare l’API di Campaign](https://developers.marketo.com/rest-api/assets/smart-campaigns/)**

Questa nuova API consente di attivare e disattivare in remoto le campagne di attivazione, per creare modelli di programma completamente automatizzati. Crea un modello di programma una volta, quindi automatizza la clonazione, gli aggiornamenti dei materiali di marketing e ora l’attivazione/pianificazione delle campagne intelligenti.

## ToutApp {#toutapp}

**Aggiornamento per annullamento iscrizione**

A partire dal 1° marzo 2018, tutte le e-mail inviate da [ToutApp.com](https://ToutApp.com) (e utilizzando il pulsante &quot;E-mail con Tout&quot; in Salesforce) avrà un collegamento di annullamento dell’abbonamento aggiunto in basso.

**Aggiornamento feed live**

Abbiamo aggiornato l&#39;aspetto delle schede Coinvolgimento e Attività per rendere più semplice e veloce la risposta dei membri delle vendite alle attività dei clienti direttamente dal feed live.

**Aggiornamento visualizzazione dettagli persone**

Il PDV (People Detail View) migliorato offre una visione completa dei contatti riunendo i dettagli di contatto Tout e Salesforce CRM.
