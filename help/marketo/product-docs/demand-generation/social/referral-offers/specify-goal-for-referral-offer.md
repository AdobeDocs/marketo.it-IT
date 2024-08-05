---
unique-page-id: 2359791
description: Specifica l'obiettivo per l'offerta di riferimento - Marketo Docs - Product Documentazione
title: Specifica l'obiettivo per l'offerta di riferimento
exl-id: 9869eb66-53df-4ea8-903f-e6650add8da2
feature: Social
source-git-commit: 97324d932b65020d041f728928d3792140bea71c
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Specifica l&#39;obiettivo per l&#39;offerta di riferimento {#specify-goal-for-referral-offer}

Quando [crei un&#39;offerta di riferimento](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md), devi definire l&#39;obiettivo di adempimento. L&#39;obiettivo può essere definito dall&#39;attività della persona sulla pagina web, ad esempio visite alle pagine o iscrizioni. È possibile utilizzare lineare un [evento](/help/marketo/product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md) JavaScript personalizzato.

>[!IMPORTANT]
>
>Il 31 luglio 2024 abbiamo iniziato il processo di deprecazione di questa funzione. Non potrai creare nuove risorse. Le risorse esistenti continueranno a funzionare fino al 31 gennaio 2025. [Ulteriori informazioni](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

In alternativa, è possibile utilizzare un trigger elenco intelligente in Marketo Engage per attendere qualsiasi pietra miliare, ad esempio la creazione di un opportunità per la persona invitata.

Esempio di obiettivi:

* 10 visite segnalate
* 5 iscrizioni segnalate
* 1 riferito opportunità creato
* 2 acquisti e-commerce riferiti
* 5 partecipanti al webinar con riferimenti

1. Vai ad Attività&#x200B;**di** marketing.

   ![](assets/ma.png)

1. Selezionate l&#39;offerta riferimento e fate clic su **Modifica bozza**.

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. Nell&#39;editor riferimento offerta, vai a **app Impostazioni** > **Dettagli** offerta.

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. In **Impostazioni**, scegli un tipo di **evento dal menu a discesa Obiettivo** di realizzazione.

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>Se prevedi di utilizzare il **passaggio di flusso Dai credito al referente** , devi selezionare **Trigger** elenco avanzato come tipo di obiettivo di adempimento qui.

* Visite segnalate: i partecipanti all&#39;offerta ricevono credito per ogni visita da un amico alla pagina che ospita l&#39;offerta.
* Iscrizioni segnalate: i partecipanti all&#39;offerta ricevono credito per ogni amico che si iscrive all&#39;offerta.
* Trigger elenco intelligente: i partecipanti all&#39;offerta ottengono credito per ogni amico che soddisfa le condizioni di un [trigger di elenchi](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) intelligenti in una [campagna](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md) intelligente. Ad esempio, è possibile utilizzare un trigger che si attiva quando un potenziale cliente segnalato si iscrive a un webinar.

* Evento JavaScript personalizzato: i partecipanti all&#39;offerta ottengono credito per ogni amico che attiva un evento JavaScript definito sulla tua pagina. Consulta [Script di conversione per eventi personalizzati](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!NOTE]
>
>Nelle campagne intelligenti sono disponibili nuovi filtri e trigger per monitorare l’attività social. Vedi [utilizzare trigger e filtri per le attività social](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!MORELIKETHIS]
>
>Successivo, puoi [selezionare le e-mail](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) di registrazione ed evasione da inviare dalla tua offerta riferimento.
