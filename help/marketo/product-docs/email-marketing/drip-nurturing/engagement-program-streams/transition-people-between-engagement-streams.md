---
unique-page-id: 2359947
description: Transizione delle persone tra flussi di coinvolgimento - Documentazione di Marketo - Documentazione del prodotto
title: Transizione Delle Persone Tra Flussi Di Coinvolgimento
exl-id: 2367852c-3dcf-4188-a50c-7c6f0b0ff7bc
feature: Engagement Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Transizione Delle Persone Tra Flussi Di Coinvolgimento {#transition-people-between-engagement-streams}

I programmi di coinvolgimento possono avere più flussi. Se [aggiungi un flusso](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md), è necessario definire un modo in cui le persone possono spostarsi da un flusso all&#39;altro. Questi vengono chiamati **regole di transizione.**

1. Vai a **Attività di marketing**.

   ![](assets/ma.png)

1. Seleziona il tuo programma di coinvolgimento multi-streaming e vai a **Flussi**.

   ![](assets/multistream.jpg)

1. Clic **Regole di transizione** per il flusso in cui desideri richiamare da altri flussi, quindi fai clic su **Modifica regole di transizione**.

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >Le regole di transizione si estraggono in un flusso; definiscono sempre le regole del flusso in cui desideri essere estratti.

   Una volta aperta la finestra della regola di transizione, individua e trascina il trigger desiderato. In questo caso, vogliamo spostare le persone in Mid Stage quando viene aggiunta a un’opportunità.

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. Imposta l’operatore su **è qualsiasi** in modo che le persone si spostino per qualsiasi opportunità aggiunta.

   ![](assets/image2014-9-15-18-3a11-3a14.png)

   >[!TIP]
   >
   >È possibile aggiungere più trigger e filtri a una regola di transizione, ma la regola di transizione utilizza tutti i filtri (l’utilizzo di TUTTI i filtri è l’unica opzione). Se devi utilizzare l’operatore OR in una regola di transizione, ti consigliamo invece di impostare una campagna avanzata esterna.

1. Fai clic su **Chiudi**.

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   Fantastico! Ora qualsiasi persona nel programma di coinvolgimento aggiunta a un’opportunità verrà spostata nel flusso Mid Stage.

   ![](assets/image2014-9-15-18-3a11-3a29.png)

   >[!NOTE]
   >
   >I passaggi descritti sopra *fare* applica alle persone che sono [in pausa](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md) anche.
