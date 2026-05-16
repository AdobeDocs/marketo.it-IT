---
unique-page-id: 4719332
description: Scopri come distribuire il JavaScript rtp in Marketo Engage, incluso rtp javascript. Utilizza questa guida per completare il passaggio successivo.
title: Distribuire il JavaScript RTP
exl-id: ef96a7f4-3942-4325-bb0f-7647ff2b33b6
feature: Web Personalization
TQID: https://experienceleague.adobe.com/XUylNa8clUib-aMhpAR8fjeu4pHRA8KSQydSH1AVxF8
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 171
ht-degree: 5%

---

# Distribuire il JavaScript RTP {#deploy-the-rtp-javascript}

Per generare e configurare il tag RTP, seguire le istruzioni di installazione riportate di seguito

## [!UICONTROL Generate Tag] {#generate-tag}

1. Accedi al tuo account RTP. Passa a **[!UICONTROL Account Settings]**.

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. In **[!UICONTROL Domain]** e **[!UICONTROL Domain Configuration]**, individuare il dominio pertinente e fare clic su **[!UICONTROL Generate Tag]**.

   ![](assets/image2014-12-1-23-3a5-3a35.png)

1. Copiare e incollare il tag Web Personalization (RTP) nel sito Web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copiare il tag JavaScript RTP e incollarlo come primo script nell&#39;intestazione delle pagine, tra i tag `<head> </head>`.

   Assicurati che il tag venga visualizzato su tutte le pagine, incluse le pagine di destinazione e i sottodomini. Per verificarlo, fai clic con il pulsante destro del mouse sulla pagina del tuo sito web. Vai a Visualizza Source pagina in un browser web. Ricerca: &quot;RTP&quot;.

1. [!UICONTROL Tag] impostato su **[!UICONTROL ON]**.

   Verificare che l&#39;interruttore [!UICONTROL Tag] sia impostato su [!UICONTROL ON]. Dovresti iniziare a visualizzare il flusso di dati nella scheda dell’organizzazione.

   Ora hai impostato con il tag RTP e sei pronto per iniziare a [creare segmenti](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) e campagne in tempo reale.

1. Verifica che il tag sia su tutte le pagine.
