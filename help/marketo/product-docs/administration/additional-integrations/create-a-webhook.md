---
unique-page-id: 2360360
description: Crea un webhook in Admin per chiamare servizi web di terze parti per SMS, dati personali e altro ancora.
title: Crea un  [!DNL Webhook]
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
feature: Administration, Webhooks
TQID: https://experienceleague.adobe.com/O4xw1wSvFeTJ2xqZn4Eo7JbrUBQQmKcl7mvLkduFXGc
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2: id: fc9b09fe-b844-4544-887b-e420c3b82065
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 202
ht-degree: 3%

---

# Crea un [!DNL Webhook] {#create-a-webhook}

Utilizza [!DNL Webhooks] per sfruttare i servizi Web di terze parti per inviare messaggi di testo, espandere i dati personali e altro ancora.

1. Passa alla schermata **[!UICONTROL Admin]**.

   ![](assets/create-a-webhook-1.png)

1. Fai clic su **[!UICONTROL Webhooks]**.

   ![](assets/create-a-webhook-2.png)

1. Fai clic su **[!UICONTROL New Webhook]**.

   ![](assets/create-a-webhook-3.png)

1. Assegna un nome e configura [!DNL Webhook].

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >Questo spesso include l’immissione delle credenziali del servizio di terze parti come parametro URL o nel modello POST.

   * **[!UICONTROL URL]**: immettere l&#39;URL utilizzato nella richiesta al servizio Web. Per inserire nella richiesta un token, ad esempio l&#39;indirizzo di posta elettronica della persona (**`{{lead.Email Address}}`**), fare clic su **[!UICONTROL Insert Token]**.

   * **[!UICONTROL Template]**: se desideri trasmettere le informazioni nel corpo della richiesta, immetti tramite il modello di payload. Modelli consentiti per i seguenti tipi di richieste: POST, DELETE, PATCH o PUT. Puoi utilizzare formati di dati come JSON o XML. Per inserire un token nel modello, fare clic su **[!UICONTROL Insert Token]**.

   * **[!UICONTROL Request Token Encoding]**: se i valori del token includono caratteri speciali (ad esempio una e commerciale, &#39;&amp;&#39;), indicare il formato della richiesta (**JSON** o **Form/Url**).

   * **[!UICONTROL Response type]**: selezionare il formato della risposta ricevuta dal servizio (**JSON** o **XML**).

   * **[!UICONTROL Request Type]**: selezionare il metodo HTTP da utilizzare (DELETE, GET, PATCH, POST, PUT).

1. Fai clic su **[!UICONTROL Create]**.

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>Ulteriori informazioni sono disponibili nella sessione di approfondimento [[!DNL Webhooks]](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/webhooks/webhooks){target="_blank"}.
