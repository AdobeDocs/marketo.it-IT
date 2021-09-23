---
unique-page-id: 10097199
description: Note sulla versione - Inverno del 16 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Inverno '16
exl-id: 1e3b9207-27fe-47b1-b709-1306ac57b93b
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 0%

---

# Note sulla versione: Inverno &#39;16 {#release-notes-winter}

Le seguenti funzionalità sono incluse nella versione invernale del 16. Fai clic sui collegamenti del titolo per visualizzare gli articoli dettagliati per ciascuna funzione.

## [È un filtro anonimo](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website/next-generation-munchkin-tracking-faq.md) {#is-anonymous-filter}

Il filtro Is Anonymous è stato rimosso per gli elenchi avanzati. Per ulteriori informazioni, consulta il documento [Next Generation Munchkin Tracking FAQ](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website/next-generation-munchkin-tracking-faq.md) . Questa modifica non influisce sulla personalizzazione web (RTP, Web Personalization), che continua a identificare visitatori web anonimi e noti e a personalizzare contenuti in tempo reale per tali visitatori.

## [Dashboard del database](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md) {#database-dashboard}

Il database lead dispone di un dashboard di riepilogo aggiornato che include la dimensione totale del database delle persone, il numero di lead commerciabili e una suddivisione dei lead per cinque origini principali.

![](assets/image2016-1-12-16-3a18-3a7.png)

## [Browser Microsoft Edge](/help/marketo/product-docs/administration/setup-administration/supported-browsers.md) {#microsoft-edge-browser}

Microsoft Edge è stato aggiunto all’ [elenco di browser](https://docs.marketo.com/display/public/DOCS/Supported+Browsers) supportati da Marketo.

## [Microsoft Outlook 2016](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md) {#microsoft-outlook}

[Microsoft Outlook 2016](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md) è ora supportato.

## [Inizio programma e-mail](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) {#email-program-head-start}

Utilizza Head Start per indicare che l’elaborazione per l’invio deve avvenire in anticipo. Invece di qualificarsi per i lead e preparare le e-mail al momento previsto del programma, Head Start garantisce che queste attività vengano eseguite in anticipo. In questo modo, il pubblico inizierà a ricevere e-mail all’ora pianificata.

![](assets/image2016-1-11-15-3a38-3a3.png)

Per utilizzare questa funzione, il programma e-mail deve essere pianificato almeno 12 ore prima e l’elenco avanzato verrà bloccato 12 ore prima dell’invio.

![](assets/image2016-1-11-15-3a35-3a55.png)

>[!NOTE]
>
>Questa funzione verrà implementata gradualmente per una settimana dopo il rilascio invernale del 16. Non è disponibile per l’utilizzo con campagne avanzate o con l’API.

## [Miglioramenti al Mobile Marketing](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md) {#mobile-marketing-enhancements}

**Supporto PhoneGap:** ora offriamo il supporto PhoneGap per la tua app mobile. [Ulteriori informazioni](https://developers.marketo.com/documentation/mobile/phonegap-plugin/).

**Supporto per le app** sandbox:

![](assets/image2016-1-12-10-3a47-3a13.png)

## [API del programma](https://developers.marketo.com/documentation/programs/) {#program-api}

Creare, aggiornare e clonare programmi tramite l’API REST. Ciò non include la creazione o l&#39;aggiornamento di elenchi smart e campagne intelligenti all&#39;interno di un programma.

## [Miglioramenti a Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md) {#microsoft-dynamics-enhancements}

**[Stato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md)** sincronizzazione: Mantieni le schede sulla velocità effettiva corrente e sul backlog del processo di sincronizzazione. Suddividila per numero di inserimenti e aggiornamenti per oggetto.

![](assets/pending-backog-cropped.png)

**[Notifiche](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md)**: Ricevi notifiche per errori di sincronizzazione comuni, insieme a un elenco di lead con tale errore.

![](assets/image2016-1-12-8-3a13-3a9.png)

## [Miglioramenti agli oggetti personalizzati](/help/marketo/product-docs/administration/marketo-custom-objects/create-marketo-custom-objects.md) {#custom-objects-enhancements}

È ora possibile creare relazioni molti-a-molti tra Lead/Account e un oggetto personalizzato utilizzando un oggetto intermedio con più campi di collegamento.

![](assets/image2016-1-11-12-3a59-3a59.png)

## [Annunci lead facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md) {#facebook-lead-ads}

[Gli ](https://www.facebook.com/business/a/lead-ads) adsb lead di facebook sono un modo più diretto per un’azienda di eseguire campagne di generazione di lead su Facebook. Le persone compilano un modulo per esprimere interesse per un prodotto o un servizio, in modo che l&#39;azienda possa seguirli. L’integrazione di Marketo con Facebook Lead Ads acquisisce automaticamente le informazioni fornite da un lead all’interno del modulo lead Ads. Le azioni di follow-up e le notifiche possono quindi essere automatizzate utilizzando il nuovo trigger Fills Out Facebook Lead Ads .

![](assets/image2016-1-11-10-3a20-3a39.png)

## [Modulo di pianificazione delle campagne Web (Personalizzazione in tempo reale)](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/schedule-a-web-campaign.md) {#web-real-time-personalization-campaign-scheduler}

Pianifica la tua campagna in anticipo. Imposta una data di inizio e di fine per contenuti web personalizzati e campagne ripetute in giorni e ore specifici. Personalizza la pianificazione per visualizzare la campagna in base all’ora del visitatore web o a un fuso orario selezionato.

![](assets/image2016-1-14-8-3a36-3a36.png)
