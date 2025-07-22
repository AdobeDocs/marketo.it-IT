---
unique-page-id: 11376159
description: Prima di creare notifiche push e messaggi in-app - Documenti Marketo - Documentazione del prodotto
title: Prima di creare notifiche push e messaggi in-app
exl-id: c7e24338-387b-4c6f-bb29-7f7e6a1a7de5
feature: Mobile Marketing
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Prima di creare notifiche push e messaggi in-app {#before-you-create-push-notifications-and-in-app-messages}

La creazione di notifiche push e messaggi in-app non è difficile, ma è necessario avere tutto pronto prima di poter iniziare. L’amministratore di Marketo e lo sviluppatore di app mobili devono seguire i passaggi seguenti per preparare le integrazioni necessarie.

1. L&#39;amministratore di Marketo [aggiunge innanzitutto un&#39;app mobile](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md).

1. L&#39;amministratore di Marketo [invia quindi uno snippet di codice allo sviluppatore](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md).

1. Lo sviluppatore scarica SDK e include snippet e altri metodi per [Android](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android) o [iOS](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-ios).

1. Per impostazione predefinita, i messaggi in-app vengono attivati all’apertura dell’app. Se desideri attivare messaggi per altri eventi, ad esempio quando viene visualizzata una pagina particolare o viene premuto un pulsante specifico, lo sviluppatore deve aggiungere eventi personalizzati al codice (vedi [Eventi personalizzati per messaggi in-app](#CustomEvents) di seguito).

1. Lo sviluppatore [genera la chiave API server e il numero del progetto per Android](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android) o [la certificazione e la password per iOS](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/mobile/installation#install-marketo-sdk-on-ios) e la invia all&#39;amministratore Marketo.

1. L&#39;amministratore di Marketo configura l&#39;accesso alle notifiche push [con la chiave API del server (Android)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md) o [con il certificato (iOS)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md).

>[!TIP]
>
>Per un amministratore di Marketo è facile verificare se la configurazione push è stata verificata. Vai [qui](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md).

## Eventi personalizzati per messaggi in-app {#custom-events-for-in-app-messages}

Per i messaggi in-app, il trigger di visualizzazione è impostato su **[!UICONTROL App Open]** per impostazione predefinita. Se desideri utilizzare eventi personalizzati per attivare la visualizzazione dei messaggi in-app (ad esempio, **Clic Aggiungi al carrello**, **Pagina impostazioni visualizzazioni**), crea un elenco di eventi desiderati e passalo allo sviluppatore di app mobili. Lo sviluppatore aggiungerà quindi gli eventi personalizzati nel codice. Una volta approvate, vengono visualizzate come attivatori di visualizzazione durante la configurazione del pubblico. **Attenzione**: il completamento del processo di approvazione della codifica degli eventi personalizzata potrebbe richiedere del tempo.

Dopo aver completato tutta la preparazione per i messaggi in-app e le notifiche push, è ora di iniziare.

>[!MORELIKETHIS]
>
>* [Creare un messaggio in-app](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
>
>* [Creare una notifica push](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)
