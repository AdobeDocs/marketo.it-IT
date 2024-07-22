---
unique-page-id: 1900573
description: Aggiungere un token di sistema come collegamento in un messaggio e-mail - Documentazione di Marketo - Documentazione del prodotto
title: Aggiungere un token di sistema come collegamento in un messaggio e-mail
exl-id: 9156be24-18ae-44ea-96e5-a6257ff29b46
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# Aggiungere un token di sistema come collegamento in un messaggio e-mail {#add-a-system-token-as-a-link-in-an-email}

Puoi utilizzare questi token di sistema per personalizzare la posizione dei collegamenti speciali nelle e-mail.

I seguenti token possono essere utilizzati come collegamenti in un modello e-mail o e-mail:

* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

>[!NOTE]
>
>Questi token saranno **non** cliccabili a meno che non siano all&#39;interno di un collegamento di ancoraggio. Inoltre, possono **non** essere incorporati in un My Token.

Ecco come aggiungerli a un’e-mail:

1. Trova e seleziona il tuo indirizzo e-mail, quindi fai clic su **Modifica bozza**.

   ![](assets/one-1.png)

1. Fare doppio clic in un&#39;area modificabile.

   ![](assets/two-1.png)

1. Evidenziare il testo da convertire in un collegamento che avrà il token e fare clic sul pulsante **Inserisci/Modifica collegamento**.

   ![](assets/three-1.png)

1. Immettere il token nell&#39;URL del collegamento e fare clic su **Inserisci**.

   ![](assets/four-1.png)

   >[!TIP]
   >
   >Copiare/incollare il token desiderato: **`{{system.forwardToFriendLink}}`** o **`{{system.unsubscribeLink}}`** o **`{{system.viewAsWebpageLink}}`**

1. Fai clic su **Salva**.

   ![](assets/image2014-9-17-22-3a12-3a17.png)

>[!IMPORTANT]
>
>Se si utilizza questo approccio per aggiungere il token di sistema &quot;viewAsWebpageLink&quot;, è possibile **non** eseguirne l&#39;override utilizzando i token. Utilizzare invece [Aggiungi un collegamento Visualizza come pagina Web a un indirizzo e-mail](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) che consente di ignorare &quot;viewAsWebPageLink&quot; utilizzando i token.

>[!NOTE]
>
>Al termine, non dimenticare di [approvare l&#39;e-mail](/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md).

Ben fatto! Ora sai come aggiungere un token di sistema come collegamento in un’e-mail.
