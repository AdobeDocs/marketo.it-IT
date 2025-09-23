---
unique-page-id: 1146940
description: Definire un elenco avanzato per Smart Campaign | Batch - Documentazione Marketo - Documentazione del prodotto
title: Definire un elenco avanzato per campagna avanzata | batch
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 5%

---

# Definire un elenco avanzato per campagna avanzata | batch {#define-smart-list-for-smart-campaign-batch}

Gli elenchi avanzati sono il meccanismo utilizzato in Marketo Engage per definire &quot;chi&quot; (quali persone) includere, che si tratti di un rapporto, un elenco o una campagna avanzata. Di seguito viene descritto come definire un elenco avanzato per una campagna batch.

>[!CAUTION]
>
>Apportare modifiche a un elenco avanzato o a una fase del flusso in una campagna attiva può potenzialmente comprometterne la funzionalità. Se scegli di farlo, procedi con cautela.

1. Scegli una campagna avanzata, quindi fai clic su **[!UICONTROL Smart List]**.

   ![](assets/define-smart-list-for-smart-campaign-batch-1.png)

1. Digita per cercare un filtro e trascinalo nell’area di lavoro. Ripeti per più filtri.

   ![](assets/define-smart-list-for-smart-campaign-batch-2.png)

   >[!NOTE]
   >
   >Una campagna avanzata con solo filtri viene eseguita in modalità _Batch_. Trova le persone nel database che si qualificano in base ai filtri ed esegue tutte attraverso il flusso in una sola volta.

   >[!NOTE]
   >
   >È possibile fare in modo che una campagna avanzata venga eseguita su una persona alla volta in base a eventi live aggiungendo trigger, che attivano la modalità _Trigger_.

1. Fai clic sull’elenco a discesa e scegli un operatore di filtro per il filtro scelto.

   ![](assets/define-smart-list-for-smart-campaign-batch-3.png)

   >[!CAUTION]
   >
   >Le linee rosse ondulate indicano errori o informazioni mancanti. Se non viene corretta, la campagna non sarà valida e non verrà eseguita.

1. Immetti il valore del filtro.

   ![](assets/define-smart-list-for-smart-campaign-batch-4.png)

   >[!NOTE]
   >
   >Per impostazione predefinita, gli utenti che soddisfano TUTTE le regole dell&#39;elenco smart sono qualificati. Può essere modificato in base alle tue esigenze della campagna. Consulta [Regole per elenchi avanzati per logica complessa](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md){target="_blank"} per ulteriori informazioni.

   Per attivare eventi live una persona alla volta, scopri come [definire un elenco avanzato per Smart Campaign | Trigger](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}.

   >[!MORELIKETHIS]
   >
   >* [Definisci elenco avanzato per Smart Campaign | Trigger](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
   >* [Aggiungere un passaggio di flusso a una campagna avanzata](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}
