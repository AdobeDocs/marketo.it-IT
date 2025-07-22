---
unique-page-id: 14352540
description: Impedire visualizzazioni automatiche - Documentazione di Marketo - Documentazione del prodotto
title: Impedire visualizzazioni automatiche
exl-id: c18715fc-4ca2-4a6b-8f63-a9406f30c0d8
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# Impedire visualizzazioni automatiche {#preventing-self-views}

## Panoramica {#overview}

Ottenere falsi positivi per il tracciamento delle visualizzazioni può causare incongruenze nei rapporti. Ciò si verifica spesso quando gli utenti di MSC richiamano accidentalmente il pixel di tracciamento dal proprio client e-mail (questa funzione viene chiamata visualizzazione automatica). Di seguito sono riportati alcuni suggerimenti su come ridurre ed eliminare in modo significativo le visualizzazioni personali.

## Web ([!DNL Outlook Web App] e Gmail) {#web-outlook-web-app-and-gmail}

[!DNL Sales Connect] memorizzerà un cookie nel browser per impedire il rilevamento delle visualizzazioni all&#39;apertura delle e-mail da Outlook Web App e Gmail. Se ricevi ancora visualizzazioni personali, ti consigliamo di effettuare le seguenti operazioni:

* Verificare che nel computer siano abilitati i cookie.

* Se utilizzi un nuovo computer o dispositivo mobile, assicurati di aver effettuato l’accesso all’applicazione web. In questo modo sarà possibile riconoscere il computer o il dispositivo in uso.

## Desktop (Windows) {#desktop-windows}

Le visualizzazioni vengono tracciate scaricando un piccolo pixel di immagine invisibile nel client e-mail. È possibile ridurre in modo significativo la quantità di visualizzazioni automatiche in [!DNL Outlook] disabilitando il download automatico delle immagini. Di seguito sono riportati i passaggi come.

1. In [!DNL Outlook], fare clic su **[!UICONTROL File]** nella barra dei menu.

   ![](assets/win-1.png)

1. Fai clic su **[!UICONTROL Options]**.

   ![](assets/win-2.png)

1. Nella finestra di dialogo Opzioni [!DNL Outlook] fare clic su **[!UICONTROL Trust Center]**.

   ![](assets/win-3.png)

1. In [!UICONTROL Microsoft Outlook Trust Center], fare clic su **[!UICONTROL Trust Center Settings]**.

   ![](assets/win-4.png)

1. Fare clic su [!UICONTROL Automatic Download] nel menu a sinistra e selezionare la casella di controllo **[!UICONTROL Don't download pictures automatically in HTML email or RSS items]**.

   ![](assets/win-5.png)

1. Fare clic su **[!UICONTROL OK]** nella finestra di dialogo [!UICONTROL Trust Center].

   ![](assets/win-6.png)

1. Fare clic su **[!UICONTROL OK]** nella finestra di dialogo Opzioni [!DNL Outlook].

   ![](assets/win-6.png)

## Desktop (Mac) {#desktop-mac}

Le visualizzazioni vengono tracciate scaricando un piccolo pixel di immagine invisibile nel client e-mail. È possibile ridurre in modo significativo la quantità di visualizzazioni automatiche in [!DNL Outlook] disabilitando il download automatico delle immagini. Di seguito sono riportati i passaggi come.

1. In [!DNL Outlook], fare clic su **[!UICONTROL Outlook]** nella barra dei menu e selezionare **[!UICONTROL Preferences]**.

   ![](assets/mac-1.png)

1. In [!UICONTROL Email] scegliere **[!UICONTROL Reading]**.

   ![](assets/mac-2.png)

1. In [!UICONTROL Security] fare clic sul pulsante di opzione **[!UICONTROL Never]**.

   ![](assets/mac-3.png)
