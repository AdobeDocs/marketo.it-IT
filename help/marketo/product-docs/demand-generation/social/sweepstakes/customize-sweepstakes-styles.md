---
unique-page-id: 2359807
description: Personalizza gli stili Sweepstakes - Marketo Docs - Documentazione prodotto
title: Personalizza stili Sweepstakes
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---


# Personalizza gli stili Sweepstakes {#customize-sweepstakes-styles}

Quando [create una pagina di destinazione ](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md), potete personalizzare l&#39;aspetto che avrà sulla pagina di destinazione.

>[!AVAILABILITY]
>
>Non tutti i clienti hanno acquistato questa funzionalità. Per informazioni, contattate il rappresentante commerciale.

1. Andate a **Marketing Activities**.

![](assets/login-marketing-activities-1.png)

1. Selezionate le aree di interesse e fate clic su **Modifica bozza**.

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. Nell&#39;editor Sweepstakes, andate a **Impostazioni app** > **Aspetto**.

   ![](assets/image2014-9-25-17-3a51-3a59.png)

1. Modificate il testo del pulsante di registrazione e il collegamento di avanzamento.

   ![](assets/image2014-9-25-17-3a52-3a22.png)

1. Per ogni elemento che desiderate personalizzare, immettete le vostre proprietà CSS personalizzate.

   ![](assets/image2014-9-25-17-3a52-3a37.png)

   Esempio di CSS per **Pulsante Invio**:
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>`

   Immagine di esempio per **Pulsante Invio**:
   `<pre>background:url(https://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >Se utilizzate un&#39;immagine con del testo, ricordate di rimuovere il testo dal campo **Enter Button** sotto Text (Testo).

1. A ogni modifica, il risultato viene visualizzato nell’anteprima Visualizza e modifica.

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >Eseguite il test del pulsante in diversi browser, incluse versioni precedenti.

   >[!MORELIKETHIS]
   >
   >Il passaggio successivo consiste nell&#39;aggiungere [e-mail di registrazione e di evasione alle proprie suddivisioni ](/help/marketo/product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md).
