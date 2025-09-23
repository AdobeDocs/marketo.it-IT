---
unique-page-id: 2359457
description: Approvare una segmentazione - Documenti Marketo - Documentazione del prodotto
title: Approvare una segmentazione
exl-id: c8b0fbe9-012c-47bf-8769-0167156b43d3
feature: Segmentation
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 2%

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

   ![](assets/image2017-3-28-14-3a25-3a49.png)

1. Nella segmentazione fare clic su **[!UICONTROL Segmentation Actions]** e quindi su **[!UICONTROL Approve]**.

   ![](assets/image2017-3-28-14-3a46-3a22.png)

   >[!NOTE]
   >
   >Lo stato cambia in [!UICONTROL Approving] con una ruota girevole ( ![](assets/image2014-9-15-15-3a31-3a43.png)) mentre è in corso l&#39;approvazione.

   >[!CAUTION]
   >
   >Il completamento dell&#39;approvazione può richiedere da alcuni minuti a più di un giorno, a seconda delle dimensioni del database.

   Una volta approvato, [!UICONTROL Status] cambia da [!UICONTROL Approving] a [!UICONTROL Approved].
   ![](assets/image2017-3-28-14-3a46-3a44.png)

   >[!TIP]
   >
   >Il numero di persone in ciascun segmento viene visualizzato tra parentesi accanto al nome del segmento.

1. La scheda **[!UICONTROL People]** in **[!UICONTROL Segment]** ora mostra l&#39;elenco finale delle persone per il segmento.

   ![](assets/image2017-3-28-14-3a47-3a10.png)

>[!CAUTION]
>
>Il numero totale di segmenti che puoi creare in una segmentazione dipende dal numero e dal tipo di filtri utilizzati e anche dalla complessità della logica dei segmenti. Anche se è possibile creare fino a 100 segmenti utilizzando campi standard, l’utilizzo di altri tipi di filtri può aumentare la complessità e la segmentazione potrebbe non essere approvata. Alcuni esempi sono: campi personalizzati, membri di un elenco, campi del proprietario del lead e fasi dei ricavi.
>
>Se ricevi un messaggio di errore durante l&#39;approvazione e hai bisogno di assistenza per ridurre la complessità della segmentazione, contatta il [supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!MORELIKETHIS]
>
>[Utilizzare i filtri di segmento in un elenco avanzato](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/use-segment-filters-in-a-smart-list.md)
