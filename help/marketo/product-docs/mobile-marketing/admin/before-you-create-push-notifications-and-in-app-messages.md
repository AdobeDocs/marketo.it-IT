---
unique-page-id: 11376159
description: Prima di creare notifiche push e messaggi in-app - Documenti Marketo - Documentazione del prodotto
title: Prima di creare notifiche push e messaggi in-app
exl-id: c7e24338-387b-4c6f-bb29-7f7e6a1a7de5
feature: Mobile Marketing
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# Prima di creare notifiche push e messaggi in-app {#before-you-create-push-notifications-and-in-app-messages}

La creazione di notifiche push e messaggi in-app non è difficile, ma è necessario avere tutto pronto prima di poter iniziare. L’amministratore di Marketo e lo sviluppatore di app mobili devono seguire i passaggi seguenti per preparare le integrazioni necessarie.

1. In primo luogo, l’amministratore di Marketo [aggiunge un’app mobile](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md).

1. L’amministratore di Marketo [invia un frammento di codice allo sviluppatore](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md).

1. Lo sviluppatore scarica l’SDK e include snippet e altri metodi per [Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android/) o [iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/).

1. Per impostazione predefinita, i messaggi in-app vengono attivati all’apertura dell’app. Se desideri attivare messaggi per altri eventi, ad esempio quando viene visualizzata una pagina particolare o viene premuto un pulsante specifico, lo sviluppatore deve aggiungere eventi personalizzati al codice (vedi [Eventi personalizzati per messaggi in-app](#CustomEvents) di seguito).

1. Sviluppatore [genera la chiave API server e il numero del progetto per Android](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/) o [la certificazione e la password per iOS](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/) e lo invia all’amministratore di Marketo.

1. L’amministratore di Marketo configura l’accesso alle notifiche push [con la chiave API del server (Android)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md) o [con il certificato (iOS)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md).

>[!TIP]
>
>Per un amministratore di Marketo è facile verificare se la configurazione push è stata verificata. Vai [qui](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md).

## Eventi personalizzati per messaggi in-app {#custom-events-for-in-app-messages}

Per i messaggi in-app, il trigger di visualizzazione è impostato su **Apertura app** per impostazione predefinita. Se desideri utilizzare eventi personalizzati per attivare la visualizzazione dei messaggi in-app (ad esempio, **Clic su Aggiungi al carrello**, **Pagina Impostazioni visualizzazioni**), crea un elenco di eventi desiderati e passalo allo sviluppatore di app mobili. Lo sviluppatore aggiungerà quindi gli eventi personalizzati nel codice. Una volta approvate, vengono visualizzate come attivatori di visualizzazione durante la configurazione del pubblico. **Attenzione**: il completamento del processo di approvazione della codifica degli eventi personalizzata potrebbe richiedere un po’ di tempo.

Dopo aver completato tutta la preparazione per i messaggi in-app e le notifiche push, è ora di iniziare.

>[!MORELIKETHIS]
>
>* [Creare un messaggio in-app](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
>
>* [Creare una notifica push](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)
