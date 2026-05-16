---
unique-page-id: 4720145
description: Scopri come implementare rtp utilizzando google tag manager in Marketo Engage, incluso come implementare rtp utilizzando dnl google. Utilizza questa guida per completare il passaggio successivo.
title: Implementazione di RTP con Google Tag Manager
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
feature: Web Personalization
TQID: https://experienceleague.adobe.com/XesXGBf2aDsnsbS2Ro1RLdd1EVrj-mBdCiv8C0dj8NU
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
source-wordcount: 152
ht-degree: 6%

---

# Implementazione di RTP tramite [!DNL Google Tag Manager] {#implementing-rtp-using-google-tag-manager}

Per implementare il tag RTP, seguire le istruzioni di installazione riportate di seguito.

1. Accedi al tuo account [!DNL Google Tag Manager].

1. Aggiungi un nuovo **[!UICONTROL Tag]** > **[!UICONTROL Tag Configurations]** > **[!UICONTROL Custom HTML Tag].** Chiamalo **RTP**.

1. Accedi al tuo **account RTP**.

1. Passa a **[!UICONTROL Account Settings]**.

   a. Se hai già ricevuto il tuo tag JavaScript dal Supporto, continua con il Passaggio 6.

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. In [!UICONTROL Domain], individuare il dominio pertinente e fare clic su **[!UICONTROL Generate Tag]**.

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. Copiare il tag JavaScript RTP e incollarlo nel nuovo **tag HTML personalizzato** creato (passaggio 1).

1. Fai clic su **[!UICONTROL Add Rule to Fire Tag]**. Seleziona **[!UICONTROL All Pages]**.

1. Fai clic su **[!UICONTROL Save]** e [pubblica la nuova versione](https://support.google.com/tagmanager/answer/2699097?hl=en).

1. Verifica che venga visualizzato in tutte le pagine, incluse le pagine di destinazione e i sottodomini.

   a. A tale scopo, fai clic con il pulsante destro del mouse sulla pagina del tuo sito web. Vai a **[!UICONTROL Inspect Element]**, cerca **RTP** per individuare il tag.
