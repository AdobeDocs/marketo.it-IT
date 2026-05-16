---
unique-page-id: 2359457
description: Scopri come approvare una segmentazione in modo che possa essere utilizzata per contenuti dinamici e reporting. Utilizza le azioni di database e segmentazione per approvare dopo aver definito le regole dei segmenti.
title: Approvare una segmentazione
exl-id: c8b0fbe9-012c-47bf-8769-0167156b43d3
feature: Segmentation
TQID: https://experienceleague.adobe.com/hvFKybwLh1INYx2YWtOmdebJVYXOzhNMMncqeOoV8EU
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
  - id: df8eb12b-4f82-491f-acbb-d74012ca5654
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 246
ht-degree: 5%

---

# Approvare una segmentazione {#approve-a-segmentation}

Una segmentazione deve essere approvata prima di poter essere utilizzata.

>[!PREREQUISITES]
>
>* [Crea una segmentazione](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)
>* [Definisci regole segmento](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)

>[!NOTE]
>
>È possibile approvare un massimo di 20 segmentazioni alla volta.

1. Passare a **[!UICONTROL Database]**.

   ![](assets/approve-a-segmentation-1.png)

1. Nella segmentazione fare clic su **[!UICONTROL Segmentation Actions]** e quindi su **[!UICONTROL Approve]**.

   ![](assets/approve-a-segmentation-2.png)

   >[!NOTE]
   >
   >Lo stato cambia in _Approvazione_ mentre è in corso l&#39;approvazione.

   >[!CAUTION]
   >
   >Il completamento dell&#39;approvazione può richiedere da alcuni minuti a uno o due giorni, a seconda delle dimensioni del database.

1. Una volta approvato, [!UICONTROL Status] cambia da [!UICONTROL Approving] a [!UICONTROL Approved].

   ![](assets/approve-a-segmentation-3.png)

   >[!TIP]
   >
   >Il numero di persone in ciascun segmento viene visualizzato tra parentesi accanto al nome del segmento.

1. La scheda **[!UICONTROL People]** in **[!UICONTROL Segment]** ora mostra l&#39;elenco finale delle persone per il segmento.

   ![](assets/approve-a-segmentation-4.png)

>[!CAUTION]
>
>Il numero totale di segmenti che puoi creare in una segmentazione dipende dal numero e dal tipo di filtri utilizzati e anche dalla complessità della logica dei segmenti. Anche se è possibile creare fino a 100 segmenti utilizzando campi standard, l’utilizzo di altri tipi di filtri può aumentare la complessità e la segmentazione potrebbe non essere approvata. Alcuni esempi sono: campi personalizzati, membri di un elenco, campi del proprietario del lead e fasi dei ricavi.
>
>Se ricevi un messaggio di errore durante l&#39;approvazione e hai bisogno di assistenza per ridurre la complessità della segmentazione, contatta il [supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support).

>[!MORELIKETHIS]
>
>[Utilizzare i filtri di segmento in un elenco avanzato](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/use-segment-filters-in-a-smart-list.md)
