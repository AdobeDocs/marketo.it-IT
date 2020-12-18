---
unique-page-id: 2359793
description: Utilizzare le e-mail in Promozioni social - Documenti Marketo - Documentazione prodotto
title: Utilizzare le e-mail nelle promozioni social
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 0%

---


# Utilizzare le e-mail nelle promozioni social {#use-emails-in-social-promotions}

Quando create un&#39;offerta di riferimento [](../../../../product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) o [sweepstakes](../../../../product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md), potete includere e-mail da inviare quando la persona si registra e di nuovo quando la persona ha vinto la ricompensa.

>[!TIP]
>
>Per creare un&#39;e-mail, vedere [Invia un&#39;e-mail con un&#39;esplosione](../../../../getting-started/quick-wins/send-an-email.md).

Nelle e-mail, utilizzate i seguenti token:

* **E-mail** di registrazione: Utilizzate  **`{{social.Share Url}}`** per inviare a ciascuna persona partecipante un collegamento di condivisione personalizzato.

* **E-mail** di evasione: Utilizzate  **`{{social.Promo Code}}`** per inviare a ciascun vincitore un codice [ ](use-promo-codes-for-offer-fulfillment.md)promozionale.

>[!PREREQUISITES]
>
>Per poter aggiungere un&#39;e-mail a un&#39;app social, è necessario che sia *operativa* e *approvata*. Vedere [Modifica impostazioni per un&#39;e-mail](../../../../product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

1. Andate a **Marketing Activities**.

   ![](assets/ma.png)

1. Selezionate l&#39;app e fate clic su **Modifica bozza**.

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. Nell&#39;editor delle app per social network, andate a **Impostazioni app > Dettagli offerta** (o **Dettagli Sweepstakes**).

   ![](assets/image2014-9-19-16-3a12-3a41.png)

1. Aggiungete il messaggio e-mail di registrazione.

   ![](assets/image2014-9-19-16-3a12-3a49.png)

   >[!NOTE]
   >
   >L&#39;e-mail di conferma viene inviata automaticamente quando una persona si registra.

1. Aggiungete il messaggio e-mail di evasione.

   ![](assets/image2014-9-19-16-3a15-3a26.png)

1. In un&#39;offerta di riferimento, scegliete se l&#39;e-mail di evasione viene inviata automaticamente o manualmente.

   ![](assets/image2014-9-19-16-3a15-3a36.png)

>[!NOTE]
>
>In un’analisi approfondita, il messaggio e-mail di evasione viene sempre inviato automaticamente quando [selezionate il vincitore](../../../../product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md).

>[!NOTE]
>
>**Definizione**
>
>* **auto su obiettivo**: Il messaggio e-mail di evasione viene inviato automaticamente quando ogni partecipante soddisfa l&#39;obiettivo.
>* **inviare** manualmente: Quando le persone iniziano a raggiungere l&#39;obiettivo, tornate all&#39;offerta di riferimento per  [inviare manualmente l&#39;e-mail](../../../../product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) di evasione.

>



>[!NOTE]
>
>**Articoli correlati**
>
>Successivamente, potete [scegliere l&#39;URL di condivisione](choose-the-share-url-for-a-social-app.md) oppure, nell&#39;offerta di riferimento, potete [caricare i codici promozionali](use-promo-codes-for-offer-fulfillment.md) che invierete.

