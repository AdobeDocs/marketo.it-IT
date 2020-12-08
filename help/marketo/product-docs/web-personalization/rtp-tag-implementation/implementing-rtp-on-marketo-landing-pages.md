---
unique-page-id: 4720151
description: Implementazione di RTP sulle pagine di destinazione Marketo - Marketo Docs - Documentazione prodotto
title: Implementazione di RTP sulle pagine di destinazione Marketo
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# Implementazione di RTP sulle pagine di destinazione Marketo {#implementing-rtp-on-marketo-landing-pages}

Per implementare il tag RTP, segui le istruzioni di installazione riportate di seguito:

1. Andate a **Design Studio.** Aprite l’elemento da modificare. Selezionate Azioni **** modello, selezionate **Modifica bozza**

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. Apportate le modifiche necessarie al modello nella scheda Sorgente **** HTML.

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. Nel tuo account RTP, vai a** Impostazioni account.**

1. Se avete già ricevuto il tag JavaScript dal supporto, continuate con il passaggio 5.

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. In Dominio, individua il dominio appropriato e fai clic su **Genera tag**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. Copiate il tag JavaScript RTP e incollatelo in tutti i modelli della pagina di destinazione tra i **`<head> </head>`** tag .
1. Fare clic su **Salva** e **chiudere** la finestra.
1. In **Design Studio**, approva la pagina di destinazione da Azioni **** modello, fai clic su **Approva**.\
   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. Infine, per rendere effettive le modifiche apportate al modello, sarà necessario **approvare** nuovamente tutte le pagine di destinazione che utilizzano tale modello. Potete riapprovarle tutte contemporaneamente dalla sezione Pagine di destinazione principale.

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. Verifica che venga visualizzato su tutte le pagine di `pages including` destinazione e i sottodomini.

   Per eseguire questa operazione, fare clic con il pulsante destro del mouse sulla `website’s` pagina. Vai a **Visualizza origine pagina.** Cercate **RTP** per individuare il tag.
