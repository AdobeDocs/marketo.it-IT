---
unique-page-id: 13795395
description: Note sulla versione - Inverno del 18 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Inverno '18
exl-id: f08bdc91-86d3-4ea2-a74a-1398ed525bbb
source-git-commit: 6ad418c8f4056b9a2fb31b0ac995692f0c618795
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 0%

---

# Note sulla versione: Inverno &#39;18 {#release-notes-winter}

Le seguenti funzionalità sono incluse nella versione invernale del 18. Per informazioni sulla disponibilità delle funzioni, consulta la tua edizione Marketo .

Fai clic sui collegamenti del titolo per visualizzare gli articoli dettagliati per ciascuna funzione. **Nota**: Alcune delle funzioni incluse in questa versione non hanno articoli associati. Se un argomento ha più sottotitoli, i collegamenti vengono posizionati in tale punto.

## Miglioramenti a livello di prestazioni e velocità di trasmissione delle campagne {#campaign-performance-and-throughput-enhancements}

Marketo sfrutta la nostra architettura dei dati di grandi dimensioni per aumentare il throughput delle campagne e migliorare l’elaborazione delle attività web, in modo da poter reagire più rapidamente alle azioni del pubblico.

## Miglioramenti all’integrazione di Marketo con Salesforce CRM {#enhancements-to-marketo-s-salesforce-crm-integration}

Abbiamo due miglioramenti alla nostra integrazione CRM Salesforce:

* [Notifiche agli amministratori di Marketo](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md) per alcuni errori di sincronizzazione CRM (credenziali scadute, limiti API raggiunti, ecc.)

* [Possibilità di disattivare le notifiche e-mail](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/turn-off-email-notifications-to-lead-owner.md) per i proprietari lead in caso di assegnazione lead

Questi miglioramenti saranno implementati nel 2018.

## [Informazioni sulle prestazioni di Marketo](/help/marketo/product-docs/reporting/performance-insights/performance-insights-overview.md) {#marketo-performance-insights}

>[!AVAILABILITY]
>
>Performance Insights è un prodotto aggiuntivo. Contatta il tuo Marketo Customer Success Manager o Account Executive per un preventivo.

Scopri in che modo le campagne e i canali hanno un impatto sui risultati aziendali con analisi di attribuzione, visualizzazioni interattive e una tabella di dati dettagliata.

![](assets/image2018-2-5-7-3a55-3a46.png)

## Miglioramenti al marketing basato su account {#account-based-marketing-enhancements}

**[Gerarchie ABM](/help/marketo/product-docs/target-account-management/target/named-accounts/tam-hierarchies.md)**

Per i clienti ABM con Salesforce o Microsoft Dynamics, ABM erediterà automaticamente (e visualizzerà) le relazioni padre-figlio stabilite nel CRM. Potrai utilizzare queste relazioni sia nel reporting roll-up che nell’esecuzione di campagne.

## E-mail marketing {#email-marketing}

**[Script e-mail dinamico](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)**

Gli script Velocity sono ora supportati nelle e-mail che utilizzano contenuto dinamico. Combina velocità e contenuti dinamici basati sulla segmentazione per creare e-mail altamente personalizzate.

**Fuso orario destinatario**

* **[Caduta mensile dell&#39;infermiera](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)**: Abbiamo aggiunto la possibilità di programmare programmi di nutrizione su cadenza mensile.

* **[Interrompi consegna](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)**: Ora puoi interrompere tutti gli invii rimanenti a metà esecuzione.

## Integrazioni di reti di annunci {#ad-network-integrations}

**[Integrazione Customer Match di Google](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-google-customer-match-as-a-launchpoint-service.md)**

Con questa integrazione, puoi inviare un pubblico Marketo a Google per il targeting utilizzando Google AdWords, nonché rieseguire il targeting del pubblico in YouTube, Search e Gmail.

**[Miglioramento dell’API di linkedIn Matched Audiences](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md)**

La nostra nuova API LinkedIn ora ti consente di rieseguire il targeting delle persone nel database Marketo in più account LinkedIn Campaign Manager.

## Personalizzazione web {#web-personalization}

**Origine dati giapponese per Web Personalization**

Marketo sta aggiungendo un’origine dati giapponese aggiuntiva per Web Personalization per migliorare l’identificazione dei visitatori web (ricerca IP inversa) e la personalizzazione per i visitatori provenienti dal Giappone. I nomi dell&#39;organizzazione verranno visualizzati in giapponese.

**[Creare un segmento Web utilizzando elenchi statici](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-a-static-list.md)**

Web Personalization ora può personalizzare il contenuto per un visitatore web noto che fa parte di un elenco statico definito in Attività di marketing (MLM). Con questo miglioramento, ora puoi commercializzare elenchi statici su più canali e rivolgerti alle persone in questi elenchi con contenuti personalizzati sul tuo sito web.

## ContentAI {#contentai}

**Miglioramento dell&#39;algoritmo predittivo**

I contenuti consigliati tramite gli algoritmi di ContentAI ottimizzati per Marketo generano fino al doppio dei clic rispetto al contenuto casuale.

## Integrazione {#integration}

**[Attivare/disattivare l’API di Campaign](https://developers.marketo.com/rest-api/assets/smart-campaigns/)**

Questa nuova API consente di attivare e disattivare in remoto le campagne di attivazione, per creare modelli di programma completamente automatizzati. Crea un modello di programma una volta, quindi automatizza la clonazione, gli aggiornamenti collaterali di marketing e ora l&#39;attivazione/pianificazione di campagne intelligenti.

## ToutApp {#toutapp}

**Annulla sottoscrizione aggiornamento**

A partire dal 1° marzo 2018, tutte le e-mail inviate da [ToutApp.com](https://ToutApp.com) (e utilizzando il pulsante &quot;Email with Tout&quot; in Salesforce) sarà aggiunto un collegamento per l’annullamento dell’abbonamento in basso.

**Aggiornamento dei feed live**

Abbiamo aggiornato l’aspetto delle schede Coinvolgimento e Attività per facilitare e velocizzare la risposta dei membri vendite alle attività dei clienti direttamente dal feed live.

**Aggiornamento della vista Dettagli persone**

La visualizzazione dei dettagli delle persone (PDV) migliorata offre una visione completa dei tuoi contatti riunendo i tuoi dati di contatto per il CRM di Tout e Salesforce.
