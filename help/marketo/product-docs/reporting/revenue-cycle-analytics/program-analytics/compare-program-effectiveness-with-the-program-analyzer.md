---
unique-page-id: 2360403
description: Confrontare l’efficacia del programma con Program Analyzer (Analizzatore di programmi) - Documentazione di Marketo - Documentazione del prodotto
title: Confrontare l’efficacia del programma con l’Analizzatore di programmi
exl-id: 6e54d0a4-3cff-46cf-be0d-1992a39d8c03
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# Confronta efficacia del programma con [!UICONTROL Program Analyzer] {#compare-program-effectiveness-with-the-program-analyzer}

Utilizzare [!UICONTROL Program Analyzer] per identificare i programmi più efficaci e quelli meno efficaci, confrontando i costi dei programmi, l&#39;acquisizione dei membri, la pipeline e i ricavi.

>[!PREREQUISITES]
>
>[Crea un [!UICONTROL Program Analyzer]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. Fai clic su **[!UICONTROL Analytics]**.

   ![](assets/image2014-9-17-18-3a50-3a30.png)

1. Seleziona il tuo analizzatore di programmi.

   ![](assets/image2014-9-17-18-3a50-3a37.png)

1. Cambia la visualizzazione in **[!UICONTROL By Program]**.

   ![](assets/image2014-9-17-18-3a50-3a44.png)

1. Utilizza **[!UICONTROL Channel Filter]** per ridurre la visualizzazione a uno o due canali. Per il momento verranno esaminati i programmi nel canale **[!UICONTROL Tradeshow]**.

   ![](assets/image2014-9-17-18-3a51-3a2.png)

   >[!TIP]
   >
   >Un modo rapido per filtrare i programmi su un solo canale consiste nel selezionare **[!UICONTROL View]** > **[!UICONTROL By Channel]**, fare clic sulla bolla per quel canale, quindi fare clic sul nome del canale nella finestra di dialogo a comparsa.

1. Utilizzare il menu a discesa **[!UICONTROL X Axis]** per scegliere una metrica per l&#39;asse orizzontale. Inizieremo con **[!UICONTROL Program Cost]**.

   ![](assets/image2014-9-17-18-3a52-3a16.png)

1. Utilizzare il menu a discesa **[!UICONTROL Y Axis]** per scegliere una metrica per l&#39;asse verticale. Scegli **[!UICONTROL New Names]** per trovare programmi efficaci per l&#39;acquisizione di nuovi lead.

   ![](assets/image2014-9-17-18-3a52-3a26.png)

1. Accendere i dispositivi di scorrimento per ingrandire.

   ![](assets/image2014-9-17-18-3a53-3a9.png)

   >[!TIP]
   >
   >È inoltre possibile migliorare la visualizzazione passando da una scala lineare a una logaritmica o viceversa. Utilizza il menu **[!UICONTROL Scale]** nella parte superiore.

1. Esplora il grafico risultante.

   ![](assets/image2014-9-17-18-3a53-3a49.png)

   Nel nostro esempio, apprendiamo che [!DNL Origami Expo] è di gran lunga migliore di tutti gli altri programmi di quel canale per l&#39;acquisizione di nuovi nomi e a un costo medio. Ma questa non è tutta la storia. Aggiungeremo altre due metriche per ottenere una comprensione più approfondita.

1. Utilizza il menu a discesa **[!UICONTROL Bubble Size]** per scegliere una metrica da confrontare in base alla dimensione delle bolle. Sceglieremo **[!UICONTROL (FT) Revenue Won]** per il nostro esempio.

   ![](assets/image2014-9-17-18-3a54-3a25.png)

   >[!NOTE]
   >
   >Molte delle metriche selezionabili nell’analizzatore di programmi sono disponibili con calcoli di primo contatto (FT) e multi contatto (MT). È importante comprendere la [differenza tra l&#39;attribuzione FT e MT](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

1. Osserva come le bolle cambiano dimensione nel grafico.

   ![](assets/image2014-9-17-18-3a54-3a57.png)

   L&#39;aggiunta di **[!UICONTROL (FT) Revenue Won]** consente di vedere rapidamente che, mentre [!DNL Origami Expo] ha acquisito molti nuovi nomi, genera ricavi relativamente ridotti. Inoltre, notiamo che il programma [!DNL Paper Fest 12] sta ottenendo nomi meno numerosi ma migliori, in quanto influisce sull&#39;aumento dei ricavi ottenuti (bolla più grande).

1. Utilizza il menu a discesa Colore per aggiungere una quarta metrica. Esamineremo **[!UICONTROL (FT) Revenue to Investment]**.

   ![](assets/image2014-9-17-18-3a55-3a33.png)

1. Osserva come cambiano i colori nel grafico.

   ![](assets/image2014-9-17-18-3a55-3a47.png)

Si vede che il programma [!DNL Paper Fest 12] non solo influisce su maggiori ricavi (bolla più grande), ma, nonostante il suo costo relativamente elevato (sul lato destro), ha il miglior ritorno all&#39;investimento (bolla più verde) di tutti i programmi nel canale [!UICONTROL Tradeshow].

>[!TIP]
>
>È possibile confrontare rapidamente i programmi di un canale con quelli di un altro. Utilizza il **Filtro canale** nella parte superiore della finestra per aggiungere altri canali.

>[!MORELIKETHIS]
>
>* [Esplora i dettagli del programma e del canale con [!UICONTROL Program Analyzer]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)
>* [Confronta l&#39;efficacia del canale con [!UICONTROL Program Analyzer]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-channel-effectiveness-with-the-program-analyzer.md)
