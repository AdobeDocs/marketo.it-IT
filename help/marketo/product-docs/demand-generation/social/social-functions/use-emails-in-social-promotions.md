---
unique-page-id: 2359793
description: Usare le email nelle promozioni Social - Marketo Docs - Documentazione prodotto
title: Utilizzare le e-mail nelle promozioni Social
exl-id: 633ad86e-d085-420f-8e28-9b722e345852
feature: Social
source-git-commit: 97324d932b65020d041f728928d3792140bea71c
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---

# Utilizzare le e-mail nelle promozioni Social {#use-emails-in-social-promotions}

Quando crei un&#39;offerta [](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) riferimento o una [lotteria](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md), puoi includere e-mail da inviare quando la persona si iscrive e di nuovo quando la persona ha vinto il premio.

>[!IMPORTANT]
>
>Il 31 luglio 2024 abbiamo iniziato il processo di deprecazione di questa funzione. Non potrai creare nuove risorse. Le risorse esistenti continueranno a funzionare fino al 31 gennaio 2025. [Ulteriori informazioni](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

>[!TIP]
>
>Per creare un messaggio e-mail, vedere [Inviare un messaggio e-mail.](/help/marketo/getting-started/quick-wins/send-an-email.md)

Nelle e-mail, utilizza questi token:

* **E-mail** di registrazione: consente di **`{{social.Share Url}}`** inviare a ogni persona partecipante una collegare di condivisione personalizzata.

* **E-mail** di evasione: da utilizzare **`{{social.Promo Code}}`** per inviare a ciascun vincitore un [codice](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md) promozionale.

>[!PREREQUISITES]
>
>Prima di poter aggiungere un&#39;e-mail a un&#39;app social, questa deve essere _operativa_ e _approvata_. Consulta [Modifica Impostazioni per ricevere un&#39;e-mail](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

1. Vai ad Attività&#x200B;**di** marketing.

   ![](assets/ma.png)

1. Seleziona l&#39;app e fai clic su **Modifica bozza**.

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. Nell&#39;editor dell&#39;app social, vai a **app Impostazioni > Dettagli** offerta (o **Dettagli** lotteria).

   ![](assets/image2014-9-19-16-3a12-3a41.png)

1. Aggiungi l&#39;indirizzo e-mail di registrazione.

   ![](assets/image2014-9-19-16-3a12-3a49.png)

   >[!NOTE]
   >
   >L&#39;e-mail di conferma viene inviata automaticamente quando una persona si iscrive.

1. Aggiungi l&#39;indirizzo e-mail di evasione.

   ![](assets/image2014-9-19-16-3a15-3a26.png)

1. In un&#39;offerta riferimento, scegli se inviare l&#39;e-mail di evasione automatica o manuale.

   ![](assets/image2014-9-19-16-3a15-3a36.png)

>[!NOTE]
>
>In un concorso a premi, l&#39;e-mail di evasione viene sempre inviata automaticamente quando selezioni [il vincitore](/help/marketo/product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md).

>[!NOTE]
>
>**Definizione**
>
>* **Auto on goal**: l&#39;e-mail di evasione viene inviata automaticamente quando ogni partecipante raggiunge l&#39;obiettivo.
>* **invio** manuale: una volta che le persone iniziano a raggiungere l&#39;obiettivo, torna alla tua offerta riferimento per inviare manualmente [l&#39;e-mail](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) di evasione.
>

>[!MORELIKETHIS]
>
>Successivo, puoi [scegliere il URL](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) di condivisione o, nella tua offerta riferimento, puoi [caricare i codici](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md) promozionali che invierai.
