---
unique-page-id: 1900577
description: Creare un token di script e-mail - Documenti Marketo - Documentazione prodotto
title: Creare un token di script e-mail
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---


# Creare un token di script e-mail {#create-an-email-script-token}

Per gli sviluppatori avanzati, nelle e-mail puoi utilizzare [script Velocity](https://velocity.apache.org/engine/1.7/user-guide.html). Ecco come farlo.

1. Andate a **Marketing Activities**.

   ![](assets/ma.png)

1. Trovate e selezionate un programma (Evento, Predefinito, Coinvolgimento, ecc.).

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. Nella scheda **My Tokens** (Token personali), trascinare un token **Email Script**.

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. Assegnate un nome al token di script e **fate clic per modificare il contenuto**.

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. Utilizzate la struttura ad albero a destra per trascinare i token **Persona, Opportunità** o **Oggetto personalizzato**.

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >Quando si accede a un array (opportunità o oggetto personalizzato), l&#39;utente è limitato ai 10 elementi più recenti associati alla persona.

1. Il token viene selezionato/attivo dopo che è stato trascinato nell&#39;editor di script.

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >Se digitate dei token a forma libera, verificate di controllare/attivare tutti i token corrispondenti nella struttura ad albero oppure questi verranno trattati come testo normale e non funzioneranno.

1. Scrivi il tuo script in Velocity. Di seguito sono riportate alcune risorse utili:

   * [Documentazione sugli script e-mail per sviluppatori Marketo](https://developers.marketo.com/email-scripting/)
   * [Guida utente Velocity](https://velocity.apache.org/engine/devel/user-guide.html)
   * [Guida di riferimento della velocità](https://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Javadoc strumenti Velocity](https://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. Una volta completato lo script, fare clic su **Salva**.

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. Fare clic su **Salva** una volta.

   ![](assets/image2014-9-17-22-3a23-3a13.png)

Ora puoi usare questo token nelle e-mail. Lo script verrà eseguito ogni volta che viene inviato un messaggio e-mail.

>[!MORELIKETHIS]
>
>[Aggiungere un token di script e-mail al messaggio e-mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-an-email-script-token-to-your-email.md)
