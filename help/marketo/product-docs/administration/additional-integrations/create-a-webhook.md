---
unique-page-id: 2360360
description: Creazione di un documento di Marketo  [!DNL Webhook]  - Documentazione del prodotto
title: Crea un  [!DNL Webhook]
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
feature: Administration, Webhooks
source-git-commit: 23a7b8cb1cd07c0194c08d30218602a52d03df5b
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---

# Crea un [!DNL Webhook] {#create-a-webhook}

Utilizza [!DNL Webhooks] per sfruttare i servizi Web di terze parti per inviare messaggi di testo, espandere i dati personali e altro ancora.

1. Vai all&#39;area **[!UICONTROL Amministratore]**.

   ![](assets/create-a-webhook-1.png)

1. Fai clic su **[!UICONTROL Webhook]**.

   ![](assets/create-a-webhook-2.png)

1. Fai clic su **[!UICONTROL Nuovo webhook]**.

   ![](assets/create-a-webhook-3.png)

1. Assegna un nome e configura [!DNL Webhook].

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >Questo spesso include l’immissione delle credenziali del servizio di terze parti come parametro URL o nel modello POST.

   * **[!UICONTROL URL]**: immetti l&#39;URL utilizzato nella richiesta al servizio Web. Per inserire un token, ad esempio l&#39;indirizzo e-mail della persona (**`{{lead.Email Address}}`**), nella richiesta, fai clic su **[!UICONTROL Inserisci token]**.

   * **[!UICONTROL Modello]**: se desideri trasmettere informazioni nel corpo della richiesta, immetti tramite il modello di payload. Modelli consentiti per i seguenti tipi di richiesta: POST, DELETE, PATCH o PUT. Puoi utilizzare formati di dati come JSON o XML. Per inserire un token nel modello, fai clic su **[!UICONTROL Inserisci token]**.

   * **[!UICONTROL Codifica token richiesta]**: se i valori del token includono caratteri speciali (ad esempio una e commerciale, &#39;&amp;&#39;), indicare il formato della richiesta (**JSON** o **Form/Url**).

   * **[!UICONTROL Tipo di risposta]**: selezionare il formato della risposta ricevuta dal servizio (**JSON** o **XML**).

   * **[!UICONTROL Tipo di richiesta]**: selezionare il metodo HTTP da utilizzare (DELETE, GET, PATCH, POST, PUT).

1. Fai clic su **[!UICONTROL Crea]**.

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>Ulteriori informazioni sono disponibili nella sessione di approfondimento [[!DNL Webhooks]](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/webhooks/webhooks){target="_blank"}.
