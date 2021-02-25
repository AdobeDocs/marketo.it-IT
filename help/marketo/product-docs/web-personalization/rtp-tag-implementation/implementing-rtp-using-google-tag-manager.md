---
unique-page-id: 4720145
description: Implementazione di RTP tramite Google Tag Manager - Marketo Docs - Documentazione prodotto
title: Implementazione di RTP tramite Google Tag Manager
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 0%

---


# Implementazione RTP tramite Google Tag Manager {#implementing-rtp-using-google-tag-manager}

Per implementare il tag RTP, segui le istruzioni di installazione riportate di seguito.

1. Accedi al tuo account Google Tag Manager.

1. Aggiungi un nuovo tag > Configurazioni tag > Tag HTML personalizzato*.** Chiamarla **RTP**.

1. Accedi al tuo account RTP**.**

1. Vai a **Impostazioni account**.

   a. Se avete già ricevuto il tag JavaScript dal supporto tecnico, continuate con il passaggio 6.

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. In Domain (Dominio), individua il dominio appropriato e fai clic su **Generate Tag**.

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. Copiate il tag JavaScript RTP e incollatelo nel nuovo **tag HTML personalizzato** creato (Passaggio 1).

1. Fare clic su **+Aggiungi regola al tag Fire**. Selezionare **Tutte le pagine**.

1. Fare clic su **Salva** e [pubblica la nuova versione](https://support.google.com/tagmanager/answer/2699097?hl=en).

1. Verifica che venga visualizzato su tutte le pagine, incluse le pagine di destinazione e i sottodomini.

   a. A tale scopo, fate clic con il pulsante destro del mouse sulla pagina del sito Web. Andate a **Inspect Element**, cercate **RTP** per individuare il tag.
