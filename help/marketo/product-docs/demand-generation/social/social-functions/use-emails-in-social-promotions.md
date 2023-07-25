---
unique-page-id: 2359793
description: Utilizzare le e-mail nelle promozioni social - Documentazione Marketo - Documentazione del prodotto
title: Utilizzare le e-mail nelle promozioni social
exl-id: 633ad86e-d085-420f-8e28-9b722e345852
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Utilizzare le e-mail nelle promozioni social {#use-emails-in-social-promotions}

Quando si crea un [offerta di riferimento](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) o un [pali](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md), puoi includere e-mail da inviare quando la persona si iscrive e di nuovo quando la persona ha vinto la ricompensa.

>[!TIP]
>
>Per creare un messaggio e-mail, consulta [Invia un&#39;esplosione e-mail](/help/marketo/getting-started/quick-wins/send-an-email.md).

Nelle e-mail, utilizza i seguenti token:

* **E-mail di iscrizione**: Utilizzare **`{{social.Share Url}}`** per inviare a ogni persona partecipante un collegamento di condivisione personalizzato.

* **E-mail di evasione**: Utilizzare **`{{social.Promo Code}}`** per inviare a ogni vincitore un [codice promozionale](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md).

>[!PREREQUISITES]
>
>Prima di poter aggiungere un’e-mail a un’app social, devi _operative_ e _approvato_. Consulta [Modificare le impostazioni per un’e-mail](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

1. Vai a **Attività di marketing**.

   ![](assets/ma.png)

1. Seleziona l’app e fai clic su **Modifica bozza**.

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. Nell’editor delle app social, vai a **Impostazioni app > Dettagli offerta** (o **Dettagli delle puntate**).

   ![](assets/image2014-9-19-16-3a12-3a41.png)

1. Aggiungi il messaggio e-mail di registrazione.

   ![](assets/image2014-9-19-16-3a12-3a49.png)

   >[!NOTE]
   >
   >L’e-mail di conferma viene inviata automaticamente quando una persona si iscrive.

1. Aggiungi l’e-mail di adempimento.

   ![](assets/image2014-9-19-16-3a15-3a26.png)

1. In un’offerta di riferimento, scegli se l’e-mail di evasione viene inviata automaticamente o manualmente.

   ![](assets/image2014-9-19-16-3a15-3a36.png)

>[!NOTE]
>
>In un’esperienza indimenticabile, l’e-mail di evasione viene sempre inviata automaticamente quando [seleziona il vincitore](/help/marketo/product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md).

>[!NOTE]
>
>**Definizione**
>
>* **auto sull&#39;obiettivo**: l’e-mail di evasione viene inviata automaticamente quando ogni partecipante raggiunge l’obiettivo.
>* **invia manualmente**: una volta che le persone iniziano a raggiungere l’obiettivo, torna all’offerta di riferimento per [inviare l’e-mail di evasione](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md).
>

>[!MORELIKETHIS]
>
>Quindi, puoi [scegli l’URL di condivisione](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) oppure, nell’offerta di riferimento, puoi [carica i codici promozionali](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md) tu manderai.
