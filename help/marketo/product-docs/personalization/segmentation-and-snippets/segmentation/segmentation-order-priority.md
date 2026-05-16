---
unique-page-id: 2359500
description: Scopri la priorità dell’ordine di segmentazione e come determina a quale segmento appartiene una persona. Modifica l’ordine dei segmenti nel database per controllarne la valutazione.
title: Priorità ordine di segmentazione
exl-id: c20d07c8-5e53-4f54-a7a3-2e1aa4fb0cdd
feature: Segmentation
TQID: https://experienceleague.adobe.com/wDvufJzxu0BFCSov4etUpEMxaol3-R5CePqllYyDeSc
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
  - id: cdd4e0f6-e87e-453f-88ee-2ee54a7de272
  - id: df8eb12b-4f82-491f-acbb-d74012ca5654
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 140
ht-degree: 4%

---

# Priorità ordine di segmentazione {#segmentation-order-priority}

È importante comprendere in che modo **order** imposta la priorità per la valutazione delle persone in una segmentazione.

>[!PREREQUISITES]
>
>[Crea segmentazione](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)
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
