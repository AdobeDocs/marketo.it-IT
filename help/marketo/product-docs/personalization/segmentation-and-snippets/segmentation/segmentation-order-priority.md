---
unique-page-id: 2359500
description: Scopri la priorità dell’ordine di segmentazione e come determina a quale segmento appartiene una persona. Modifica l’ordine dei segmenti nel database per controllarne la valutazione.
title: Priorità ordine di segmentazione
exl-id: c20d07c8-5e53-4f54-a7a3-2e1aa4fb0cdd
feature: Segmentation
source-git-commit: 80b39eb99cdaacf4c9655aa175da3d22548dcca6
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 4%

---

# Priorità ordine di segmentazione {#segmentation-order-priority}

È importante comprendere in che modo **order** imposta la priorità per la valutazione delle persone in una segmentazione.

>[!PREREQUISITES]
>
>[Crea una segmentazione](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)
>[Definisci regole segmento](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)

>[!NOTE]
>
>Puoi modificare una segmentazione solo in modalità bozza.

1. Vai al **database**.

   ![](assets/segmentation-order-priority-1.png)

1. Seleziona la **segmentazione**. In **[!UICONTROL Segmentation Actions]**, fare clic su **[!UICONTROL Edit Segments]**.

   ![](assets/segmentation-order-priority-2.png)

   Da questa schermata puoi controllare o modificare l’ordine dei segmenti.

   ![](assets/segmentation-order-priority-3.png)

>[!NOTE]
>
>* I segmenti si escludono a vicenda. Una persona può essere membro di un solo segmento alla volta.
>* Quando una persona è idonea per due segmenti, apparterrà solo al primo segmento dell’elenco.
>* Se una persona non è idonea per alcun segmento, diventa membro del segmento predefinito.
