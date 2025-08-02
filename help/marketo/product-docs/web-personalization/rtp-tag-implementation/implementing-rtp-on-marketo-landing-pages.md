---
unique-page-id: 4720151
description: Implementazione di RTP sulle pagine di destinazione di Marketo - Documentazione di Marketo - Documentazione del prodotto
title: Implementazione di RTP sulle pagine di destinazione di Marketo
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---

# Implementazione di RTP sulle pagine di destinazione di Marketo {#implementing-rtp-on-marketo-landing-pages}

Per implementare [!UICONTROL RTP tag], seguire le istruzioni di installazione riportate di seguito:

1. Passare a **[!UICONTROL Design Studio].** Aprire l&#39;elemento da modificare. Selezionare **[!UICONTROL Template Actions]**, selezionare **[!UICONTROL Edit Draft]**.

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
