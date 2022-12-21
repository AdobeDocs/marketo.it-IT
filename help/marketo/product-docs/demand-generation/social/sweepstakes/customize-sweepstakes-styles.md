---
unique-page-id: 2359807
description: Personalizzare gli stili di Sweepstakes - Marketo Docs - Documentazione del prodotto
title: Personalizzare gli stili degli sweep
exl-id: 2b1437d9-a424-4d05-b614-7502c12e6ba2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---

# Personalizzare gli stili degli sweep {#customize-sweepstakes-styles}

Quando [creare una sweep](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md), puoi personalizzare l’aspetto della pagina di destinazione.

>[!AVAILABILITY]
>
>Non tutti i clienti hanno acquistato questa funzionalità. Contatta il tuo rappresentante commerciale per i dettagli.

1. Vai a **Attività di marketing**.

![](assets/login-marketing-activities-1.png)

1. Seleziona la posta in gioco e fai clic su **Modifica bozza**.

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. Nell&#39;editor Sweepstakes, vai a **Impostazioni app** > **Aspetto**.

   ![](assets/image2014-9-25-17-3a51-3a59.png)

1. Modifica il testo del pulsante di registrazione e il collegamento di avanzamento.

   ![](assets/image2014-9-25-17-3a52-3a22.png)

1. Per ogni elemento che desideri personalizzare, immetti le proprietà CSS personalizzate.

   ![](assets/image2014-9-25-17-3a52-3a37.png)

   Esempio di CSS per **Pulsante Invio**:
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>`

   Immagine di esempio per **Pulsante Invio**:
   `<pre>background:url(https://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >Se utilizzi un’immagine con testo su di essa, ricorda di rimuovere il testo dal **Pulsante Invio** campo sotto Testo sopra.

1. Man mano che apporti ogni modifica, il risultato viene visualizzato nell’anteprima Visualizza e modifica .

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >Testa il pulsante in diversi browser, incluse le versioni precedenti.

   >[!MORELIKETHIS]
   >
   >Il passaggio successivo consiste nell’aggiungere [e-mail di iscrizione e di evasione per i vostri dolci](/help/marketo/product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md).
