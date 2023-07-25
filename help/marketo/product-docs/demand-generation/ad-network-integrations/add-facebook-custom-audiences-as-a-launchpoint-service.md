---
unique-page-id: 4720257
description: Aggiungere tipi di pubblico personalizzati di Facebook come servizio LaunchPoint - Documentazione di Marketo - Documentazione del prodotto
title: Aggiungere tipi di pubblico personalizzati di Facebook come servizio LaunchPoint
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---

# Aggiungere tipi di pubblico personalizzati di Facebook come servizio LaunchPoint {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Con questa integrazione è possibile inviare dati di pubblico da elenchi statici e avanzati di Marketo a Facebook per utilizzarli come tipi di pubblico personalizzati nelle campagne Facebook Ad. Ecco come configurarlo.

1. Vai a Marketo **Amministratore**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Vai a **LaunchPoint**, fai clic su **Nuovo** e seleziona **Nuovo servizio**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Immetti un **Nome visualizzato** per il servizio e selezionare **Tipi di pubblico personalizzati facebook** servizio da **Servizio** a discesa.

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. Apri una nuova scheda nello stesso browser e vai a [facebook.com](https://www.facebook.com/). Accedi a Facebook utilizzando l’account che desideri utilizzare per l’integrazione.

   >[!CAUTION]
   >
   >Affinché Marketo possa inviare tipi di pubblico su più account di Ad Manager, l&#39;utente Facebook autorizzato nei passaggi seguenti deve avere accesso a *tutto* di questi conti.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. Dopo aver effettuato l’accesso a Facebook, torna a Marketo. Clic **Autorizza**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >Tu _deve_ utilizza un account Facebook Business Manager per il funzionamento dell’integrazione di tipi di pubblico personalizzati. Per informazioni sulla configurazione di un account Business Manager, fare riferimento a [Guida di facebook](https://www.facebook.com/business/help/1710077379203657).

1. Se richiesto, fare clic su **OK** per accettare l’installazione dell’app Marketo in Facebook.

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Ora sei autorizzato! Seleziona una modalità corrispondente e fai clic su **Crea**.

   >[!NOTE]
   >
   >**Corrispondenza di base** utilizza solo indirizzi e-mail. **Corrispondenza avanzata** utilizza sette campi aggiuntivi, che aumentano il tasso di corrispondenza, per una maggiore conversione. Tuttavia, se l’informativa sulla privacy della tua azienda non consente la condivisione di campi aggiuntivi o se i tuoi dati non li includono, seleziona Corrispondenza di base.

   ![](assets/fb-custom-adv-matching-hands.png)

   Ottimo lavoro! Ora puoi passare a qualsiasi elenco statico o avanzato in Marketo e inviare i dati sul pubblico a Facebook.

   >[!CAUTION]
   >
   >Oh, prima di andare, assicurati di [Accettare i termini dei tipi di pubblico personalizzati di Facebook](https://www.facebook.com/ads/manage/customaudiences/tos.php) nel tuo account Facebook. In caso contrario, gli aggiornamenti del pubblico non riusciranno.

>[!MORELIKETHIS]
>
>* [Creare un pubblico personalizzato in Facebook](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
>
>* [Configurazione annunci lead Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)
