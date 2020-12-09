---
unique-page-id: 1900577
description: Creare un token di script e-mail - Documenti Marketo - Documentazione prodotto
title: Creare un token di script e-mail
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---


# Creare un token di script e-mail {#create-an-email-script-token}

Per gli sviluppatori avanzati, potete utilizzare gli script [](http://velocity.apache.org/engine/1.7/user-guide.html) Velocity nelle e-mail. Ecco come farlo.

1. Vai a Attività **** di marketing.

   ![](assets/ma.png)

1. Trovate e selezionate un programma (Evento, Predefinito, Coinvolgimento, ecc.).

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. Nella scheda **Token** personali trascinare un token script **** e-mail.

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. Assegnate un nome al token script e-mail e **fate clic per modificarne** il contenuto.

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. Utilizzate la struttura ad albero a destra per trascinare i token **Persona, Opportunità** o Oggetto **** personalizzato.

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >Quando si accede a un array (opportunità o oggetto personalizzato), l&#39;utente è limitato ai 10 elementi più recenti associati alla persona.

1. Il token viene selezionato/attivo dopo che è stato trascinato nell&#39;editor di script.

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >**Promemoria**
   >
   >
   >Se digitate dei token a forma libera, verificate di controllare/attivare tutti i token corrispondenti nella struttura ad albero oppure questi verranno trattati come testo normale e non funzioneranno.

1. Scrivi il tuo script in Velocity. Di seguito sono riportate alcune risorse utili:

   * [Documentazione sugli script e-mail per sviluppatori Marketo](http://developers.marketo.com/email-scripting/)
   * [Guida utente Velocity](http://velocity.apache.org/engine/devel/user-guide.html)
   * [Guida di riferimento della velocità](http://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Javadoc strumenti Velocity](http://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. Al termine dello script, fare clic su **Salva**.

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. Fai clic su **Salva** una volta di più.

   ![](assets/image2014-9-17-22-3a23-3a13.png)

Ora puoi usare questo token nelle e-mail. Lo script verrà eseguito ogni volta che viene inviato un messaggio e-mail.

>[!MORELIKETHIS]
>
>* [Aggiungere un token di script e-mail al messaggio e-mail](add-an-email-script-token-to-your-email.md)

>



