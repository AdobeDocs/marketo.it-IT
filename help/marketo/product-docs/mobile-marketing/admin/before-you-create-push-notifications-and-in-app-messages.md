---
unique-page-id: 11376159
description: Prima di creare notifiche push e messaggi in-app - Documenti Marketo - Documentazione prodotto
title: Prima di creare notifiche push e messaggi in-app
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 0%

---


# Prima di creare notifiche push e messaggi in-app {#before-you-create-push-notifications-and-in-app-messages}

La creazione di notifiche push e messaggi in-app non è difficile, ma è necessario avere tutto pronto prima di iniziare. L&#39;amministratore di marketing e lo sviluppatore di app mobili devono seguire i passaggi indicati di seguito per preparare le integrazioni necessarie.

1. Innanzitutto, l&#39;amministratore di Marketing [aggiunge un&#39;app mobile](add-a-mobile-app.md)
1. L&#39;amministratore di marketing, quindi [invia uno snippet di codice allo sviluppatore](send-sdk-code-to-a-developer.md)
1. Lo sviluppatore scarica l&#39;SDK, e include snippet e altri metodi, per [Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android/) o [iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/)
1. Per impostazione predefinita, i messaggi in-app vengono attivati all&#39;apertura dell&#39;app. Se si desidera attivare messaggi per altri eventi, ad esempio quando viene visualizzata una particolare pagina o viene premuto un pulsante specifico, lo sviluppatore deve aggiungere al codice eventi personalizzati (vedere [Eventi personalizzati per i messaggi in-app](#CustomEvents) sotto)
1. Lo sviluppatore [genera la chiave Server API e il numero del progetto per Android](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/) o [la certificazione e la password per iOS](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/) e la invia all&#39;amministratore di Marketo
1. L&#39;amministratore di marketing configura l&#39;accesso alla notifica push [con la chiave API server (Android)](configure-mobile-app-android-push-access.md) o [con il certificato (iOS)](configure-mobile-app-ios-push-access.md)

>[!TIP]
>
>È facile per un amministratore di marketing verificare se la configurazione push è verificata. Basta andare [qui](verify-push-configuration.md).

## Eventi personalizzati per messaggi in-app {#custom-events-for-in-app-messages}

Per la messaggistica in-app, l&#39;attivatore dello schermo è impostato su **App Open** per impostazione predefinita. Se desiderate utilizzare eventi personalizzati per attivare la visualizzazione dei messaggi in-app (ad esempio, **Clic su Aggiungi al carrello**, **Visualizzazioni pagina Impostazioni**), create un elenco degli eventi desiderati e distribuitelo allo sviluppatore di app mobili. Lo sviluppatore aggiungerà quindi gli eventi personalizzati nel codice. Una volta approvati, vengono visualizzati come attivatori di visualizzazione durante la configurazione del pubblico. **Attenzione**: Il processo di approvazione della codifica dell&#39;evento personalizzato potrebbe richiedere del tempo.

Dopo aver preparato tutti i messaggi in-app e le notifiche push, è ora di iniziare!

>[!MORELIKETHIS]
>
>* [Creare un messaggio in-app](https://docs.marketo.com/display/docs/create+an+in-app+message)
   >
   >
* [Creare una notifica push](../../../product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)

>



