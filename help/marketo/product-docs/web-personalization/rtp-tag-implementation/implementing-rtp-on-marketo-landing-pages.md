---
unique-page-id: 4720151
description: Scopri come implementare rtp sulle pagine di destinazione di marketo in Marketo Engage, incluso l’implementazione di rtp su marketo. Utilizza questa guida per completare il passaggio successivo.
title: Implementazione di RTP sulle pagine di destinazione di Marketo
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
feature: Web Personalization
TQID: https://experienceleague.adobe.com/scyZfbFBloPu8JRfJiMjm62AFCHM7WCxaats3qssq2A
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d65b4a73-87a3-4d56-b638-74e74d9939ceid: e2290edd-b061-4880-9d79-dee306cf5aa9id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bccid: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 187
ht-degree: 6%

---

# Implementazione di RTP sulle pagine di destinazione di Marketo {#implementing-rtp-on-marketo-landing-pages}

Per implementare [!UICONTROL RTP tag], seguire le istruzioni di installazione riportate di seguito:

1. Vai a **[!UICONTROL Design Studio].** Apri l’elemento da modificare. Selezionare **[!UICONTROL Template Actions]**, selezionare **[!UICONTROL Edit Draft]**.

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. Apporta le modifiche al modello nella scheda **HTML Source**.

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. Nel tuo account RTP, vai a **[!UICONTROL Account Settings]**.

   a. Se hai già ricevuto il tag JavaScript dal Supporto tecnico - continua con il passaggio 5.

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. In [!UICONTROL Domain], individuare il dominio pertinente e fare clic su **[!UICONTROL Generate Tag]**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. Copiare il tag JavaScript RTP e incollarlo in tutti i modelli di pagina di destinazione tra i tag **`<head> </head>`**.

1. Fare clic su **[!UICONTROL Save]** e **[!UICONTROL Close]** nella finestra.

1. Tornando a **[!UICONTROL Design Studio]**, approva la pagina di destinazione da **[!UICONTROL Template Actions]**, fai clic su **[!UICONTROL Approve]**.

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. Infine, per rendere effettive le modifiche apportate al modello, **devi approvare nuovamente** le pagine di destinazione che utilizzano tale modello. È possibile approvarle nuovamente tutte contemporaneamente dalla sezione principale [!UICONTROL Landing Pages].

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. Verifica che venga visualizzato in tutte le pagine, incluse le pagine di destinazione e i sottodomini.

   A tale scopo, fai clic con il pulsante destro del mouse sulla pagina del sito web. Vai a **[!UICONTROL View Page Source].** Cerca **[!UICONTROL RTP]** per individuare il tag.
