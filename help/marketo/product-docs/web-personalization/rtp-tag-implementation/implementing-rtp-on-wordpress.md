---
unique-page-id: 4720149
description: Scopri come implementare rtp su wordpress in Marketo Engage, inclusa l’implementazione di rtp su dnl wordpress. Utilizza questa guida per completare il passaggio successivo.
title: Implementazione di RTP su Wordpress
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
feature: Web Personalization
TQID: https://experienceleague.adobe.com/5V3CEgasEJi4zrYoezh8Tt340VGHNNHaliF2wdbBLwY
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: e2290edd-b061-4880-9d79-dee306cf5aa9id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bccid: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 189
ht-degree: 3%

---

# Implementazione di RTP su [!DNL Wordpress] {#implementing-rtp-on-wordpress}

Per implementare [!UICONTROL RTP tag], seguire le istruzioni di installazione riportate di seguito:

1. Apri il file **header.php** del tema **[!DNL WordPress]**.

   È possibile utilizzare un client FTP per accedere al server o modificare i file dei temi direttamente dal dashboard [!DNL WordPress]. L&#39;editor di file si trova nella scheda **[!UICONTROL Appearance]** nel menu della barra laterale.

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. Nell&#39;elenco dei file modello a destra dell&#39;editor di testo, trovare **header.php** e aprirlo.

1. Passa a **[!UICONTROL Account Settings]**.

   a. Se hai già ricevuto il tag JavaScript dal Supporto tecnico - continua con il passaggio 5.

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. In [!UICONTROL Domain], individuare il dominio pertinente e fare clic su **[!UICONTROL Generate Tag]**.

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. Copia il tag JavaScript RTP e incollalo nei modelli del tuo sito web.

   a. Verificare che si tratti del primo script nell&#39;intestazione della pagina, tra i tag **`<head> </head>`**.

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. Fare clic su **[!UICONTROL Update File]** per il file header.php.

1. Verifica che venga visualizzato in tutte le pagine, incluse le pagine di destinazione e i sottodomini.

   a. A tale scopo, fai clic con il pulsante destro del mouse sulla pagina del sito web. Vai a **[!UICONTROL View Page Source].** Cerca **RTP** per individuare il tag.
