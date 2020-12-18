---
unique-page-id: 2359791
description: Specificare l'obiettivo per l'offerta di riferimento - Documenti Marketo - Documentazione prodotto
title: Specificare l'obiettivo per l'offerta di riferimento
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---


# Specificare l&#39;obiettivo per l&#39;offerta di riferimento {#specify-goal-for-referral-offer}

Quando [create un&#39;offerta di riferimento](create-a-referral-offer.md), dovete definire l&#39;obiettivo di evasione. L&#39;obiettivo può essere definito in base all&#39;attività della persona sulla pagina Web, ad esempio visite di pagina o registrazioni. È anche possibile utilizzare un evento JavaScript [personalizzato](../../../../product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md).

In alternativa, è possibile utilizzare un [attivatore smart list](specify-goal-for-referral-offer.md) in Marketo per attendere qualsiasi attività cardine, ad esempio la creazione di un&#39;opportunità per la persona di riferimento.

Obiettivi di esempio:

* 10 visite di cui
* 5 registrazioni di riferimento
* 1 opportunità di riferimento creata
* 2 acquisti e-commerce di riferimento
* 5 partecipanti al webinar di riferimento

1. Andate a **Marketing Activities**.

   ![](assets/ma.png)

1. Selezionate l&#39;offerta di riferimento e fate clic su **Modifica bozza.**

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. Nell&#39;editor delle offerte di riferimento, andate a **Impostazioni app** > **Dettagli offerta.**

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. In **Impostazioni**, scegliete un tipo di evento dal menu a discesa **Obiettivo di evasione**.

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>Se si prevede di utilizzare il passaggio di flusso **Assegna credito al referente**, è necessario selezionare il trigger **Smart List** come tipo di obiettivo di evasione.

* Visite di riferimento: I partecipanti all&#39;offerta ricevono credito per ogni visita da un amico alla pagina in cui è presente l&#39;offerta.
* Sign-Ups Di Riferimento: I partecipanti all&#39;offerta ricevono credito per ogni amico che si registra per l&#39;offerta.
* Trigger elenco avanzato: I partecipanti all&#39;offerta ottengono credito per ogni amico che soddisfa le condizioni di un [trigger di elenco smart](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) in una [campagna smart](http://docs.marketo.com/display/docs/smart+campaigns). Ad esempio, potete utilizzare un trigger che si attiva quando un potenziale potenziale di ricerca di riferimento si registra per un seminario Web.

* Evento JavaScript personalizzato: I partecipanti all&#39;offerta ottengono credito per ogni amico che attiva un evento JavaScript definito sulla pagina. Vedere [Script di conversione per eventi personalizzati](../../../../product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!NOTE]
>
>Nelle campagne intelligenti sono disponibili nuovi filtri e attivatori per monitorare l&#39;attività social. Consultate [usare attivatori e filtri per attività social](../../../../product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!MORELIKETHIS]
>
>Successivamente, è possibile [selezionare le e-mail di registrazione e di evasione](send-referral-offer-fulfillment-email.md) da inviare dall&#39;offerta di riferimento.

