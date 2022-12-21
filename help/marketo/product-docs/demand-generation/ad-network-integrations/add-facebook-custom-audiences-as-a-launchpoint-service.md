---
unique-page-id: 4720257
description: Aggiungere tipi di pubblico personalizzati di Facebook as a LaunchPoint Service - Documentazione di Marketo - Documentazione del prodotto
title: Aggiungere tipi di pubblico personalizzati di Facebook come servizio LaunchPoint
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---

# Aggiungere tipi di pubblico personalizzati di Facebook come servizio LaunchPoint {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Con questa integrazione è possibile inviare dati sul pubblico da elenchi statici e avanzati di Marketo a Facebook da utilizzare come tipi di pubblico personalizzati nelle campagne pubblicitarie Facebook. Ecco come configurarlo.

1. Vai a Marketo **Amministratore**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Vai a **LaunchPoint**, fai clic su **Nuovo** e seleziona **Nuovo servizio**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Inserisci un **Nome visualizzato** per il servizio e seleziona la **Tipi di pubblico personalizzati facebook** dal servizio **Servizio** a discesa.

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. Apri una nuova scheda nello stesso browser e vai a [facebook.com](https://www.facebook.com/). Accedi a Facebook utilizzando l’account che desideri utilizzare per l’integrazione.

   >[!CAUTION]
   >
   >Affinché Marketo possa inviare tipi di pubblico tra più account Ad Manager, l’utente Facebook autorizzato nei seguenti passaggi deve avere accesso a *tutto* di tali conti.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. Dopo aver effettuato l’accesso a Facebook, torna a Marketo. Fai clic su **Autorizzare**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >You _deve_ utilizza un account Facebook Business Manager per il corretto funzionamento dell’integrazione con tipi di pubblico personalizzati. Per informazioni su come impostare un account Business Manager, consulta [Guida di facebook](https://www.facebook.com/business/help/1710077379203657).

1. Se richiesto, fai clic su **OK** per accettare l’installazione dell’app Marketo in Facebook.

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Ora sei autorizzato! Seleziona una modalità corrispondente e fai clic su **Crea**.

   >[!NOTE]
   >
   >**Corrispondenza di base** utilizza solo indirizzi e-mail. **Corrispondenza avanzata** utilizza sette campi aggiuntivi, che aumentano il tasso di corrispondenza, per una maggiore conversione. Tuttavia, se l&#39;informativa sulla privacy dell&#39;azienda non consente la condivisione di campi aggiuntivi o se i dati non li includono, selezionare Corrispondenza di base.

   ![](assets/fb-custom-adv-matching-hands.png)

   Ottimo lavoro! Ora puoi passare a qualsiasi elenco statico o avanzato in Marketo e inviare i dati sul pubblico a Facebook.

   >[!CAUTION]
   >
   >Oh, prima di andare, assicurati di [Accettare i termini personalizzati del pubblico di Facebook](https://www.facebook.com/ads/manage/customaudiences/tos.php) nel tuo account Facebook! Senza questo intervento, gli aggiornamenti del pubblico non riusciranno.

>[!MORELIKETHIS]
>
>* [Creare un pubblico personalizzato in Facebook](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
>
>* [Imposta annunci lead Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)

