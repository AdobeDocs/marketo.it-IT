---
unique-page-id: 2360360
description: Creare un Webhook - Marketo Docs - Documentazione del prodotto
title: Creare un Webhook
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
source-git-commit: 5f509a7aa27692e54bf129b94c657aff0f645f2b
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 0%

---

# Creare un Webhook {#create-a-webhook}

Utilizza i webhook per sfruttare i servizi web di terze parti per inviare messaggi di testo, espandere i dati delle persone e altro ancora.

>[!AVAILABILITY]
>
>Non tutti i clienti hanno acquistato questa funzionalità. Contatta il tuo rappresentante commerciale per i dettagli.

1. Vai a **Amministratore** area.

   ![](assets/create-a-webhook-1.png)

1. Fai clic su **Webhook**.

   ![](assets/create-a-webhook-2.png)

1. Fai clic su **Nuovo Webhook**.

   ![](assets/create-a-webhook-3.png)

1. Denomina e configura il tuo webhook.

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >Ciò include spesso l&#39;immissione delle credenziali del servizio di terze parti come parametro URL o nel modello POST.

   * **URL**: Immetti l’URL utilizzato nella richiesta al servizio Web. Per inserire un token, ad esempio l’indirizzo e-mail della persona (**`{{lead.Email Address}}`**), nella richiesta fai clic su **Inserisci token**.

   * **Modello**: Se si desidera trasmettere informazioni nel corpo di POST, inserire il modello. Utilizza qualsiasi formato di dati che supporti HTTP POST, inclusi XML, JSON o SOAP. Per inserire un token nel modello, fai clic su **Inserisci token**.

   * **Richiedi codifica token**: Se i valori del token includono caratteri speciali (ad esempio una e commerciale, &quot;&amp;&quot;), indica il formato della richiesta (**JSON** o **Modulo/Url**).

   * **Tipo di risposta**: Seleziona il formato della risposta ricevuta dal servizio (**JSON** o **XML**).

   * **Tipo di richiesta**: Selezionare il metodo HTTP da utilizzare (DELETE, GET, PATCH, POST, PUT).

1. Fai clic su **Crea**.

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>Ulteriori informazioni nel [webhook](https://developers.marketo.com/documentation/webhooks/) immersione profonda.
