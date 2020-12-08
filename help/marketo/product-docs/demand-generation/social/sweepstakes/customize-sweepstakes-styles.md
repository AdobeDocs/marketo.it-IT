---
unique-page-id: 2359807
description: Personalizza gli stili Sweepstakes - Marketo Docs - Documentazione prodotto
title: Personalizza stili Sweepstakes
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# Personalizza stili Sweepstakes {#customize-sweepstakes-styles}

Quando [create una pagina di destinazione](create-sweepstakes.md), potete personalizzare l’aspetto che avrà sulla pagina di destinazione.

>[!NOTE]
>
>**Disponibilità**
>
>Non tutti i clienti hanno acquistato questa funzionalità. Per informazioni, contattate il rappresentante commerciale.

1. Vai a Attività di marketing.

![](assets/login-marketing-activities-1.png)

1. Selezionate gli sweep e fate clic su **Modifica** **bozza**.

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. Nell’editor Sweepstakes, vai a **App** **Settings** **>** Appearance **(Impostazioni app**).

   ![](assets/image2014-9-25-17-3a51-3a59.png)

1. Modificate il testo del pulsante di registrazione e il collegamento di avanzamento.
1. ![](assets/image2014-9-25-17-3a52-3a22.png)

1. Per ogni elemento che desiderate personalizzare, immettete le vostre proprietà CSS personalizzate.

   ![](assets/image2014-9-25-17-3a52-3a37.png)

   Esempio di CSS per il pulsante **Invio**:
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>` Immagine di esempio per il pulsante **Invio**:
   `<pre>background:url(http://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >Se si utilizza un&#39;immagine con del testo al suo interno, ricordare di rimuovere il testo dal campo **Enter** **Button **Text precedente.

1. A ogni modifica, il risultato viene visualizzato nell’anteprima Visualizza e modifica.

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >**Promemoria**
   >
   >
   >Eseguite il test del pulsante in diversi browser, incluse versioni precedenti.

   >[!NOTE]
   >
   >**Articoli correlati**
   >
   >
   >Il passo successivo consiste nell’aggiungere e-mail di [registrazione e di evasione alle vostre esigenze](../../../../product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md).

