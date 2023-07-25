---
unique-page-id: 2359449
description: Definire le regole del segmento - Documentazione di Marketo - Documentazione del prodotto
title: Definire le regole del segmento
exl-id: e6631848-aa8c-4709-b182-4c88abbd365b
feature: Segmentation
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# Definire le regole del segmento {#define-segment-rules}

La definizione delle regole di segmento consente di categorizzare le persone in gruppi diversi che si escludono a vicenda.

>[!PREREQUISITES]
>
>[Creare una segmentazione](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

1. Vai a **Database.**

   ![](assets/image2017-3-28-14-3a7-3a42.png)

1. Seleziona **Segmentazione** dalla struttura, quindi fare clic su un **Segmento**.

   ![](assets/image2017-3-28-14-3a11-3a15.png)

1. Clic **Elenco avanzato** e aggiungere filtri.

   ![](assets/image2017-3-28-14-3a18-3a19.png)

   >[!CAUTION]
   >
   >I segmenti attualmente non supportano _Nel passato_ e _Nell’arco temporale_  sui filtri. Questo perché le segmentazioni verificano la disponibilità di aggiornamenti solo quando viene registrato un valore di dati di modifica. Questi valori sono _non_ registrato per elementi che vengono modificati automaticamente, ad esempio campi formula e date. Inoltre, gli operatori di date con intervalli di date relativi non sono supportati in quanto vengono calcolati al momento dell’approvazione della segmentazione e non al momento di un’attività Modifica valore dati.

   >[!NOTE]
   >
   >I filtri &quot;Tipo SFDC&quot; e &quot;Tipo Microsoft&quot; non sono attualmente supportati negli elenchi avanzati di segmentazione.

1. Inserisci i valori appropriati per i filtri.

   ![](assets/image2017-3-28-14-3a18-3a33.png)

   >[!CAUTION]
   >
   >Il comportamento di registrazione delle attività per i campi Account può influire sulla qualifica. Pertanto, consigliamo di non utilizzare i campi Account durante la definizione delle regole del segmento.

1. Fai clic su **Persone (bozza)** per visualizzare le persone idonee per essere membri di questo segmento.

   ![](assets/image2017-3-28-14-3a20-3a15.png)

1. Vai a **Azioni di segmentazione**. Clic **Approva**.

   ![](assets/image2014-9-15-11-3a36-3a7.png)

   >[!CAUTION]
   >
   >Il numero totale di segmenti che puoi creare in una segmentazione dipende dal numero e dal tipo di filtri utilizzati e anche dalla complessità della logica dei segmenti. Anche se è possibile creare fino a 100 segmenti utilizzando campi standard, l’utilizzo di altri tipi di filtri può aumentare la complessità e la segmentazione potrebbe non essere approvata. Alcuni esempi sono: campi personalizzati, membri di un elenco, campi del proprietario del lead e fasi dei ricavi.
   >
   >Se ricevi un messaggio di errore durante l’approvazione e hai bisogno di assistenza per ridurre la complessità della segmentazione, contatta [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Consulta la dashboard per una panoramica rapida dei segmenti in un grafico a torta, nonché delle regole applicate.

   ![](assets/image2014-9-15-11-3a36-3a19.png)

Ottimo lavoro! Questi segmenti diventeranno utili in molti posti in Marketo.

>[!NOTE]
>
>Una persona può qualificarsi per segmenti diversi, ma alla fine appartiene a uno solo che dipende dal [ordine di priorità dei segmenti](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md).

>[!NOTE]
>
>La schermata Persone (bozza) mostra tutte le persone idonee per essere un membro e non è sempre l’elenco finale delle persone. Approva il segmento per visualizzare l’elenco finale.

>[!MORELIKETHIS]
>
>[Approvare una segmentazione](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/approve-a-segmentation.md)
