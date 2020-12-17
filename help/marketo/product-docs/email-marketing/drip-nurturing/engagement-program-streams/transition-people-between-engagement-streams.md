---
unique-page-id: 2359947
description: Transizione tra i flussi di coinvolgimento - Marketo Docs - Documentazione del prodotto
title: Persone Di Transizione Tra I Flussi Di Coinvolgimento
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---


# Persone di transizione tra flussi di coinvolgimento {#transition-people-between-engagement-streams}

I programmi di coinvolgimento possono avere più di un flusso. Se [aggiungete un flusso](../../../../product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md), è necessario definire un modo per consentire agli utenti di spostarsi da un flusso all&#39;altro. Tali regole sono denominate **regole di transizione.**

1. Andate a **Marketing Activities**.

   ![](assets/ma.png)

1. Selezionate il programma di coinvolgimento con più flussi e passate a **Streams**.

   ![](assets/multistream.jpg)

1. Fare clic su **Regole di transizione** per il flusso in cui si desidera eseguire il pulling da altri flussi, quindi fare clic su **Edit Transition Rules. **

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >Le regole di transizione entrano in un flusso; definire sempre le regole del flusso in cui si desidera eseguire il pull.

   Una volta aperta la finestra della regola di transizione, trova e trascina il trigger desiderato. In questo caso, vogliamo spostare le persone in fase intermedia quando viene aggiunta a un&#39;opportunità.
` ![](assets/image2014-9-15-18-3a10-3a46.png)

   `

1. Impostiamo l&#39;operatore su** è qualsiasi** in modo che le persone si spostino per ogni opportunità aggiunta.

   ` ![](assets/image2014-9-15-18-3a11-3a14.png)

   `

   >[!TIP]
   >
   >Potete aggiungere più attivatori e filtri a una regola di transizione, ma la regola di transizione utilizza tutti i filtri (l&#39;uso di TUTTI i filtri è l&#39;unica opzione). Se è necessario utilizzare O in una regola di transizione, è consigliabile impostare una campagna smart esterna.

1. Fare clic su **Chiudi**.

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   Fantastico! Ora qualsiasi persona nel programma di coinvolgimento che viene aggiunta a un&#39;opportunità verrà spostata nel flusso Mid Stage.

   ` ![](assets/image2014-9-15-18-3a11-3a29.png)

   `

   >[!NOTE]
   >
   >I passaggi descritti sopra *do* si applicano anche alle persone [in pausa](http://docs.marketo.com/display/DOCS/Pause+People+in+an+Engagement+Program).

