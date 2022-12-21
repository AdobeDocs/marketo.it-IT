---
unique-page-id: 2360403
description: Confrontare l’efficacia del programma con Program Analyzer - Marketo Docs - Documentazione del prodotto
title: Confrontare l'efficacia del programma con Program Analyzer
exl-id: 6e54d0a4-3cff-46cf-be0d-1992a39d8c03
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Confrontare l&#39;efficacia del programma con Program Analyzer {#compare-program-effectiveness-with-the-program-analyzer}

Utilizzare Program Analyzer per identificare i programmi più efficaci e meno efficaci, confrontando i costi dei programmi, l&#39;acquisizione dei membri, la pipeline e i ricavi.

>[!PREREQUISITES]
>
>[Creare un’analisi dei programmi](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. Fai clic su **Analytics**.

   ![](assets/image2014-9-17-18-3a50-3a30.png)

1. Seleziona il tuo programma Analyzer.

   ![](assets/image2014-9-17-18-3a50-3a37.png)

1. Cambia la visualizzazione in per programma.

   ![](assets/image2014-9-17-18-3a50-3a44.png)

1. Utilizza il Filtro canali per ridurre la visualizzazione a uno o due canali. Per il momento, guardiamo i programmi nel canale Tradeshow.

   ![](assets/image2014-9-17-18-3a51-3a2.png)

   >[!TIP]
   >
   >Un modo rapido per filtrare i programmi in un solo canale è quello di selezionare **Visualizza** > **Per canale**, fai clic sulla bolla per quel canale, quindi fai clic sul nome del canale nella finestra di dialogo a comparsa.

1. Utilizza il menu a discesa Asse X per scegliere una metrica per l’asse orizzontale. Inizieremo con il costo del programma.

   ![](assets/image2014-9-17-18-3a52-3a16.png)

1. Utilizza il menu a discesa Asse Y per scegliere una metrica per l’asse verticale. Scegliamo Nuovi nomi per trovare programmi che siano in grado di acquisire nuovi lead.

   ![](assets/image2014-9-17-18-3a52-3a26.png)

1. Accendere i cursori per ingrandire.

   ![](assets/image2014-9-17-18-3a53-3a9.png)

   >[!TIP]
   >
   >Puoi anche provare a migliorare la tua visualizzazione passando da una scala lineare a una scala logaritmica, o viceversa. Utilizza la **Scala** in alto.

1. Esplora il grafico risultante.

   ![](assets/image2014-9-17-18-3a53-3a49.png)

   Nel nostro esempio, impariamo che Origami Expo è molto meglio di tutti gli altri programmi in quel canale per catturare nuovi nomi, e a un costo medio. Ma non è tutta la storia. Aggiungeremo altre due metriche per comprendere meglio.

1. Utilizza il menu a discesa Dimensione bolla per scegliere una metrica da confrontare in base alle dimensioni delle bolle. Sceglieremo (FT) Revenue Won per il nostro esempio.

   ![](assets/image2014-9-17-18-3a54-3a25.png)

   >[!NOTE]
   >
   >Molte delle metriche che è possibile scegliere nell&#39;analizzatore di programmi sono disponibili con calcoli di primo contatto (FT) e multi-touch (MT). È importante comprendere il [differenza tra l’attribuzione FT e MT](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

1. Osserva le bolle che cambiano dimensione nel grafico.

   ![](assets/image2014-9-17-18-3a54-3a57.png)

   Aggiungendo **(FT) Entrate vinte**, vediamo rapidamente che, mentre l&#39;Origami Expo ha acquisito molti nuovi nomi, si traduce in entrate relativamente ridotte. Inoltre, vediamo che il programma Paper Fest 12 sta ottenendo meno nomi ma migliori, in quanto influenza più entrate vinte (bolla più grande).

1. Utilizza il menu a discesa Colore per aggiungere una quarta metrica. Esamineremo i ricavi per gli investimenti (FT).

   ![](assets/image2014-9-17-18-3a55-3a33.png)

1. Guardate come cambiano i colori nel grafico.

   ![](assets/image2014-9-17-18-3a55-3a47.png)

Vediamo che il programma Paper Fest 12 non solo influenza più entrate (bolla più grande), ma nonostante il suo costo relativamente elevato del programma (sul lato destro), ha il miglior ritorno agli investimenti (bolla più verde) di tutti i programmi nel canale Tradeshow.

>[!TIP]
>
>È possibile confrontare rapidamente i programmi in un canale con quelli in un altro. Utilizza semplicemente **Filtro canale** nella parte superiore della finestra per aggiungere altri canali.

>[!MORELIKETHIS]
>
>* [Esplorare i dettagli del programma e del canale con Program Analyzer](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)
>* [Confrontare l&#39;efficacia dei canali con Program Analyzer](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-channel-effectiveness-with-the-program-analyzer.md)

