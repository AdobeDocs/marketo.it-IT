---
unique-page-id: 2360360
description: Creazione di un documento di Marketo  [!DNL Webhook]  - Documentazione del prodotto
title: Crea un  [!DNL Webhook]
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
feature: Administration, Webhooks
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '181'
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
