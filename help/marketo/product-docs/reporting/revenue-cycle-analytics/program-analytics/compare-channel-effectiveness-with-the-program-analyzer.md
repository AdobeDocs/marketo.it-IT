---
unique-page-id: 2360401
description: Confrontare l’efficacia dei canali con Program Analyzer - Marketo Docs - Documentazione del prodotto
title: Confrontare l'efficacia dei canali con Program Analyzer
exl-id: bfe635a7-b077-4074-889d-fc2256102cd5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# Confrontare l&#39;efficacia dei canali con Program Analyzer {#compare-channel-effectiveness-with-the-program-analyzer}

Utilizza Program Analyzer per confrontare i costi dei canali, l&#39;acquisizione dei membri, la pipeline, i ricavi e altro ancora, per identificare i canali più efficaci e meno efficaci.

>[!PREREQUISITES]
>
>[Creare un’analisi dei programmi](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. Fai clic su **Analytics** in **My Marketo**.

   ![](assets/image2014-9-17-18-3a36-3a13.png)

1. Seleziona la tua **Analisi del programma**.

   ![](assets/image2014-9-17-18-3a36-3a40.png)

1. Cambia la visualizzazione in **Per canale**.

   ![](assets/image2014-9-17-18-3a36-3a59.png)

1. Utilizza la **Asse X** menu a discesa per scegliere una metrica per l’asse orizzontale. Cominciamo con **Costo del programma**.

   ![](assets/image2014-9-17-18-3a37-3a7.png)

1. Utilizza il menu a discesa Asse Y per scegliere una metrica per l’asse verticale. Ecco, andiamo con **(FT) Pipeline creata**.

   ![](assets/image2014-9-17-18-3a37-3a50.png)

   >[!NOTE]
   >
   >Molte delle metriche che è possibile scegliere nell&#39;analizzatore di programmi sono disponibili con calcoli di primo contatto (FT) e multi-touch (MT). È importante comprendere il [differenza tra l’attribuzione FT e MT](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

1. Utilizza la **Asse Y** menu a discesa per scegliere **(MT) Pipeline creata**.

   ![](assets/image2014-9-17-18-3a39-3a5.png)

   In questa visualizzazione di attribuzione multi-touch, vediamo che il canale Webinar ha più influenza sulla pipeline creata e costa meno dei canali di Tradeshow e Online Advertising.

   Ora aggiungiamo altre due dimensioni!

1. Utilizza la **Dimensioni bolle** a discesa per selezionare una misura aggiuntiva, ad esempio **Nuovi nomi**.

   ![](assets/image2014-9-17-18-3a39-3a36.png)

1. Guarda come cambia il grafico.

   ![](assets/image2014-9-17-18-3a39-3a55.png)

   Vediamo che il canale Webinar si restringe, come misurato da **Nuovi nomi**. Possiamo concludere che, pur avendo molti membri, è meno efficace nel generare nuovi lead rispetto al canale Tradeshow.

1. Infine, utilizza il menu a discesa Colore per aggiungere la quarta dimensione. Seleziona **(FT) Entrate vinte**.

   ![](assets/image2014-9-17-18-3a41-3a7.png)

1. Guardate come cambiano i colori nel grafico.

   ![](assets/image2014-9-17-18-3a41-3a19.png)

   Dai colori, impariamo che il canale Tradeshow, la bolla più verde, ha influenzato i maggiori ricavi ottenuti, misurati dall’attribuzione di primo contatto.

1. Ora, se cambiamo la metrica Colore in **(MT) Entrate vinte**, vediamo che il canale della pubblicità online, ora il più verde, ha influenzato più entrate -nel tempo_ dei canali del Webinar e del Tradeshow.

   ![](assets/image2014-9-17-18-3a41-3a40.png)

Nel nostro esempio, vediamo che il canale Tradeshow è sia il più costoso (più lontano a destra) che il più efficace (più alto sull’asse Y) durante la misurazione della pipeline creata dal primo contatto. Consideriamo ora la pipeline di ogni canale creata in base all’attribuzione multi-touch.

>[!TIP]
>
>Gli esempi in questi passaggi misurano l’efficacia in base alla pipeline creata. Utilizza il menu a discesa Asse Y per selezionare altri modi per misurare l’efficacia del canale, come Nuovi nomi, Membri, Costo per successo, ecc.

>[!MORELIKETHIS]
>
>* [Esplorare i dettagli del programma e del canale con Program Analyzer](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)
>* [Confrontare l&#39;efficacia del programma con Program Analyzer](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-program-effectiveness-with-the-program-analyzer.md)

