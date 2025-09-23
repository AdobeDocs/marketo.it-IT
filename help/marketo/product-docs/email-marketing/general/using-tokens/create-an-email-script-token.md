---
unique-page-id: 1900577
description: Creare un token di script e-mail - Documentazione di Marketo - Documentazione di prodotto
title: Creare un token di script e-mail
exl-id: c7f8c3e0-6d64-4115-b9b6-261576360ba1
feature: Tokens
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 4%

---

# Creare un token di script e-mail {#create-an-email-script-token}

Per gli sviluppatori avanzati, puoi utilizzare [gli script Velocity](https://velocity.apache.org/engine/1.7/user-guide.html) nelle e-mail. Ecco come farlo.

1. Vai a **[!UICONTROL Marketing Activities]**.

   ![](assets/ma.png)

1. Trova e seleziona un programma (Evento, Predefinito o Coinvolgimento, ecc.).

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. Nella scheda **[!UICONTROL My Tokens]** trascinare un token **[!UICONTROL Email Script]**.

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. Denomina il token dello script e-mail e **[!UICONTROL Click to Edit]** il relativo contenuto.

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. Utilizza la struttura a destra per trascinare **[!UICONTROL Person]**, **[!UICONTROL Opportunity]** o **[!UICONTROL Custom Object]** token.

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >Quando accedi a un array (opportunità o oggetto personalizzato) sei limitato ai 10 elementi più recenti associati alla persona.

1. Osserva che il token diventa selezionato/attivo dopo averlo trascinato nell’editor di script.

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >Se digiti token in formato libero, assicurati di controllare/attivare tutti i token corrispondenti nella struttura, altrimenti verranno trattati come testo normale e non funzioneranno.

1. Scrivi il tuo script in Velocity. Di seguito sono riportate alcune risorse utili:

   * [Documentazione Scripting E-Mail Per Sviluppatori Marketo](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/email-scripting)
   * [Guida utente Velocity](https://velocity.apache.org/engine/devel/user-guide.html)
   * [Guida di riferimento Velocity](https://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Strumenti Velocity Javadoc](https://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. Una volta completato lo script, fare clic su **[!UICONTROL Save]**.

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. Fai clic su **[!UICONTROL Save]** un&#39;altra volta.

   ![](assets/image2014-9-17-22-3a23-3a13.png)

Ora puoi utilizzare questo token nelle e-mail. Eseguirà lo script ogni volta che viene inviato un messaggio e-mail.

>[!MORELIKETHIS]
>
>[Aggiungi un token di script e-mail all&#39;e-mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-an-email-script-token-to-your-email.md)
