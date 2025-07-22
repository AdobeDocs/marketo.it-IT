---
unique-page-id: 4720145
description: Implementazione di RTP tramite Google Tag Manager - Documentazione di Marketo - Documentazione del prodotto
title: Implementazione di RTP tramite Google Tag Manager
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# Implementazione di RTP tramite [!DNL Google Tag Manager] {#implementing-rtp-using-google-tag-manager}

Per implementare il tag RTP, seguire le istruzioni di installazione riportate di seguito.

1. Accedi al tuo account [!DNL Google Tag Manager].

1. Aggiungi un nuovo **[!UICONTROL Tag]** > **[!UICONTROL Tag Configurations]** > **[!UICONTROL Custom HTML Tag].** Chiamarlo **RTP**.

1. Accedi al tuo **account RTP**.

1. Vai a **[!UICONTROL Account Settings]**.

   a. Se hai già ricevuto il tag JavaScript dal Supporto, continua con il passaggio 6.

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. In [!UICONTROL Domain], individuare il dominio pertinente e fare clic su **[!UICONTROL Generate Tag]**.

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. Copiare il tag JavaScript RTP e incollarlo nel nuovo **tag HTML personalizzato** creato (passaggio 1).

1. Fare clic su **[!UICONTROL Add Rule to Fire Tag]**. Seleziona **[!UICONTROL All Pages]**.

1. Fai clic su **[!UICONTROL Save]** e [pubblica la nuova versione](https://support.google.com/tagmanager/answer/2699097?hl=en).

1. Verifica che venga visualizzato in tutte le pagine, incluse le pagine di destinazione e i sottodomini.

   a. Per farlo, fai clic con il pulsante destro del mouse sulla pagina del tuo sito web. Vai a **[!UICONTROL Inspect Element]**, cerca **RTP** per individuare il tag.
