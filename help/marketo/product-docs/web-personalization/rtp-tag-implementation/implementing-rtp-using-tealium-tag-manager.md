---
unique-page-id: 9437340
description: Implementazione di RTP con Tealium Tag Manager - Documentazione di Marketo - Documentazione del prodotto
title: Implementazione di RTP con Tealium Tag Manager
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 1%

---

# Implementazione di RTP tramite [!DNL Tealium] Tag Manager {#implementing-rtp-using-tealium-tag-manager}

Per implementare il tag RTP, seguire le istruzioni di installazione riportate di seguito.

1. Accedi al tuo account di [!DNL Tealium] Tag Manager.

1. Passare alla scheda [!UICONTROL Tags] e aggiungere [!UICONTROL Tealium Custom Container Tag], che si trova nella scheda [!UICONTROL Misc] del marketplace dei tag.

1. In [!UICONTROL Title field], immettere **RTP Marketo** e fare clic su **[!UICONTROL Finish]**.

1. Salva le modifiche.

   >[!NOTE]
   >
   >Non è ancora necessario pubblicare il nuovo contenitore.

1. Dopo aver salvato il profilo, fai clic sul tuo nome/indirizzo e-mail nell’angolo superiore destro della console Tealium iQ.

1. Scegliere [!UICONTROL Admin] dal menu **[!UICONTROL Manage Templates]** in [!UICONTROL Account Admin].

1. Selezionare **[!UICONTROL Tealium Custom Container]: Marketo RTP** dall&#39;elenco a discesa per aprire il modello di tag.

1. Accedi al tuo account RTP.

1. Vai a [!UICONTROL Account Settings].

   >[!NOTE]
   >
   >Se hai già ricevuto il tuo tag JavaScript dal Supporto, continua con il passaggio 11.

1. In Dominio individuare il dominio pertinente e fare clic su **[!UICONTROL Generate Tag]**.

1. Copiare il tag JavaScript RTP e incollarlo tra [!UICONTROL Start Tag Library Code] e [!UICONTROL End Tag Library Code] nel modello di profilo Tealium.

   >[!NOTE]
   >
   >**Passaggi importanti**
   >
   >Rimuovere i tag `<!-- RTP tag -->` e `<!-- End of RTP tag -->` dal codice inserito nel file.
   >
   >Rimuovere i tag `<script type='text/javascript'>` e `</script>` dal codice inserito nel file.

1. Fai clic su **[!UICONTROL Save Profile Template]** e pubblica il nuovo profilo.
