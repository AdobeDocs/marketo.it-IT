---
unique-page-id: 7515767
description: Condivisione di segmenti tra aree di lavoro e partizioni - Documenti Marketo - Documentazione prodotto
title: Condivisione di segmenti tra aree di lavoro e partizioni
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---


# Condivisione di segmenti tra aree di lavoro e partizioni {#share-segmentations-across-workspaces-and-partitions}

>[!PREREQUISITES]
>
>Questo articolo è solo per i clienti che dispongono di aree di lavoro e partizioni

## Cos&#39;è una segmentazione? {#whats-a-segmentation}

Marketo è bravo a scegliere le persone giuste per un programma o una campagna intelligente. Tuttavia, per le persone più permanenti, è consigliabile utilizzare le segmentazioni. Sono necessari per utilizzare contenuti dinamici avanzati in Marketo.

>[!NOTE]
>
>**Tubo profondo**
>
>Scopri [come creare segmentazioni](../../../product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).

Una volta configurate queste persone (**e** utilizzate le aree di lavoro), sarà necessario condividerle tra le aree di lavoro. Ecco alcune buone cose da sapere:

## Regole e suggerimenti {#rules-tips}

* Ogni iscrizione a Marketo può contenere fino a 20 segmentazioni &quot;totali&quot; su più aree di lavoro (**non 20 per area di lavoro**).
* È possibile condividere una segmentazione solo con aree di lavoro a cui si ha accesso.
* Assicuratevi di creare e utilizzare un&#39;area di lavoro **Predefinita con visibilità in tutte le partizioni**.

* L&#39;elaborazione della segmentazione viene eseguita solo sulle persone nell&#39;area di lavoro in cui viene creata la segmentazione.

   * Create la segmentazione da condividere all’interno dell’area di lavoro predefinita.

      * Approva segmentazione
      * L&#39;area di lavoro condivisa visualizza una cartella bloccata e la segmentazione è di sola lettura.
      * La versione condivisa non può essere modificata. È possibile modificare solo la segmentazione originale in cui è stata creata.
   * Quando si fa clic su un segmento (ad es. settore sanitario) all&#39;interno di una segmentazione condivisa, le persone visualizzate saranno solo le persone nella partizione associata all&#39;area di lavoro visualizzata.

      * Se si crea una segmentazione in Workspace 1 (WS1) e la si condivide con WS2 e WS1 non ha accesso alla partizione per WS2, NON verrà ricalcolata la segmentazione.
      * Se crei una segmentazione in un’area di lavoro con partizioni limitate e la condividi con un’altra area di lavoro, l’area di lavoro che ha ricevuto la segmentazione condivisa visualizzerà solo le persone che si sovrappongono.


>[!NOTE]
>
>Alcune di queste regole sono un po&#39; complesse. Il modo più semplice per iniziare è testare con persone specifiche. Puoi sempre creare nuove segmentazioni e sbarazzarti di quelle vecchie.

## Scenari di esempio {#example-scenarios}

![](assets/image2015-5-27-16-3a26-3a25.png)

** ![](assets/image2015-5-27-16-3a26-3a48.png)

**

## Condivisione di una segmentazione {#share-a-segmentation}

1. Vai al database.

   ![](assets/image2017-3-29-8-3a15-3a40.png)

1. Fai clic con il pulsante destro del mouse su Segmentazioni e seleziona Nuove cartelle.

   ![](assets/image2017-3-29-8-3a40-3a31.png)

1. Denominate la cartella da condividere tra le aree di lavoro (ad esempio: Segmenti di condivisione.)

   ![](assets/image2017-3-29-8-3a40-3a45.png)

1. Sposta le segmentazioni da condividere nella cartella.

   ![](assets/image2017-3-29-8-3a41-3a3.png)

1. Fate clic con il pulsante destro del mouse sulla cartella e selezionate Condividi cartella.

   ![](assets/image2017-3-29-8-3a41-3a19.png)

1. Selezionate le aree di lavoro con cui desiderate condividere la cartella. Fate clic su Salva.

   ![](assets/image2015-5-27-11-3a6-3a40.png)

   >[!NOTE]
   >
   >Nella finestra di dialogo vengono visualizzate le aree di lavoro per le quali si dispone dell’autorizzazione di visualizzazione. Per questo motivo, Marketo consiglia di creare e condividere segmenti dall’area di lavoro Predefinito con visibilità in tutte le aree di lavoro e le partizioni.

La cartella di origine viene visualizzata nella struttura del database con una freccia che indica che è condivisa con altre aree di lavoro. Nell’area di lavoro condivisa, la cartella viene visualizzata con un blocco che indica che il contenuto della cartella è stato condiviso da un’altra area di lavoro e che è di sola lettura.

>[!NOTE]
>
>**Articoli correlati**
>
>[Segmentazione e snippet](http://docs.marketo.com/display/docs/segmentation+and+snippets)

