---
unique-page-id: 1900573
description: Aggiungere un token di sistema come collegamento in un’e-mail - Marketo Docs - Documentazione del prodotto
title: Aggiungere un token di sistema come collegamento in un’e-mail
exl-id: 9156be24-18ae-44ea-96e5-a6257ff29b46
source-git-commit: 65caed388ac33fc9f3142102343fe43ebc186e6e
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Aggiungere un token di sistema come collegamento in un&#39;e-mail {#add-a-system-token-as-a-link-in-an-email}

Puoi utilizzare questi token di sistema per personalizzare la posizione dei collegamenti speciali nelle e-mail.

I seguenti token possono essere utilizzati come collegamenti in un modello e-mail o e-mail:

* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

>[!NOTE]
>
>È possibile fare clic su questi token **non** a meno che non si trovi all’interno di un collegamento di ancoraggio. Inoltre, possono **non** essere incorporati in un My Token.

Ecco come aggiungerli a un’e-mail:

1. Trova e seleziona il tuo messaggio e-mail, quindi fai clic su **Modifica bozza**.

   ![](assets/one-1.png)

1. Fare doppio clic in un’area modificabile.

   ![](assets/two-1.png)

1. Evidenziare il testo da convertire in un collegamento che avrà il token e fare clic sul pulsante **Inserisci/Modifica collegamento**.

   ![](assets/three-1.png)

1. Inserisci il token nell’URL del collegamento e fai clic su **Inserisci**.

   ![](assets/four-1.png)

   >[!TIP]
   >
   >Copia/Incolla il token desiderato: **`{{system.forwardToFriendLink}}`** o **`{{system.unsubscribeLink}}`** o **`{{system.viewAsWebpageLink}}`**

1. Fare clic su **Salva**.

   ![](assets/image2014-9-17-22-3a12-3a17.png)

>[!IMPORTANT]
>
>Se utilizzi questo approccio per aggiungere il token di sistema &quot;viewAsWebpageLink&quot;, puoi **non** ignorarlo utilizzando i token. Utilizza invece [Aggiungi una visualizzazione come collegamento di pagina web a un approccio Email](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) che ti consente di ignorare &quot;viewAsWebPageLink&quot; utilizzando i token.

>[!NOTE]
>
>Non dimenticare di [approvare l&#39;e-mail](/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md) al termine.

Ben fatto! Ora sai come aggiungere un token di sistema come collegamento in un’e-mail.
