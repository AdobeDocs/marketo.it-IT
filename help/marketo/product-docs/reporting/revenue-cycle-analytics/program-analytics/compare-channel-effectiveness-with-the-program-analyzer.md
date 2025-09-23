---
unique-page-id: 2360401
description: Confrontare l’efficacia dei canali con Programme Analyzer - Documentazione di Marketo - Documentazione del prodotto
title: Confrontare l’efficacia dei canali con l’analizzatore di programmi
exl-id: bfe635a7-b077-4074-889d-fc2256102cd5
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 1%

---

# Confronta l&#39;efficacia del canale con [!UICONTROL Program Analyzer] {#compare-channel-effectiveness-with-the-program-analyzer}

Utilizza [!UICONTROL Program Analyzer] per confrontare i costi del canale, l&#39;acquisizione dei membri, la pipeline, i ricavi e altro ancora, per identificare i canali più efficaci e meno efficaci.

>[!PREREQUISITES]
>
>[Crea un [!UICONTROL Program Analyzer]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. Fai clic su **[!UICONTROL Analytics]** in **Il mio Marketo**.

   ![](assets/image2014-9-17-18-3a36-3a13.png)

1. Seleziona il tuo analizzatore di programmi.

   ![](assets/image2014-9-17-18-3a36-3a40.png)

1. Cambia la visualizzazione in **[!UICONTROL By Channel]**.

   ![](assets/image2014-9-17-18-3a36-3a59.png)

1. Utilizzare il menu a discesa **[!UICONTROL X Axis]** per scegliere una metrica per l&#39;asse orizzontale. Iniziamo con **[!UICONTROL Program Cost]**.

   ![](assets/image2014-9-17-18-3a37-3a7.png)

1. Utilizzare il menu a discesa **[!UICONTROL Y Axis]** per scegliere una metrica per l&#39;asse verticale. In questo caso, **[!UICONTROL (FT) Pipeline Created]** sarà disponibile.

   ![](assets/image2014-9-17-18-3a37-3a50.png)

   >[!NOTE]
   >
   >Molte delle metriche selezionabili nell’analizzatore di programmi sono disponibili con calcoli di primo contatto (FT) e multi contatto (MT). È importante comprendere la [differenza tra l&#39;attribuzione FT e MT](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

1. Utilizzare il menu a discesa **[!UICONTROL Y Axis]** per scegliere **[!UICONTROL (MT) Pipeline Created]**.

   ![](assets/image2014-9-17-18-3a39-3a5.png)

   In questa visualizzazione di attribuzione multi-touch, vediamo che il canale del webinar ha più influenza sulla creazione della pipeline e costa meno rispetto ai canali Tradeshow e Online Advertising.

   Ora aggiungiamo altre due dimensioni.

1. Utilizza il menu a discesa **[!UICONTROL Bubble Size]** per selezionare una misura aggiuntiva, come **[!UICONTROL New Names]**.

   ![](assets/image2014-9-17-18-3a39-3a36.png)

1. Osserva come cambia il grafico.

   ![](assets/image2014-9-17-18-3a39-3a55.png)

   Il canale del webinar si riduce, come misurato da **[!UICONTROL New Names]**. Pur avendo molti iscritti, possiamo concludere che è meno efficace nel generare nuovi lead rispetto al canale Tradeshow.

1. Infine, utilizza il menu a discesa Colore per aggiungere la quarta dimensione. Selezionare **[!UICONTROL (FT) Revenue Won]**.

   ![](assets/image2014-9-17-18-3a41-3a7.png)

1. Osserva come cambiano i colori nel grafico.

   ![](assets/image2014-9-17-18-3a41-3a19.png)

   Dai colori, apprendiamo che il canale Tradeshow, la bolla più verde, ha influenzato i maggiori ricavi ottenuti, come misurato dall’attribuzione del primo contatto.

1. Ora, se modifichiamo la metrica Colore in **[!UICONTROL (MT) Revenue Won]**, notiamo che il canale Online Advertising, ora il più verde, ha influenzato più ricavi _nel tempo_ rispetto ai canali Webinar e Tradeshow.

   ![](assets/image2014-9-17-18-3a41-3a40.png)

Nel nostro esempio, vediamo che il canale Tradeshow è sia il più costoso (più a destra) che il più riuscito (più alto sull’asse Y) quando si misura la pipeline creata con il primo contatto. Consideriamo ora la pipeline di ogni canale creata in base all’attribuzione multi-touch.

>[!TIP]
>
>Gli esempi in questi passaggi misurano l’efficacia in base alla pipeline creata. Utilizza il menu a discesa [!UICONTROL Y Axis] per selezionare altri modi di misurare l&#39;efficacia del canale, come [!UICONTROL New Names], [!UICONTROL Members], [!UICONTROL Cost per Success], ecc.

>[!MORELIKETHIS]
>
>* [Esplora i dettagli del programma e del canale con [!UICONTROL Program Analyzer]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)
>* [Confronta l&#39;efficacia del programma con [!UICONTROL Program Analyzer]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-program-effectiveness-with-the-program-analyzer.md)
