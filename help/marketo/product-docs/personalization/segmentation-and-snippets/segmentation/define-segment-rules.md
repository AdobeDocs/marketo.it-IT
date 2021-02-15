---
unique-page-id: 2359449
description: Definizione delle regole di segmento - Documenti Marketo - Documentazione prodotto
title: Definire le regole di segmento
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---


# Definire le regole di segmento {#define-segment-rules}

La definizione delle regole di segmento consente di classificare le persone in diversi gruppi che si escludono a vicenda.

>[!PREREQUISITES]
>
>[Creazione di una segmentazione](create-a-segmentation.md)

1. Vai al **database.**

   ![](assets/image2017-3-28-14-3a7-3a42.png)

1. Fare clic su **Segmentazione **dalla struttura, quindi fare clic su un particolare **Segmento**.

   ![](assets/image2017-3-28-14-3a11-3a15.png)

1. Fare clic su **Smart List** e aggiungere i filtri.

   ![](assets/image2017-3-28-14-3a18-3a19.png)

   >[!CAUTION]
   >
   >I segmenti attualmente non supportano gli operatori *In Past* e *In Timeframe *nei filtri. Questo perché le segmentazioni controllano solo la disponibilità di aggiornamenti quando viene registrato un valore di dati di modifica. Questi valori sono *not* registrati per elementi che si modificano automaticamente, come campi formula e date. Inoltre, gli operatori di date con intervalli di date relativi non sono supportati in quanto vengono calcolati al momento dell&#39;approvazione della segmentazione, non al momento di un&#39;attività Modifica valore dati.

   >[!NOTE]
   >
   >I filtri &quot;SFDC Type&quot; e &quot;Microsoft Type&quot; non sono attualmente supportati negli elenchi smart di segmentazione.

1. Compila i valori appropriati per i filtri.

   ![](assets/image2017-3-28-14-3a18-3a33.png)

   >[!NOTE]
   >
   >**Tubo profondo**
   >
   >
   >Gli elenchi intelligenti sono straordinari. Scopri tutto quello che puoi fare con [Smart Lists and Static Lists](https://docs.marketo.com/display/docs/smart+lists+and+static+lists).

1. Fare clic sulla scheda **Persone (Bozza)** per visualizzare le persone che possono essere considerate membri di questo segmento.

   ![](assets/image2017-3-28-14-3a20-3a15.png)

1. Vai a **Azioni segmentazione**. Fare clic su **Approva**.

   ![](assets/image2014-9-15-11-3a36-3a7.png)

   >[!CAUTION]
   >
   >Il numero totale di segmenti che è possibile creare in una segmentazione dipende dal numero e dal tipo di filtri utilizzati e anche dalla complessità della logica dei segmenti. Anche se è possibile creare fino a 100 segmenti utilizzando campi standard, l&#39;uso di altri tipi di filtri può aumentare la complessità e la segmentazione potrebbe non essere approvata. Alcuni esempi sono: campi personalizzati, membri dell’elenco, campi del proprietario del lead e fasi delle entrate.
   >
   >
   >Se durante l&#39;approvazione ricevete un messaggio di errore e richiedete assistenza per ridurre la complessità della segmentazione, contattate il supporto [Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Controlla il dashboard per una panoramica rapida dei segmenti in un grafico a torta, così come le regole applicate.

   ![](assets/image2014-9-15-11-3a36-3a19.png)

Ottimo lavoro! Questi segmenti saranno utili in molti punti di Marketo.

>[!NOTE]
>
>Una persona può essere qualificata per segmenti diversi, ma alla fine appartiene solo a uno che dipende dall&#39;ordine di priorità [dei segmenti](segmentation-order-priority.md).

>[!NOTE]
>
>**Promemoria**
>
>La schermata Persone (Bozza) mostra tutte le persone idonee ad essere membro e non è sempre l’elenco finale delle persone. Approva il segmento per visualizzare l’elenco finale.

>[!MORELIKETHIS]
>
>* [Approvare una segmentazione](approve-a-segmentation.md)

>



