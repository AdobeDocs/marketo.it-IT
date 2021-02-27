---
unique-page-id: 10097199
description: Note sulla versione -Winter '16 - Marketo Docs - Documentazione prodotto
title: Note sulla versione - Inverno '16
translation-type: tm+mt
source-git-commit: 029d8b419ba5078980b4fde9890bdb35194bf264
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 0%

---


# Note sulla versione: Inverno &#39;16 {#release-notes-winter}

Le seguenti funzionalità sono incluse nella release invernale &#39;16. Fate clic sui collegamenti del titolo per visualizzare articoli dettagliati per ciascuna funzione.

## [Filtro anonimo](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website/next-generation-munchkin-tracking-faq.md) {#is-anonymous-filter}

Il filtro Is Anonymous è stato rimosso per gli Smart List. Per ulteriori informazioni, consultare il documento [Next Generation Munchkin Tracking FAQ](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website/next-generation-munchkin-tracking-faq.md). Questa modifica non influisce sulla Web Personalization (RTP), che continua a identificare visitatori Web anonimi e noti e a personalizzare i contenuti in tempo reale per tali visitatori.

## [Pannello database](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md)  {#database-dashboard}

Il database lead dispone di un dashboard di riepilogo aggiornato che include la dimensione totale del database delle persone, il numero di lead commercializzabili e una suddivisione dei lead per cinque origini principali.

![](assets/image2016-1-12-16-3a18-3a7.png)

## [Microsoft Edge Browser](/help/marketo/product-docs/administration/setup-administration/supported-browsers.md) {#microsoft-edge-browser}

Microsoft Edge è stato aggiunto all&#39;elenco [dei browser](https://docs.marketo.com/display/public/DOCS/Supported+Browsers) supportati da Marketo.

## [Microsoft Outlook 2016](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md) {#microsoft-outlook}

[Microsoft Outlook 2016 ora ](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md) è supportato.

## [Inizio programma e-mail](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) {#email-program-head-start}

Utilizzate Head Start per indicare che l&#39;elaborazione per il vostro invio deve avvenire in anticipo. Invece di classificare i lead e preparare i messaggi e-mail al momento previsto del programma, Head Start garantisce che tali attività vengano eseguite in anticipo. In questo modo, il pubblico inizierà a ricevere e-mail all&#39;ora pianificata.

![](assets/image2016-1-11-15-3a38-3a3.png)

Per utilizzare questa funzione, il programma e-mail deve essere pianificato almeno 12 ore prima dell&#39;invio e l&#39;Smart List verrà bloccato 12 ore prima dell&#39;invio.

![](assets/image2016-1-11-15-3a35-3a55.png)

>[!NOTE]
>
>Questa funzione verrà implementata gradualmente per una settimana dopo la release invernale &#39;16. Non è disponibile per l&#39;utilizzo con campagne intelligenti o con l&#39;API.

## [Miglioramenti di Mobile Marketing](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md) {#mobile-marketing-enhancements}

**Supporto PhoneGap:** ora offriamo il supporto PhoneGap per la vostra app mobile. [Ulteriori](https://developers.marketo.com/documentation/mobile/phonegap-plugin/) informazioni.

**Supporto per le app** sandbox:

![](assets/image2016-1-12-10-3a47-3a13.png)

## [API del programma](https://developers.marketo.com/documentation/programs/) {#program-api}

Creare, aggiornare e duplicare i programmi tramite REST API. Ciò non include la creazione o l&#39;aggiornamento di elenchi smart e campagne intelligenti all&#39;interno di un programma.

## [Miglioramenti di Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md) {#microsoft-dynamics-enhancements}

**[Stato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md)** sincronizzazione: Tenere schede sulla velocità effettiva corrente e sul backlog del processo di sincronizzazione. Suddividerlo per numero di inserimenti e aggiornamenti per oggetto.

![](assets/pending-backog-cropped.png)

**[Notifiche](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md)**: Ricevi notifiche per errori di sincronizzazione comuni, insieme a un elenco di lead che presentano tale errore.

![](assets/image2016-1-12-8-3a13-3a9.png)

## [Miglioramenti agli oggetti personalizzati](/help/marketo/product-docs/administration/marketo-custom-objects/create-marketo-custom-objects.md) {#custom-objects-enhancements}

È ora possibile creare relazioni molti-a-molti tra Lead/Account e un oggetto personalizzato utilizzando un oggetto intermediario con più campi di collegamento.

![](assets/image2016-1-11-12-3a59-3a59.png)

## [Annunci lead Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md) {#facebook-lead-ads}

[I ](https://www.facebook.com/business/a/lead-ads) principali indirizzi di Facebook rappresentano un modo più diretto per consentire a un&#39;azienda di gestire campagne di generazione dei lead su Facebook. Le persone compilano un modulo per esprimere interesse per un prodotto o un servizio, in modo che l&#39;azienda possa seguirli. L’integrazione di Marketo con gli Annunci lead di Facebook acquisisce automaticamente le informazioni fornite da un lead all’interno del modulo Annuncio lead. Le azioni di follow-up e le notifiche possono quindi essere automatizzate utilizzando il nuovo attivatore di annunci lead per la compilazione Facebook.

![](assets/image2016-1-11-10-3a20-3a39.png)

## [Pianificazione delle campagne Web (Personalizzazione in tempo reale)](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/schedule-a-web-campaign.md) {#web-real-time-personalization-campaign-scheduler}

Programmate in anticipo la campagna. Configurate una data di inizio e di fine per contenuti Web personalizzati e ripetete le campagne in giorni e ore specifici. Personalizzate la pianificazione per visualizzare la campagna in base all&#39;ora del visitatore Web o a un fuso orario selezionato.

![](assets/image2016-1-14-8-3a36-3a36.png)
