---
unique-page-id: 4720257
description: Scopri come aggiungere tipi di pubblico personalizzati di Facebook come servizio LaunchPoint. Inviare elenchi Marketo a Facebook per utilizzarli come tipi di pubblico personalizzati nelle campagne pubblicitarie.
title: 'Aggiungi [!DNL Facebook] tipi di pubblico personalizzati come servizio [!DNL LaunchPoint] '
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
feature: Integrations
TQID: https://experienceleague.adobe.com/oqtZ6Dbnnj8FgpPOLwZbLrmTmmex5spooX0VuJeugT0
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
topic_v2:
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 294
ht-degree: 1%

---

# Aggiungi [!DNL Facebook] tipi di pubblico personalizzati come servizio [!DNL LaunchPoint] {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Con questa integrazione è possibile inviare dati di pubblico da elenchi statici e avanzati di Marketo a [!DNL Facebook] per utilizzarli come tipi di pubblico personalizzati nelle campagne pubblicitarie [!DNL Facebook]. Segui questi passaggi per configurarlo.

1. Passare a Marketo **[!UICONTROL Admin]**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Vai a **[!UICONTROL LaunchPoint]**, fai clic su **[!UICONTROL New]** e seleziona **[!UICONTROL New Service]**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Immetti **[!UICONTROL Display Name]** per il servizio e seleziona il servizio **[!UICONTROL Facebook Custom Audiences]** dal menu a discesa **[!UICONTROL Service]**.

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. Apri una nuova scheda nello stesso browser e passa a [facebook.com](https://www.facebook.com/). Accedere a [!DNL Facebook] utilizzando l&#39;account che si desidera utilizzare per l&#39;integrazione.

   >[!CAUTION]
   >
   >Affinché Marketo possa inviare tipi di pubblico su più account di Ad Manager, l&#39;utente [!DNL Facebook] autorizzato nei passaggi seguenti deve avere accesso a *tutti* gli account.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. Dopo aver effettuato l&#39;accesso a [!DNL Facebook], tornare a Marketo. Fai clic su **[!UICONTROL Authorize]**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >*devi* utilizzare un account di [!DNL Facebook] Business Manager per il corretto funzionamento dell&#39;integrazione dei tipi di pubblico personalizzati. Per informazioni sulla configurazione di un account di Business Manager, consultare la [[!DNL Facebook] Guida](https://www.facebook.com/business/help/1710077379203657).

1. Se richiesto, fare clic su **[!UICONTROL OK]** per accettare l&#39;installazione dell&#39;app Marketo in [!DNL Facebook].

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Ora sei autorizzato. Selezionare una modalità corrispondente e fare clic su **[!UICONTROL Create]**.

   >[!NOTE]
   >
   >**[!UICONTROL Basic Matching]** utilizza solo indirizzi e-mail. **[!UICONTROL Advanced Matching]** utilizza sette campi aggiuntivi, che aumentano il tasso di corrispondenza, per una maggiore conversione. Tuttavia, se l&#39;informativa sulla privacy della tua azienda non consente la condivisione di campi aggiuntivi o se i tuoi dati non li includono, seleziona [!UICONTROL Basic Matching].

   ![](assets/fb-custom-adv-matching-hands.png)

   Ora puoi passare a qualsiasi elenco statico o avanzato in Marketo e inviare dati sul pubblico a [!DNL Facebook].

   >[!CAUTION]
   >
   >Prima di utilizzare la tua integrazione, [Accetta i termini dei tipi di pubblico personalizzati di  [!DNL Facebook]](https://www.facebook.com/ads/manage/customaudiences/tos.php) nel tuo account [!DNL Facebook]. In caso contrario, gli aggiornamenti del pubblico non riusciranno.

>[!MORELIKETHIS]
>
>* [Crea un pubblico personalizzato in [!DNL Facebook]](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
>
>* [Configura [!DNL Facebook] Annunci lead](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)
