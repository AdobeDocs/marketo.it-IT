---
unique-page-id: 4720218
description: Implementazione di RTP tramite Adobe Tag Manager - Documentazione di Marketo - Documentazione del prodotto
title: Implementazione di RTP con Adobe Tag Manager
exl-id: 5a938d02-6b09-45d5-94b0-dbb50b5d62b6
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 6%

---

# Implementazione di RTP con Adobe Tag Manager {#implementing-rtp-using-adobe-tag-manager}

Per implementare il tag RTP, seguire le istruzioni di installazione riportate di seguito:

1. Accedi al tuo account RTP.

1. Vai a **[!UICONTROL Account Settings]**.

   a. Se hai già ricevuto il tag JavaScript dal Supporto tecnico - continua con il passaggio 4.

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. In [!UICONTROL Domain], individuare il dominio pertinente e fare clic su **[!UICONTROL Generate Tag]**.

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. Accedi al tuo account [!DNL Dynamic Tag Manager] ([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in)).

1. Vai a **[!UICONTROL Dashboard].** Fare clic sulla relativa proprietà Web.

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. Vai a **[!UICONTROL Rules]**, fai clic su **[!UICONTROL Create New Rule]**.

1. Compila quanto segue

   1. [!UICONTROL Name]: **RTP Marketo**
   1. [!UICONTROL Conditions] (comprimi): regola di attivazione in - **[!UICONTROL Top of Page]**
   1. [!UICONTROL Javascript] (comprimi): fare clic su **[!UICONTROL Add New Script]**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. Chiama il nuovo tag: **Marketo RTP Tag**

1. Rimuovi il seguente codice da [!UICONTROL RTP tag]

   * `<script type='text/javascript'>`
   * `</script>`

1. Incolla il tag JavaScript RTP.

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >Assicurarsi di rimuovere tutti i tag e di lasciare solo lo script stesso (nessun `<script type='text/javascript'>` , `</script>` )

1. Fare clic su **[!UICONTROL Save Code]** nell&#39;editor di script e su **[!UICONTROL Save Rule]** nell&#39;editor di regole.

1. Nel pannello Regole, individua la regola di caricamento pagina Marketo RTP e seleziona **[!UICONTROL Actions]** nel menu a discesa **[!UICONTROL Activate Rules]**.

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **[!UICONTROL Verify]** visualizzato su tutte le pagine, incluse le pagine di destinazione e i sottodomini.

   Per farlo, fai clic con il pulsante destro del mouse sulle pagine del tuo sito web. Vai a **[!UICONTROL Inspect Element]**, fai clic su **[!UICONTROL Network]**, cerca: **RTP**.
