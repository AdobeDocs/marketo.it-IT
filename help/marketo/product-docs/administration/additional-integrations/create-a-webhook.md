---
unique-page-id: 2360360
description: Creare un Webhook - Documenti Marketo - Documentazione prodotto
title: Creare un Webhook
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 0%

---


# Creare un Webhook {#create-a-webhook}

Utilizza i webhooks per sfruttare i servizi Web di terze parti per inviare messaggi di testo, espandere i dati delle persone e altro ancora.

>[!AVAILABILITY]
>
>Non tutti i clienti hanno acquistato questa funzionalità. Per informazioni, contattate il rappresentante commerciale.

1. Accedete a **Admin** e fate clic su **Webhooks**.

   ![](assets/image2014-9-24-14-3a52-3a57.png)

1. Fare clic su **Nuovo Webhook**.

   ![](assets/image2014-9-24-14-3a53-3a9.png)

1. Denominate e configurate il webhook.

   ![](assets/image2014-9-24-14-3a53-3a19.png)

   >[!NOTE]
   >
   >Ciò spesso include l&#39;immissione delle credenziali del servizio di terze parti come parametro URL o nel modello POST.

   * **URL**: Inserite l’URL che utilizzate per POST della richiesta al servizio Web. Per inserire un token, ad esempio l&#39;indirizzo e-mail della persona (**`{{lead.Email Address}}`**), nella richiesta fare clic su **Inserisci token**.

   * **Modello**: Se desiderate trasmettere le informazioni nel corpo del POST, inserite il modello. Utilizzate qualsiasi formato di dati che supporti POST HTTP, inclusi XML, JSON o SOAP. Per inserire un token nel modello, fare clic su **Inserisci token**.

   * **Richiedi codifica** token: Se i valori del token includono caratteri speciali (ad esempio una e commerciale, &#39;&amp;&#39;), indicate il formato della richiesta (**** JSONo  **Form/Url**).

   * **Tipo** di risposta: Selezionate il formato della risposta ricevuta dal servizio (**** JSONo  **XML**).

   Fate clic su Crea.

   ![](assets/image2014-9-24-14-3a53-3a35.png)

>[!NOTE]
>
>Ulteriori informazioni sono disponibili nella [webhooks](https://developers.marketo.com/documentation/webhooks/) immersione profonda.
