---
unique-page-id: 4720257
description: Aggiungere audience personalizzate Facebook come servizio LaunchPoint - Documenti Marketo - Documentazione prodotto
title: Aggiungere audience personalizzate di Facebook come servizio LaunchPoint
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---


# Aggiungere audience personalizzate di Facebook come servizio LaunchPoint {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Con questa integrazione potete inviare i dati del pubblico da Marketo agli elenchi statici e smart a Facebook da utilizzare come audience personalizzata nelle campagne pubblicitarie di Facebook. Ecco come impostarlo.

1. Vai a Marketo **Admin**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Vai a **LaunchPoint**, fai clic su **New** e seleziona **New Service**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Immettete un **Nome visualizzato** per il servizio e selezionate il servizio **Personalizzato pubblico di Facebook** dal menu a discesa **Servizio**.

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. Aprite una nuova scheda nello stesso browser e passate a [facebook.com](https://www.facebook.com/). Effettuate l&#39;accesso a Facebook utilizzando l&#39;account che desiderate utilizzare per l&#39;integrazione.

   >[!CAUTION]
   >
   >Affinché Marketo possa inviare audience tra più account Ad Manager, l&#39;utente Facebook che autorizzi nei seguenti passaggi deve avere accesso a *all* di questi account.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. Dopo aver effettuato l&#39;accesso a Facebook, tornate a Marketo. Fare clic su **Autorizza**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >Per consentire il funzionamento dell&#39;integrazione dell&#39;audience personalizzata, _è necessario_ utilizzare un account Facebook Business Manager. Per informazioni su come impostare un account Business Manager, fare riferimento alla [Guida di Facebook](https://www.facebook.com/business/help/1710077379203657).

1. Se richiesto, fate clic su **OK** per accettare l&#39;installazione dell&#39;app Marketo in Facebook.

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Adesso sei autorizzato! Selezionare una modalità corrispondente e fare clic su **Crea**.

   >[!NOTE]
   >
   >**Basic** Matchingusa solo indirizzi e-mail. **Advanced** Matchingutilizza sette campi aggiuntivi, che aumentano il tasso di corrispondenza, per una maggiore conversione. Tuttavia, se l&#39;informativa sulla privacy dell&#39;azienda non consente la condivisione di campi aggiuntivi o se i dati non li includono, selezionare Corrispondenza di base.

   ![](assets/fb-custom-adv-matching-hands.png)

   Ottimo lavoro! Ora puoi passare a qualsiasi elenco statico o smart in Marketo e inviare i dati del pubblico a Facebook.

   >[!CAUTION]
   >
   >Oh, prima di andare, assicurati di [Accettare i termini di audience personalizzati di Facebook](https://www.facebook.com/ads/manage/customaudiences/tos.php) all&#39;interno del tuo account Facebook! Senza questo, gli aggiornamenti del pubblico non riusciranno.

>[!MORELIKETHIS]
>
>* [Creare un pubblico personalizzato in Facebook](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
   >
   >
* [Impostazione Di Annunci Lead Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)

