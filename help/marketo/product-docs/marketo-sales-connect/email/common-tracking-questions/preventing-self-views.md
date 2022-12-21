---
unique-page-id: 14352540
description: Prevenzione delle visualizzazioni automatiche - Documenti Marketo - Documentazione del prodotto
title: Impedire visualizzazioni automatiche
exl-id: c18715fc-4ca2-4a6b-8f63-a9406f30c0d8
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 0%

---

# Impedire visualizzazioni automatiche {#preventing-self-views}

## Panoramica {#overview}

Ottenere falsi positivi sul tracciamento delle visualizzazioni può portare a incongruenze nel reporting. Questo si verifica spesso quando gli utenti di MSC richiamano accidentalmente il pixel di tracciamento dal loro client e-mail (lo chiamiamo visualizzazione automatica). Di seguito sono riportati alcuni suggerimenti su ridurre in modo significativo e persino eliminare le visualizzazioni di sé.

## Web (Outlook Web App e Gmail) {#web-outlook-web-app-and-gmail}

Sales Connect memorizzerà un cookie nel browser per impedire il tracciamento delle visualizzazioni quando si aprono le e-mail da Outlook Web App e Gmail. Se ricevi ancora visualizzazioni personali, ti consigliamo di effettuare le seguenti operazioni:

* Assicurati che nel computer siano abilitati i cookie.

* Se utilizzi un nuovo computer o dispositivo mobile, assicurati di aver effettuato l’accesso all’applicazione web. Questo ci permetterà di riconoscere il vostro computer/dispositivo in futuro.

## Desktop (Windows) {#desktop-windows}

Le visualizzazioni vengono tracciate scaricando un piccolo pixel immagine invisibile nel client e-mail. È possibile ridurre notevolmente la quantità di visualizzazioni automatiche in Outlook disattivando le immagini da scaricare automaticamente. Di seguito sono riportati i passaggi da seguire.

1. In Outlook, fai clic su **File** nella barra dei menu.

   ![](assets/win-1.png)

1. Fai clic su **Opzioni**.

   ![](assets/win-2.png)

1. Nella finestra di dialogo Opzioni di Outlook fare clic su **Centro protezione**.

   ![](assets/win-3.png)

1. In Centro protezione di Microsoft Outlook fare clic su **Impostazioni del Centro protezione**.

   ![](assets/win-4.png)

1. Fai clic su Scarica automaticamente nel menu a sinistra, quindi seleziona il **Non scaricare automaticamente le immagini nelle e-mail di HTML o negli elementi RSS** casella di controllo.

   ![](assets/win-5.png)

1. Fai clic su **OK** nella finestra di dialogo Centro protezione.

   ![](assets/win-6.png)

1. Fai clic su **OK** nella finestra di dialogo Opzioni di Outlook.

   ![](assets/win-6.png)

## Desktop (Mac) {#desktop-mac}

Le visualizzazioni vengono tracciate scaricando un piccolo pixel immagine invisibile nel client e-mail. È possibile ridurre notevolmente la quantità di visualizzazioni automatiche in Outlook disattivando le immagini da scaricare automaticamente. Di seguito sono riportati i passaggi da seguire.

1. In Outlook, fai clic su **Outlook** nella barra dei menu e seleziona **Preferenze**.

   ![](assets/mac-1.png)

1. In E-mail, scegli **Lettura**.

   ![](assets/mac-2.png)

1. In Sicurezza, fai clic sul pulsante **Mai** pulsante di scelta.

   ![](assets/mac-3.png)
