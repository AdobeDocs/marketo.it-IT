---
unique-page-id: 3571886
description: Utilizzo di Success Path Analyzer - Marketo Docs - Documentazione del prodotto
title: Utilizzo di Success Path Analyzer
exl-id: f816b7ac-a158-46bd-9d00-09ef4cc8b381
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# Utilizzo di Success Path Analyzer {#using-the-success-path-analyzer}

Utilizza un Analisi di percorso di successo per esplorare i dettagli specifici che riflettono sia il flusso (quantità) che la velocità (in termini di giorni) delle persone nelle fasi del tuo [Modello del ciclo dei ricavi](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md).

>[!PREREQUISITES]
>
>[Creare un analizzatore del percorso di successo](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/create-a-success-path-analyzer.md)

1. Vai a **Analytics** e seleziona la **Analisi del percorso di successo**.

   ![](assets/image2015-6-12-17-3a23-3a53.png)

   Il grafico a destra riflette i dati presenti nel pulsante selezionato a sinistra. Per impostazione predefinita, si tratta di Balance.

1. Fai clic su **In Flusso** per rappresentare il numero di persone che sono entrate nell’area di visualizzazione durante l’intervallo di tempo selezionato.

   ![](assets/image2015-6-12-17-3a30-3a52.png)

   * Fai clic su Out Flow (Flusso di uscita) per rappresentare il numero di persone uscite dal palco.
   * Fai clic su Conv % per rappresentare il tasso di conversione da questo a quello successivo.
   * Fai clic su Tempo medio per vedere quanto tempo hanno trascorso le persone in questa fase prima di passare alla fase successiva.

1. Fai clic su **Azioni grafico** > Confronta periodo per confrontare i dati con un intervallo di tempo diverso di uguale lunghezza.

   ![](assets/image2015-6-12-17-3a39-3a15.png)

1. Seleziona la **Da** data del periodo di confronto.

   ![](assets/image2015-6-12-17-3a43-3a49.png)

   La **A** la data viene impostata automaticamente in modo che corrisponda alla lunghezza del periodo di tempo originale.

1. Fai clic su **Confronto**.

   ![](assets/image2015-6-12-17-3a44-3a8.png)

1. Il grafico si aggiorna con i dati sovrapposti per il periodo di confronto, in verde.

   ![](assets/image2015-6-12-17-3a46-3a16.png)

1. Per modificare la scala temporale del grafico, fare clic su una delle **Grafico di** pulsanti: giornaliero (predefinito), settimanale e mensile

   ![](assets/image2015-6-12-17-3a46-3a55.png)

1. Per le fasi con gli SLA (Accordi a livello di servizio), fai clic su **Azioni grafico** > **Mostra scadenza SLA** mostrare a ogni persona che ha mancato un target SLA entro il periodo di tempo specificato.

   ![](assets/image2015-6-12-17-3a49-3a23.png)

1. Il grafico si aggiorna per riflettere il numero di SLA dovuti su ciascun nodo, in arancione.

   ![](assets/image2015-6-12-17-3a50-3a16.png)

   Le persone visualizzate in arancione potrebbero *o* essere ancora nella fase SLA.

1. Fai clic su **Azioni grafico** > **Mostra SLA scaduto** mostrare a tutte le persone con target SLA scaduti che si trovano ancora nella fase SLA al termine del periodo di tempo specificato.

   ![](assets/image2015-6-12-17-3a51-3a39.png)

1. Il grafico viene aggiornato per riflettere il numero di SLA scaduti su ciascun nodo, in arancione.

   ![](assets/image2015-6-12-17-3a52-3a17.png)

1. Per leggere i dettagli specifici di un punto dati su un nodo specifico (data), passa il puntatore del mouse sulla bolla.

   ![](assets/image2015-6-12-17-3a52-3a49.png)

1. Per stampare il grafico, fare clic su **Azioni grafico** > **Stampa grafico**.

   ![](assets/image2015-6-12-17-3a53-3a34.png)

L&#39;analizzatore è qui per aiutarvi a comprendere il movimento attraverso il vostro modello. Con l&#39;avanzare dei progressi, questo diventerà molto importante per strategizzare le tue attività di marketing.
