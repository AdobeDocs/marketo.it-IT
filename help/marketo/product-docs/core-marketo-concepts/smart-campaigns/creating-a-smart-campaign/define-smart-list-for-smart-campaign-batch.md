---
unique-page-id: 1146940
description: Definire un elenco avanzato per Smart Campaign | Batch - Documentazione Marketo - Documentazione del prodotto
title: Definire un elenco avanzato per Smart Campaign | Lotto
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Definire un elenco avanzato per Smart Campaign | Lotto {#define-smart-list-for-smart-campaign-batch}

Gli elenchi avanzati sono il meccanismo utilizzato in Marketo per definire &quot;chi&quot; (quali persone) includere, che si tratti di un rapporto, un elenco o una campagna avanzata. Di seguito viene descritto come definire un elenco avanzato per una campagna batch.

1. Scegli una campagna avanzata, quindi fai clic su **Elenco avanzato**.

   ![](assets/define-smart-list-for-smart-campaign-batch-1.png)

1. Digita per cercare un filtro e trascinalo nell’area di lavoro. Ripeti per più filtri.

   ![](assets/define-smart-list-for-smart-campaign-batch-2.png)

   >[!NOTE]
   >
   >Viene eseguita una campagna avanzata con solo filtri **Batch** modalità. Trova le persone nel database che si qualificano in base ai filtri ed esegue tutte attraverso il flusso in una sola volta.

   >[!NOTE]
   >
   >Puoi fare in modo che una campagna avanzata venga eseguita su una persona alla volta in base a eventi live aggiungendo trigger, che inseriscono la campagna avanzata in **Trigger** modalità.

1. Fai clic sull’elenco a discesa e scegli un operatore di filtro per il filtro scelto.

   ![](assets/define-smart-list-for-smart-campaign-batch-3.png)

   >[!CAUTION]
   >
   >Le linee rosse ondulate indicano errori o informazioni mancanti. Se non viene corretta, la campagna non sarà valida e non verrà eseguita.

1. Immetti il valore del filtro.

   ![](assets/define-smart-list-for-smart-campaign-batch-4.png)

   >[!NOTE]
   >
   >Per impostazione predefinita, gli utenti che soddisfano TUTTE le regole dell&#39;elenco smart sono qualificati. Può essere modificato in base alle tue esigenze della campagna. Estrai  [Regole per elenchi avanzati per logica complessa](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md) per ulteriori informazioni.

   Per attivare eventi live una persona alla volta, scopri come [Definire un elenco avanzato per Smart Campaign | Attivatore](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md).

   >[!MORELIKETHIS]
   >
   >* [Definire un elenco avanzato per Smart Campaign | Attivatore](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
   >* [Aggiungere un passaggio di flusso a una campagna avanzata](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
