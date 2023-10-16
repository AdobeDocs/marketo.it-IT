---
unique-page-id: 2359807
description: Personalizzare gli stili di Sweepstakes - Documentazione di Marketo - Documentazione del prodotto
title: Personalizzare gli stili di Sweepstakes
exl-id: 2b1437d9-a424-4d05-b614-7502c12e6ba2
source-git-commit: 2671f81f62658447e4b2a3dc2e02a4e0927443e8
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# Personalizzare gli stili di Sweepstakes {#customize-sweepstakes-styles}

Quando [creare una sweepstakes](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md), puoi personalizzarne l’aspetto sulla pagina di destinazione.

>[!AVAILABILITY]
>
>Non tutti gli utenti del Marketo Engage hanno acquistato questa funzionalità. Per ulteriori informazioni, contatta l’Adobe Account Team (il tuo Account Manager).

1. Vai a **Attività di marketing**.

![](assets/login-marketing-activities-1.png)

1. Selezionate le sweepstakes e fate clic su **Modifica bozza**.

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. Nell’editor di punteggi, vai a **Impostazioni app** > **Aspetto**.

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
   >Se utilizzi un’immagine con del testo, ricorda di rimuoverla dal **Pulsante Invio** in Testo sopra.

1. Ogni volta che apportate una modifica, il risultato viene visualizzato nell&#39;anteprima Visualizza e modifica.

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >Prova il pulsante in diversi browser, incluse le versioni precedenti.

   >[!MORELIKETHIS]
   >
   >Il passaggio successivo consiste nell’aggiungere [e-mail di iscrizione e di evasione ai tuoi interessi](/help/marketo/product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md).
