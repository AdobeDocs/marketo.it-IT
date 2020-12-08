---
unique-page-id: 2359791
description: Specificare l'obiettivo per l'offerta di riferimento - Documenti Marketo - Documentazione prodotto
title: Specificare l'obiettivo per l'offerta di riferimento
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---


# Specificare l&#39;obiettivo per l&#39;offerta di riferimento {#specify-goal-for-referral-offer}

Quando [create un&#39;offerta](create-a-referral-offer.md)di riferimento, dovete definire l&#39;obiettivo di evasione. L&#39;obiettivo può essere definito in base all&#39;attività della persona sulla pagina Web, ad esempio visite di pagina o registrazioni. È anche possibile utilizzare un evento [JavaScript](../../../../product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md)personalizzato.

In alternativa, è possibile utilizzare un attivatore [per elenchi](specify-goal-for-referral-offer.md) smart in Marketo per attendere un&#39;attività cardine, ad esempio la creazione di un&#39;opportunità per la persona di riferimento.

Obiettivi di esempio:

* 10 visite di cui
* 5 registrazioni di riferimento
* 1 opportunità di riferimento creata
* 2 acquisti e-commerce di riferimento
* 5 partecipanti al webinar di riferimento

1. Vai a Attività **** di marketing.

   ![](assets/ma.png)

1. Selezionate l&#39;offerta di riferimento e fate clic su **Modifica bozza.**

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. Nell&#39;editor delle offerte di riferimento, andate a Impostazioni **** app > Dettagli **offerta.**

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. In **Impostazioni**, scegliete un tipo di evento dal menu a discesa **Obiettivo** di evasione.

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>Se si prevede di utilizzare il passaggio **di flusso Assegna credito al referente** , è necessario selezionare Attivazione **elenco** avanzato come tipo di obiettivo di evasione.

* Visite di riferimento: I partecipanti all&#39;offerta ricevono credito per ogni visita da un amico alla pagina in cui è presente l&#39;offerta.
* Sign-Ups Di Riferimento: I partecipanti all&#39;offerta ricevono credito per ogni amico che si registra per l&#39;offerta.
* Trigger elenco avanzato: I partecipanti all&#39;offerta ottengono credito per ogni amico che soddisfa le condizioni di un attivatore di elenco [](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) avanzato in una campagna [](http://docs.marketo.com/display/docs/smart+campaigns)intelligente. Ad esempio, potete utilizzare un trigger che si attiva quando un potenziale potenziale di ricerca di riferimento si registra per un seminario Web.

* Evento JavaScript personalizzato: I partecipanti all&#39;offerta ottengono credito per ogni amico che attiva un evento JavaScript definito sulla pagina. Vedere Script di [conversione per eventi](../../../../product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md)personalizzati.

>[!NOTE]
>
>Nelle campagne intelligenti sono disponibili nuovi filtri e attivatori per monitorare l&#39;attività social. Consultate [Utilizzare trigger e filtri per le attività](../../../../product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md)social.

>[!NOTE]
>
>**Articoli correlati**
>
>Quindi, potete [selezionare le e-mail](send-referral-offer-fulfillment-email.md) di registrazione e di evasione da inviare dall&#39;offerta di riferimento.

