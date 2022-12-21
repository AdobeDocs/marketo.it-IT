---
unique-page-id: 1900577
description: Creare un token di script e-mail - Documenti Marketo - Documentazione del prodotto
title: Creare un token di script e-mail
exl-id: c7f8c3e0-6d64-4115-b9b6-261576360ba1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# Creare un token di script e-mail {#create-an-email-script-token}

Per gli sviluppatori avanzati, puoi utilizzare [Script Velocity](https://velocity.apache.org/engine/1.7/user-guide.html) nelle e-mail. Ecco come farlo.

1. Vai a **Attività di marketing**.

   ![](assets/ma.png)

1. Trova e seleziona qualsiasi programma (Evento, Predefinito o Coinvolgimento, ecc.).

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. Sotto la **Token personali** trascina un **Script e-mail** token.

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. Denomina il token di script e-mail e **fare clic per modificare** il suo contenuto.

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. Utilizza l&#39;albero a destra per trascinare **Persona, opportunità** oppure **Oggetto personalizzato** gettoni.

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >Quando si accede a un array (opportunità o oggetto personalizzato), il limite è limitato ai 10 elementi più recenti associati alla persona.

1. Nota che il token viene selezionato/attivo dopo averlo trascinato nell’editor di script.

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >Se digiti dei token in formato libero, assicurati di controllare/attivare tutti i token corrispondenti nell’albero o saranno trattati come testo normale e non funzioneranno.

1. Scrivi il tuo script in Velocity. Di seguito sono riportate alcune risorse utili:

   * [Documentazione sugli script per e-mail per sviluppatori Marketo](https://developers.marketo.com/email-scripting/)
   * [Guida utente di Velocity](https://velocity.apache.org/engine/devel/user-guide.html)
   * [Guida di riferimento di Velocity](https://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Javadoc Strumenti Velocity](https://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. Al termine dello script, fai clic su **Salva**.

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. Fai clic su **Salva** ancora una volta.

   ![](assets/image2014-9-17-22-3a23-3a13.png)

Ora puoi utilizzare questo token nelle e-mail. Lo script verrà eseguito ogni volta che viene inviato un messaggio e-mail.

>[!MORELIKETHIS]
>
>[Aggiungi un token di script e-mail al tuo indirizzo e-mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-an-email-script-token-to-your-email.md)
