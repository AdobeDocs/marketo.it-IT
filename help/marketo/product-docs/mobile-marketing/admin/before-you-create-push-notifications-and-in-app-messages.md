---
unique-page-id: 11376159
description: Prima di creare notifiche push e messaggi in-app - Documenti Marketo - Documentazione del prodotto
title: Prima di creare notifiche push e messaggi in-app
exl-id: c7e24338-387b-4c6f-bb29-7f7e6a1a7de5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# Prima di creare notifiche push e messaggi in-app {#before-you-create-push-notifications-and-in-app-messages}

La creazione di notifiche push e messaggi in-app non è difficile, ma è necessario disporre di tutto per poter iniziare. Gli sviluppatori di app mobili e amministratori di Marketo devono seguire i passaggi seguenti per preparare le integrazioni necessarie.

1. Innanzitutto, l’amministratore di Marketo [aggiunge un’app mobile](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md).

1. L’amministratore di Marketo [invia uno snippet di codice allo sviluppatore](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md).

1. Lo sviluppatore scarica l’SDK e include snippet e altri metodi, per [Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android/) o [iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/).

1. Per impostazione predefinita, i messaggi in-app vengono attivati all’apertura dell’app. Se desideri attivare i messaggi per altri eventi, ad esempio quando viene visualizzata una pagina particolare o viene premuto un pulsante specifico, lo sviluppatore deve aggiungere eventi personalizzati al codice (vedi [Eventi personalizzati per i messaggi in-app](#CustomEvents) qui sotto).

1. Lo sviluppatore [genera la chiave API server e il numero di progetto per Android](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/) o [certificazione e password per iOS](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/) e lo invia all&#39;amministratore di Marketo.

1. L’amministratore di Marketo configura l’accesso alle notifiche push [con la chiave API server (Android)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md) o [con il certificato (iOS)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md).

>[!TIP]
>
>È facile per un amministratore di Marketo verificare se la configurazione push è verificata. Vai e basta [qui](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md).

## Eventi personalizzati per i messaggi in-app {#custom-events-for-in-app-messages}

Per la messaggistica in-app, l’attivatore di visualizzazione è impostato su **Apri app** per impostazione predefinita. Se desideri utilizzare eventi personalizzati per attivare la visualizzazione dei messaggi in-app (ad esempio, **Clic Aggiungi al carrello**, **Pagina Visualizzazioni**), crea un elenco di eventi desiderati e assegnalo allo sviluppatore di app mobili. Lo sviluppatore aggiungerà quindi gli eventi personalizzati nel codice. Una volta approvati, vengono visualizzati come attivatori di visualizzazione durante la configurazione del pubblico. **Attenzione**: Il completamento del processo di approvazione della codifica degli eventi personalizzati potrebbe richiedere del tempo.

Dopo aver completato tutta la preparazione per i messaggi in-app e le notifiche push, è ora di iniziare!

>[!MORELIKETHIS]
>
>* [Creare un messaggio in-app](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
>
>* [Creare una notifica push](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)

