---
unique-page-id: 10097199
description: Note sulla versione -Inverno '16 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Inverno '16
exl-id: 1e3b9207-27fe-47b1-b709-1306ac57b93b
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 0%

---

# Note sulla versione: inverno 2016 {#release-notes-winter}

Le seguenti funzioni sono incluse nella versione invernale del &#39;16. Fai clic sui collegamenti del titolo per visualizzare articoli dettagliati per ciascuna funzione.

## [Filtro anonimo](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website/next-generation-munchkin-tracking-faq.md) {#is-anonymous-filter}

Il filtro È anonimo è stato rimosso per gli elenchi avanzati. Consulta la [Domande frequenti sul tracciamento Munchkin di nuova generazione](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website/next-generation-munchkin-tracking-faq.md) per i dettagli. Questa modifica non influisce sulla personalizzazione web (RTP, Web Personalization), che continua a identificare visitatori web anonimi e noti e a personalizzare contenuti in tempo reale per tali visitatori.

## [Dashboard del database](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md) {#database-dashboard}

Il database dei lead dispone di una dashboard di riepilogo aggiornata che include le dimensioni totali del database delle persone, il numero di lead commerciabili e una suddivisione dei lead per le prime cinque origini.

![](assets/image2016-1-12-16-3a18-3a7.png)

## [Browser Edge di Microsoft](/help/marketo/product-docs/administration/setup-administration/supported-browsers.md) {#microsoft-edge-browser}

Microsoft Edge è stato aggiunto al [elenco dei browser](https://docs.marketo.com/display/public/DOCS/Supported+Browsers) supportati da Marketo.

## [Microsoft Outlook 2016](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md) {#microsoft-outlook}

[Microsoft Outlook 2016](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md) è ora supportato.

## [Inizio intestazione programma e-mail](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) {#email-program-head-start}

Utilizza Head Start per indicare che l’elaborazione dell’invio deve avvenire in anticipo. Invece di qualificare i lead e preparare le e-mail all’orario pianificato del programma, Head Start assicura che queste attività vengano eseguite in anticipo. In questo modo, il pubblico inizierà a ricevere e-mail all’ora pianificata.

![](assets/image2016-1-11-15-3a38-3a3.png)

Per utilizzare questa funzione, il programma e-mail deve essere pianificato con almeno 12 ore di anticipo e l’elenco avanzato verrà bloccato 12 ore prima dell’invio.

![](assets/image2016-1-11-15-3a35-3a55.png)

>[!NOTE]
>
>Questa funzione verrà implementata gradualmente per una settimana dopo il rilascio della versione invernale del 16. Non è disponibile per l’utilizzo con campagne intelligenti o con l’API.

## [Miglioramenti al mobile marketing](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md) {#mobile-marketing-enhancements}

**Supporto PhoneGap:** Ora offriamo il supporto di PhoneGap per la tua app mobile. [Ulteriori informazioni](https://developers.marketo.com/documentation/mobile/phonegap-plugin/).

**Supporto per le app sandbox**:

![](assets/image2016-1-12-10-3a47-3a13.png)

## [API del programma](https://developers.marketo.com/documentation/programs/) {#program-api}

Crea, aggiorna e clona programmi tramite l’API REST. Ciò non include la creazione o l’aggiornamento di elenchi avanzati e campagne intelligenti all’interno di un programma.

## [Miglioramenti di Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md) {#microsoft-dynamics-enhancements}

**[Stato sincronizzazione](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md)**: mantieni le schede sulla velocità effettiva corrente e sul backlog del processo di sincronizzazione. Suddividilo per il numero di inserimenti e aggiornamenti per oggetto.

![](assets/pending-backog-cropped.png)

**[Notifiche](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md)**: ricevi notifiche per gli errori di sincronizzazione comuni, insieme a un elenco di lead che presentano tale errore.

![](assets/image2016-1-12-8-3a13-3a9.png)

## [Miglioramenti agli oggetti personalizzati](/help/marketo/product-docs/administration/marketo-custom-objects/create-marketo-custom-objects.md) {#custom-objects-enhancements}

È ora possibile creare relazioni molti-a-molti tra lead/account e un oggetto personalizzato utilizzando un oggetto intermedio con più campi di collegamento.

![](assets/image2016-1-11-12-3a59-3a59.png)

## [Annunci lead facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md) {#facebook-lead-ads}

[Facebook Lead ads](https://www.facebook.com/business/a/lead-ads) rappresentano un modo più diretto per un’azienda di eseguire campagne di generazione di lead su Facebook. Le persone compilano un modulo per esprimere interesse per un prodotto o un servizio, in modo che l&#39;azienda possa seguirli. L’integrazione di Marketo con Facebook Lead Ads acquisisce automaticamente le informazioni fornite da un lead all’interno del modulo Lead Ads. Le azioni di follow-up e le notifiche possono quindi essere automatizzate utilizzando il nuovo trigger Riempimenti annunci lead Facebook.

![](assets/image2016-1-11-10-3a20-3a39.png)

## [Pianificazione campagne web (personalizzazione in tempo reale)](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/schedule-a-web-campaign.md) {#web-real-time-personalization-campaign-scheduler}

Pianifica la campagna in anticipo. Imposta una data di inizio e una data di fine per i contenuti web personalizzati e per le campagne ripetute in giorni e ore specifici. Personalizza la pianificazione per visualizzare la campagna in base all’ora del visitatore web o al fuso orario selezionato.

![](assets/image2016-1-14-8-3a36-3a36.png)
