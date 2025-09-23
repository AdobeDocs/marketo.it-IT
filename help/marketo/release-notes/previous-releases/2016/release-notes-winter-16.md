---
unique-page-id: 10097199
description: Note sulla versione -Inverno '16 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Inverno '16
exl-id: 1e3b9207-27fe-47b1-b709-1306ac57b93b
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 1%

---

# Note sulla versione - Inverno 2016 {#release-notes-winter}

Le seguenti funzioni sono incluse nella versione invernale del &#39;16. Fai clic sui collegamenti del titolo per visualizzare articoli dettagliati per ciascuna funzione.

## [Filtro anonimo](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website/next-generation-munchkin-tracking-faq.md) {#is-anonymous-filter}

Il filtro È anonimo è stato rimosso per gli elenchi avanzati. Per informazioni dettagliate, consulta il documento [Domande frequenti sul tracciamento dei Munchkin di nuova generazione](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website/next-generation-munchkin-tracking-faq.md). Questa modifica non interessa il Web Personalization (RTP), che continua a identificare i visitatori anonimi e noti e a personalizzare i contenuti in tempo reale per tali visitatori.

## [Dashboard database](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md)  {#database-dashboard}

[!UICONTROL Lead Database] dispone di una dashboard di riepilogo aggiornata che include la dimensione totale del database delle persone, il numero di lead commerciabili e una suddivisione dei lead per le prime cinque origini.

![](assets/image2016-1-12-16-3a18-3a7.png)

## [Browser Microsoft Edge](/help/marketo/product-docs/administration/setup-administration/supported-browsers.md) {#microsoft-edge-browser}

[!DNL Microsoft Edge] è stato aggiunto all&#39;[elenco di browser](https://docs.marketo.com/display/public/DOCS/Supported+Browsers) supportati da Marketo.

## [Microsoft Outlook 2016](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md) {#microsoft-outlook}

[[!DNL Microsoft Outlook] 2016](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md) è ora supportato.

## [Inizio intestazione programma e-mail](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) {#email-program-head-start}

Utilizza [!UICONTROL Head Start] per indicare che l&#39;elaborazione per l&#39;invio deve avvenire in anticipo. Invece di qualificare i lead e preparare le e-mail all&#39;ora pianificata del programma, [!UICONTROL Head Start] assicura che queste attività vengano eseguite in anticipo. In questo modo, il pubblico inizierà a ricevere e-mail all’ora pianificata.

![](assets/image2016-1-11-15-3a38-3a3.png)

Per utilizzare questa funzione, il programma e-mail deve essere pianificato con almeno 12 ore di anticipo e l’elenco avanzato verrà bloccato 12 ore prima dell’invio.

![](assets/image2016-1-11-15-3a35-3a55.png)

>[!NOTE]
>
>Questa funzione verrà implementata gradualmente per una settimana dopo il rilascio della versione invernale del 16. Non è disponibile per l’utilizzo con campagne intelligenti o con l’API.

## [Miglioramenti al marketing per dispositivi mobili](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md) {#mobile-marketing-enhancements}

Supporto di **[!DNL PhoneGap]:** Offriamo ora il supporto di [!DNL PhoneGap] per la tua app mobile. [Ulteriori informazioni](https://developers.marketo.com/documentation/mobile/phonegap-plugin/).

**Supporto per le app sandbox**:

![](assets/image2016-1-12-10-3a47-3a13.png)

## [API programma](https://developers.marketo.com/documentation/programs/) {#program-api}

Crea, aggiorna e clona programmi tramite l’API REST. Ciò non include la creazione o l’aggiornamento di elenchi avanzati e campagne intelligenti all’interno di un programma.

## [Miglioramenti Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md) {#microsoft-dynamics-enhancements}

**[[!UICONTROL Sync Status]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md)**: Mantieni schede sulla velocità effettiva corrente e sul backlog del processo di sincronizzazione. Suddividilo per il numero di inserimenti e aggiornamenti per oggetto.

![](assets/pending-backog-cropped.png)

**[[!UICONTROL Notifications]](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md)**: ricevere notifiche per gli errori di sincronizzazione comuni, insieme a un elenco di lead che presentano tale errore.

![](assets/image2016-1-12-8-3a13-3a9.png)

## [Miglioramenti agli oggetti personalizzati](/help/marketo/product-docs/administration/marketo-custom-objects/create-marketo-custom-objects.md) {#custom-objects-enhancements}

È ora possibile creare relazioni molti-a-molti tra lead/account e un oggetto personalizzato utilizzando un oggetto intermedio con più campi di collegamento.

![](assets/image2016-1-11-12-3a59-3a59.png)

## [Annunci lead Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md) {#facebook-lead-ads}

[[!UICONTROL Facebook Lead ads]](https://www.facebook.com/business/a/lead-ads) sono un modo più diretto per un&#39;azienda di eseguire campagne di generazione di lead su [!DNL Facebook]. Le persone compilano un modulo per esprimere interesse per un prodotto o un servizio, in modo che l&#39;azienda possa seguirli. L&#39;integrazione di Marketo con [!UICONTROL Facebook Lead Ads] acquisisce automaticamente le informazioni fornite da un lead all&#39;interno del modulo Annuncio lead. Le azioni di completamento e le notifiche possono quindi essere automatizzate utilizzando il nuovo trigger [!UICONTROL Fills Out Facebook Lead Ads].

![](assets/image2016-1-11-10-3a20-3a39.png)

## [Utilità di pianificazione campagne Web (Real-Time Personalization)](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/schedule-a-web-campaign.md) {#web-real-time-personalization-campaign-scheduler}

Pianifica la campagna in anticipo. Imposta una data di inizio e una data di fine per i contenuti web personalizzati e per le campagne ripetute in giorni e ore specifici. Personalizza la pianificazione per visualizzare la campagna in base all’ora del visitatore web o al fuso orario selezionato.

![](assets/image2016-1-14-8-3a36-3a36.png)
