---
unique-page-id: 9437340
description: Scopri come implementare rtp utilizzando Tealium Tag Manager in Marketo Engage, incluso l’implementazione di rtp utilizzando dnl. Utilizza questa guida per completare il passaggio successivo.
title: Implementazione di RTP con Tealium Tag Manager
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
feature: Web Personalization
TQID: https://experienceleague.adobe.com/zMs2Dii5RERdH8tKb86a6EhxXUx2IpbZkDOCklUvvY4
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: e2290edd-b061-4880-9d79-dee306cf5aa9id: ea90ebee-5c84-42d9-8b21-006bdabc95a3id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bccid: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 201
ht-degree: 5%

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

1. Scegliere **[!UICONTROL Manage Templates]** dal menu [!UICONTROL Admin] in [!UICONTROL Account Admin].

1. Selezionare **[!UICONTROL Tealium Custom Container]: Marketo RTP** dall&#39;elenco a discesa per aprire il modello di tag.

1. Accedi al tuo account RTP.

1. Passa a [!UICONTROL Account Settings].

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
