---
unique-page-id: 2359791
description: Specifica l’obiettivo per l’offerta di riferimento - Documentazione di Marketo - Documentazione del prodotto
title: Specifica l'obiettivo per l'offerta di riferimento
exl-id: 9869eb66-53df-4ea8-903f-e6650add8da2
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Specifica l&#39;obiettivo per l&#39;offerta di riferimento {#specify-goal-for-referral-offer}

Quando [creare un’offerta di riferimento](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md), è necessario definire l’obiettivo di adempimento. L’obiettivo può essere definito dall’attività della persona sulla pagina web, ad esempio visite o iscrizioni. Puoi anche utilizzare un’ [evento JavaScript personalizzato](/help/marketo/product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md).

In alternativa, puoi utilizzare un trigger di elenco avanzato in Marketo per attendere eventuali milestone, ad esempio la creazione di un’opportunità per la persona di riferimento.

Esempio di obiettivi:

* 10 visite rinviate
* 5 iscrizioni rinviate
* 1 opportunità referenziata creata
* 2 acquisti e-commerce referenziati
* 5 partecipanti al webinar con riferimenti

1. Vai a **Attività di marketing**.

   ![](assets/ma.png)

1. Seleziona l’offerta di riferimento e fai clic su **Modifica bozza**.

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. Nell’editor delle offerte di riferimento, vai a **Impostazioni app** > **Dettagli offerta**.

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. Sotto **Impostazioni**, scegli un tipo di evento dal **Obiettivo di adempimento** a discesa.

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>Se prevedi di utilizzare il **Attribuisci credito al referente** passaggio di flusso, è necessario selezionare **Trigger elenco avanzato** come tipo di obiettivo di adempimento qui.

* Visite con riferimento: i partecipanti all’offerta ricevono un credito per ogni visita da un amico alla pagina che ospita la tua offerta.
* Iscrizioni con riferimento: i partecipanti all’offerta ricevono credito per ogni amico che si iscrive all’offerta.
* Trigger elenco avanzato: i partecipanti all’offerta ricevono credito per ogni amico che soddisfa le condizioni di un [elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) attivare in un [campagna intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md). Ad esempio, puoi utilizzare un trigger che viene attivato quando un prospect indicato si iscrive a un webinar.

* Evento JavaScript personalizzato: i partecipanti all’offerta ricevono credito per ogni amico che attiva un evento JavaScript definito sulla pagina. Consulta [Script di conversione per eventi personalizzati](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!NOTE]
>
>Nelle campagne intelligenti sono disponibili nuovi filtri e trigger per monitorare l’attività social. Consulta [utilizzare trigger e filtri per attività social](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!MORELIKETHIS]
>
>Quindi, puoi [seleziona le e-mail di iscrizione e di evasione](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) da inviare dall&#39;offerta di riferimento.
