---
unique-page-id: 2359791
description: Specificare l'obiettivo per l'offerta di riferimento - Documenti Marketo - Documentazione del prodotto
title: Specifica obiettivo per offerta di riferimento
exl-id: 9869eb66-53df-4ea8-903f-e6650add8da2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Specifica obiettivo per offerta di riferimento {#specify-goal-for-referral-offer}

Quando [creare un’offerta di riferimento](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md), devi definire l’obiettivo di realizzazione. L’obiettivo può essere definito in base all’attività della persona sulla pagina web, ad esempio visite di pagina o iscrizioni. Puoi anche utilizzare un [evento JavaScript personalizzato](/help/marketo/product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md).

In alternativa, è possibile utilizzare un trigger di elenco smart in Marketo per attendere qualsiasi attività cardine, ad esempio la creazione di un’opportunità per la persona indicata.

Obiettivi di esempio:

* 10 visite di riferimento
* 5 iscrizioni di riferimento
* 1 opportunità di riferimento creata
* 2 acquisti e-commerce rinviati
* 5 partecipanti al webinar di riferimento

1. Vai a **Attività di marketing**.

   ![](assets/ma.png)

1. Seleziona l’offerta di riferimento e fai clic su **Modifica bozza**.

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. Nell’editor delle offerte di riferimento, vai a **Impostazioni app** > **Dettagli offerta**.

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. Sotto **Impostazioni**, scegli un tipo di evento dal **Obiettivo di realizzazione** a discesa.

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>Se prevedi di utilizzare il **Attribuisci credito al referente** passaggio di flusso, è necessario selezionare **Attivatore di elenchi avanzati** come tipo di obiettivo di realizzazione qui.

* Visite di riferimento: I partecipanti all’offerta ricevono credito per ogni visita da un amico alla pagina che ospita la tua offerta.
* Segni di riferimento: I partecipanti all&#39;offerta ricevono credito per ogni amico che si iscrive all&#39;offerta.
* Attivatore di elenchi avanzati: I partecipanti all&#39;offerta ricevono credito per ogni amico che soddisfa le condizioni di un [smart list](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) attivatore in un [campagna intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md). Ad esempio, puoi utilizzare un trigger che viene attivato quando un potenziale potenziale di riferimento si iscrive a un webinar.

* Evento JavaScript personalizzato: I partecipanti all’offerta ricevono credito per ogni amico che attiva un evento JavaScript definito sulla tua pagina. Vedi [Script di conversione per eventi personalizzati](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!NOTE]
>
>Nelle campagne avanzate sono disponibili nuovi filtri e trigger per monitorare l’attività social. Vedi [utilizzare trigger e filtri per attività social](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!MORELIKETHIS]
>
>Successivamente, puoi [seleziona le e-mail di registrazione e di evasione](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) da inviare dalla tua offerta di riferimento.
