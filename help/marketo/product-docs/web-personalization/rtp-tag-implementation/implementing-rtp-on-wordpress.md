---
unique-page-id: 4720149
description: Implementazione di RTP su Wordpress - Documentazione di Marketo - Documentazione del prodotto
title: Implementazione di RTP su Wordpress
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# Implementazione di RTP su [!DNL Wordpress] {#implementing-rtp-on-wordpress}

Per implementare [!UICONTROL RTP tag], seguire le istruzioni di installazione riportate di seguito:

1. Apri il file **header.php** del tema **[!DNL WordPress]**.

   È possibile utilizzare un client FTP per accedere al server o modificare i file dei temi direttamente dal dashboard [!DNL WordPress]. L&#39;editor di file si trova nella scheda **[!UICONTROL Appearance]** nel menu della barra laterale.

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. Nell&#39;elenco dei file modello a destra dell&#39;editor di testo, trovare **header.php** e aprirlo.

1. Vai a **[!UICONTROL Account Settings]**.

   a. Se hai già ricevuto il tag JavaScript dal Supporto tecnico - continua con il passaggio 5.

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. In [!UICONTROL Domain], individuare il dominio pertinente e fare clic su **[!UICONTROL Generate Tag]**.

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. Copia il tag JavaScript RTP e incollalo nei modelli del tuo sito web.

   a. Assicurarsi che sia il primo script nell&#39;intestazione della pagina, tra i tag **`<head> </head>`**.

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. Fare clic su **[!UICONTROL Update File]** per il file header.php.

1. Verifica che venga visualizzato in tutte le pagine, incluse le pagine di destinazione e i sottodomini.

   a. Per farlo, fai clic con il pulsante destro del mouse sulla pagina del sito web. Vai a **[!UICONTROL View Page Source].** Cerca **RTP** per individuare il tag.
