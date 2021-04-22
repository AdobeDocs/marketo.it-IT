---
unique-page-id: 7515767
description: Condivisione di segmenti tra aree di lavoro e partizioni - Documenti Marketo - Documentazione del prodotto
title: Condivisione di segmenti tra aree di lavoro e partizioni
exl-id: b50f4328-fdba-4e39-bc0d-75bade1f9cbc
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Condividere segmenti tra aree di lavoro e partizioni {#share-segmentations-across-workspaces-and-partitions}

>[!PREREQUISITES]
>
>Questo articolo è riservato ai clienti che dispongono di aree di lavoro e partizioni.

## Cos&#39;è una segmentazione? {#whats-a-segmentation}

Marketo è brava a scegliere le persone giuste per un programma o una campagna intelligente. Tuttavia, per gli utenti tipo più permanenti, devi utilizzare le segmentazioni. Sono necessari per utilizzare contenuti dinamici avanzati in Marketo.

>[!NOTE]
>
>Scopri [come creare segmentazioni](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).

Una volta configurati questi utenti utente (_e_ utilizzi le aree di lavoro), dovrai condividerli tra le aree di lavoro. Ecco alcune buone cose da sapere:

## Regole e suggerimenti {#rules-tips}

* Ogni abbonamento a Marketo può contenere fino a 20 Segmenti &quot;totali&quot; in più aree di lavoro (**non 20 per area di lavoro**).
* Puoi condividere una segmentazione solo con le aree di lavoro a cui hai accesso.
* Assicurati di creare e utilizzare un&#39;area di lavoro **Predefinita con visibilità in tutte le partizioni**.

* L’elaborazione della segmentazione viene eseguita solo sulle persone nell’area di lavoro in cui viene creata la segmentazione.

   * Crea la segmentazione da condividere all’interno dell’area di lavoro predefinita.
      * Approvare la segmentazione
      * L&#39;area di lavoro condivisa visualizza una cartella bloccata e la segmentazione è di sola lettura.
      * Impossibile modificare la versione condivisa. Puoi modificare solo la segmentazione originale in cui è stata creata.
   * Quando si fa clic su un segmento (ad es. settore sanitario) all’interno di una segmentazione condivisa, le persone visualizzate saranno solo le persone nella partizione associata all’area di lavoro che si sta visualizzando.
      * Se crei una segmentazione in Workspace 1 (WS1) e la condividi con WS2 e WS1 non ha accesso alla partizione per WS2, NON ricalcolerà la segmentazione.
      * Se crei una segmentazione in un’area di lavoro con partizioni limitate e la condividi con un’altra area di lavoro, l’area di lavoro che ha ricevuto la segmentazione condivisa visualizzerà solo le persone che si sovrappongono.


>[!NOTE]
>
>Alcune di queste regole sono un po&#39; complesse. Il modo più semplice per iniziare è testare con persone specifiche. Puoi sempre creare nuove segmentazioni e sbarazzarti di quelle vecchie.

## Scenari di esempio {#example-scenarios}

![](assets/image2015-5-27-16-3a26-3a25.png)

![](assets/image2015-5-27-16-3a26-3a48.png)

## Condividere una segmentazione {#share-a-segmentation}

1. Vai al **Database**.

   ![](assets/image2017-3-29-8-3a15-3a40.png)

1. Fai clic con il pulsante destro del mouse su **Segmentazioni** e seleziona **Nuove cartelle**.

   ![](assets/image2017-3-29-8-3a40-3a31.png)

1. Denomina la cartella da condividere tra le aree di lavoro (ad esempio: Condividere segmenti).

   ![](assets/image2017-3-29-8-3a40-3a45.png)

1. Sposta le segmentazioni da condividere nella cartella.

   ![](assets/image2017-3-29-8-3a41-3a3.png)

1. Fai clic con il pulsante destro del mouse sulla cartella e seleziona **Condividi cartella**.

   ![](assets/image2017-3-29-8-3a41-3a19.png)

1. Selezionare le aree di lavoro con cui si desidera condividere la cartella. Fare clic su **Salva**.

   ![](assets/image2015-5-27-11-3a6-3a40.png)

   >[!NOTE]
   >
   >Nella finestra di dialogo vengono visualizzate le aree di lavoro per le quali si dispone dell’autorizzazione per visualizzare. Pertanto, Marketo consiglia di creare e condividere segmenti dall’area di lavoro predefinita con visibilità in tutte le aree di lavoro e le partizioni.

La cartella di origine viene visualizzata nella struttura del database con una freccia che indica che è condivisa con altre aree di lavoro. Dall&#39;interno dell&#39;area di lavoro condivisa, la cartella viene visualizzata con un blocco per indicare che il contenuto della cartella è stato condiviso da un&#39;altra area di lavoro e in sola lettura.
