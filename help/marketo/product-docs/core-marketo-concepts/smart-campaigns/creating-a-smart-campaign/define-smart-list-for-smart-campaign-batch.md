---
unique-page-id: 1146940
description: Definire un elenco avanzato per Smart Campaign | Batch - Documentazione Marketo - Documentazione del prodotto
title: Definire un elenco avanzato per Smart Campaign | Batch
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Definire un elenco avanzato per Smart Campaign | Batch {#define-smart-list-for-smart-campaign-batch}

Gli elenchi avanzati sono il meccanismo utilizzato in Marketo per definire &quot;chi&quot; (quali persone) da includere, sia che si tratti di un rapporto, di un elenco o di una campagna intelligente. Ecco come definire un elenco smart per una campagna batch.

1. Scegli una campagna avanzata, quindi fai clic su **Elenco avanzato**.

   ![](assets/campaignchoose-hand.png)

1. Digita per cercare un filtro, quindi trascinalo e rilascialo nell’area di lavoro. Ripeti l’operazione per più filtri.

   ![](assets/dragin.png)

   >[!NOTE]
   >
   >Una campagna avanzata con solo i filtri viene eseguita in modalità **Batch** . Trova le persone nel database che si qualificano in base ai filtri e le esegue tutte in una sola volta nel flusso.

   >[!NOTE]
   >
   >Puoi eseguire una campagna intelligente su una persona alla volta in base agli eventi live aggiungendo dei trigger, che inseriscono la campagna intelligente in modalità **Trigger** .

1. Fai clic sull’elenco a discesa e scegli un operatore di filtro per il filtro scelto.

   ![](assets/programdropdown-hands.png)

   >[!CAUTION]
   >
   >Le linee rosse strizzate indicano errori o informazioni mancanti. Se non viene corretta, la campagna non sarà valida e non verrà eseguita.

1. Immetti il valore del filtro.

   ![](assets/chooseprogram.png)

   >[!NOTE]
   >
   >Per impostazione predefinita, le persone che soddisfano TUTTE le regole dell’elenco avanzato sono qualificate. Può essere modificato in base alle esigenze della campagna. Consulta [Regole di elenco avanzato per la logica complessa](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md) per ulteriori informazioni.

   Per attivare eventi live una persona alla volta, scopri come [definire un elenco avanzato per Smart Campaign | Trigger](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md).

   >[!MORELIKETHIS]
   >
   >* [Definire un elenco avanzato per Smart Campaign | Trigger](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
   >* [Aggiungere un passaggio di flusso a una campagna avanzata](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

