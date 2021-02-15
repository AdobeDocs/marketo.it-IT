---
unique-page-id: 2360403
description: Confronta l'efficacia del programma con il programma Analyzer - Marketo Docs - Documentazione del prodotto
title: Confronta l'efficacia del programma con Program Analyzer
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 0%

---


# Confronta l&#39;efficacia del programma con l&#39;analizzatore del programma {#compare-program-effectiveness-with-the-program-analyzer}

Utilizzate Program Analyzer per identificare i programmi più e meno efficaci, confrontando i costi dei programmi, l&#39;acquisizione dei membri, la pipeline e le entrate.

>[!PREREQUISITES]
>
>* [Creare un analizzatore di programmi](create-a-program-analyzer.md)


1. Fate clic su Analytics.

   ![](assets/image2014-9-17-18-3a50-3a30.png)

1. Selezionare il programma Analyzer.

   ![](assets/image2014-9-17-18-3a50-3a37.png)

1. Modificate Visualizza in per programma.

   ![](assets/image2014-9-17-18-3a50-3a44.png)

1. Usate il filtro canale per ridurre la visualizzazione a uno o due canali. Per ora, guardiamo i programmi nel canale di Tradeshow.

   ![](assets/image2014-9-17-18-3a51-3a2.png)

   >[!TIP]
   >
   >Un modo rapido per filtrare i programmi su un solo canale è selezionare **Visualizza > Per canale**, fare clic sulla bolla per quel canale, quindi fare clic sul nome del canale nella finestra di dialogo a comparsa.

1. Utilizzate il menu a discesa Asse X per scegliere una metrica per l&#39;asse orizzontale. Cominceremo con il costo del programma.

   ![](assets/image2014-9-17-18-3a52-3a16.png)

1. Utilizzate il menu a discesa Asse Y per scegliere una metrica per l&#39;asse verticale. Scegliamo New Names (Nuovi nomi) per trovare programmi adatti a catturare nuovi lead.

   ![](assets/image2014-9-17-18-3a52-3a26.png)

1. Attivate i cursori per ingrandire.

   ![](assets/image2014-9-17-18-3a53-3a9.png)

   >[!TIP]
   >
   >È inoltre possibile provare a migliorare la visualizzazione passando da una scala lineare a una logaritmica o viceversa. Utilizzate il menu **Scala** nella parte superiore.

1. Esplorate il grafico risultante.

   ![](assets/image2014-9-17-18-3a53-3a49.png)

   Nel nostro esempio, impariamo che l&#39;Origami Expo è molto meglio di tutti gli altri programmi in quel canale per catturare nuovi nomi, e ad un costo medio. Ma non è tutta la storia. Aggiungeremo altre due metriche per comprendere meglio.

1. Utilizzate il menu a discesa Dimensione bolla per scegliere una metrica da confrontare per la dimensione delle bolle. Sceglieremo (FT) Revenue Won per il nostro esempio.

   ![](assets/image2014-9-17-18-3a54-3a25.png)

   >[!NOTE]
   >
   >Molte delle metriche che è possibile scegliere nell&#39;analizzatore di programma sono disponibili con calcoli &quot;first-touch&quot; (FT) e &quot;multi-touch&quot; (MT). È importante comprendere la differenza [tra l&#39;attribuzione FT e MT](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

1. Le bolle cambiano dimensione nel grafico.

   ![](assets/image2014-9-17-18-3a54-3a57.png)

   Aggiungendo **(FT) Revenue Won**, vediamo rapidamente che, mentre l&#39;Origami Expo ha acquisito molti nuovi nomi, si traduce in entrate relativamente poco. Inoltre, vediamo che il programma Paper Fest 12 sta ottenendo meno ma migliori nomi, in quanto influenza più entrate vinte (bolla più grande).

1. Utilizzate il menu a discesa Colore per aggiungere una quarta metrica. Vedremo (FT) Revenue to Investment.

   ![](assets/image2014-9-17-18-3a55-3a33.png)

1. Guardate come cambiano i colori nel grafico.

   ![](assets/image2014-9-17-18-3a55-3a47.png)

Vediamo che il programma Paper Fest 12 non solo influenza più entrate (bolla più grande), ma nonostante il suo costo relativamente elevato (sul lato destro), ha il miglior ritorno all&#39;investimento (bolla più verde) di tutti i programmi nel canale Tradeshow.

>[!TIP]
>
>È possibile confrontare rapidamente i programmi in un canale con quelli in un altro. È sufficiente utilizzare il **Filtro canale** nella parte superiore della finestra per aggiungere altri canali.

>[!MORELIKETHIS]
>
>* [Esplora i dettagli di programma e canale con il programma Analyzer](explore-program-and-channel-details-with-the-program-analyzer.md)
>* [Confronto dell&#39;efficacia dei canali con l&#39;analisi dei programmi](compare-channel-effectiveness-with-the-program-analyzer.md)


>[!NOTE]
>
>Ulteriori informazioni sulle analisi avanzate in [Esplora ciclo di entrate](https://docs.marketo.com/display/docs/revenue+cycle+analytics).
