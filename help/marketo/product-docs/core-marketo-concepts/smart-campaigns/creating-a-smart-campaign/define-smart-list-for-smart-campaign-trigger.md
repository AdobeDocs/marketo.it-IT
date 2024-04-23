---
unique-page-id: 1146942
description: Definire un elenco avanzato per Smart Campaign | Trigger - Documentazione di Marketo - Documentazione del prodotto
title: Definire un elenco avanzato per Smart Campaign | Trigger
exl-id: 14d9b15e-864a-47ef-8f39-3d65e6036a82
feature: Smart Campaigns
source-git-commit: a9d902bf40e6193838a931ecb96a080bae098d68
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Definire un elenco avanzato per Smart Campaign | Trigger {#define-smart-list-for-smart-campaign-trigger}

Fai in modo che una campagna avanzata venga eseguita su una persona alla volta in base agli eventi live aggiungendo trigger.

>[!CAUTION]
>
>Apportare modifiche a un elenco avanzato o a una fase del flusso in una campagna attiva può potenzialmente comprometterne la funzionalità. Se scegli di farlo, procedi con cautela.

1. In Smart Campaign, fai clic su **[!UICONTROL Elenco avanzato]** scheda.

   ![](assets/define-smart-list-for-smart-campaign-trigger-1.png)

1. Cerca il trigger desiderato e trascinalo sull’area di lavoro.

   ![](assets/define-smart-list-for-smart-campaign-trigger-2.png)

   >[!NOTE]
   >
   >Viene eseguita una campagna avanzata con trigger in _Trigger_ modalità. Viene eseguito su una persona alla volta in base agli eventi attivati ed eventuali filtri aggiuntivi.

   >[!IMPORTANT]
   >
   >Quando utilizzi un campo booleano in un elenco avanzato di una campagna di trigger, devi impostarlo esplicitamente su &quot;false&quot; affinché il campo possa essere valutato correttamente durante l’esecuzione della campagna.

1. Fai clic sull’elenco a discesa e scegli un operatore.

   ![](assets/define-smart-list-for-smart-campaign-trigger-3.png)

   >[!CAUTION]
   >
   >Le linee rosse ondulate indicano errori o informazioni mancanti. Se non viene corretta, la campagna non sarà valida e non verrà eseguita.

   >[!TIP]
   >
   >In una campagna intelligente con trigger e filtri, i trigger si trovano in alto e, quando vengono attivati, solo le persone che soddisfano i criteri di filtro passano attraverso il flusso.

1. Definisci il trigger.

   ![](assets/define-smart-list-for-smart-campaign-trigger-4.png)

   >[!NOTE]
   >
   >Con più trigger, una persona passa attraverso il flusso se _QUALSIASI_ viene attivato uno dei trigger.

Per eseguire la campagna su un set di persone contemporaneamente, scopri come [Definire un elenco avanzato per Smart Campaign | Batch](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md){target="_blank"}.

>[!MORELIKETHIS]
>
>[Aggiungere un passaggio di flusso a una campagna avanzata](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}
