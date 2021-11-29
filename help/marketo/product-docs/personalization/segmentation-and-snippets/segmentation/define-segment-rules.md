---
unique-page-id: 2359449
description: Definire le regole di segmento - Documenti Marketo - Documentazione del prodotto
title: Definire le regole di segmento
exl-id: e6631848-aa8c-4709-b182-4c88abbd365b
source-git-commit: 55afdc537d0a5d0b6114f478c4dd2ded09c84e34
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# Definire le regole di segmento {#define-segment-rules}

La definizione delle regole di segmento consente di classificare le persone in gruppi diversi che si escludono a vicenda.

>[!PREREQUISITES]
>
>[Creare una segmentazione](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

1. Vai a **Database.**

   ![](assets/image2017-3-28-14-3a7-3a42.png)

1. Seleziona **Segmentazione** dall&#39;albero, quindi fare clic su un particolare **Segmento**.

   ![](assets/image2017-3-28-14-3a11-3a15.png)

1. Fai clic su **Elenco avanzato** e aggiungi i filtri.

   ![](assets/image2017-3-28-14-3a18-3a19.png)

   >[!CAUTION]
   >
   >I segmenti attualmente non supportano _In passato_ e _In Timeframe_  sui filtri. Questo perché le segmentazioni verificano la presenza di aggiornamenti solo quando viene registrato un valore di dati di modifica. Questi valori sono _not_ registrati per elementi che cambiano automaticamente, ad esempio campi formula e date. Inoltre, gli operatori di date con intervalli di date relativi non sono supportati in quanto sono calcolati al momento dell’approvazione della segmentazione, non al momento di un’attività Modifica valore dati.

   >[!NOTE]
   >
   >I filtri &quot;SFDC Type&quot; e &quot;Microsoft Type&quot; non sono attualmente supportati negli elenchi smart di segmentazione.

1. Inserisci i valori appropriati per i filtri.

   ![](assets/image2017-3-28-14-3a18-3a33.png)

   >[!CAUTION]
   >
   >Il comportamento di registrazione delle attività per i campi Account può influire sulla qualificazione. Pertanto, sconsigliamo l’uso dei campi Account durante la definizione delle regole del segmento.

1. Fai clic sul pulsante **Persone (bozza)** per visualizzare le persone che possono essere membri di questo segmento.

   ![](assets/image2017-3-28-14-3a20-3a15.png)

1. Vai a **Azioni di segmentazione**. Fai clic su **Approva**.

   ![](assets/image2014-9-15-11-3a36-3a7.png)

   >[!CAUTION]
   >
   >Il numero totale di segmenti che puoi creare in una segmentazione dipende dal numero e dal tipo di filtri utilizzati e dalla complessità della logica dei segmenti. Anche se puoi creare fino a 100 segmenti utilizzando campi standard, l’utilizzo di altri tipi di filtri può aumentare la complessità e la segmentazione potrebbe non riuscire ad approvarla. Alcuni esempi sono: campi personalizzati, membro dell’elenco, campi del proprietario del lead e fasi di ricavo.
   >
   >Se ricevi un messaggio di errore durante l’approvazione e richiedi assistenza per ridurre la complessità della segmentazione, contatta [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Consulta il dashboard per una rapida panoramica dei segmenti in un grafico a torta, oltre alle regole applicate.

   ![](assets/image2014-9-15-11-3a36-3a19.png)

Ottimo lavoro! Questi segmenti saranno molto utili in molti luoghi in Marketo.

>[!NOTE]
>
>Una persona può qualificarsi per segmenti diversi, ma alla fine appartiene solo a uno che dipende dal [ordine prioritario dei segmenti](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md).

>[!NOTE]
>
>La schermata Persone (Bozza) mostra tutte le persone che si qualificano come membri e non è sempre l’elenco finale delle persone. Approva il segmento per visualizzare l’elenco finale.

>[!MORELIKETHIS]
>
>[Approvare una segmentazione](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/approve-a-segmentation.md)
