---
unique-page-id: 4720215
description: Scopri come implementare rtp su wordpress enterprise in Marketo Engage, incluso l’implementazione di rtp su wordpress. Utilizza questa guida per completare il passaggio successivo.
title: Implementazione di RTP su Wordpress Enterprise
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
feature: Web Personalization
source-git-commit: 50befbf7339cd7a8b25b0942515497f6acc8f9ab
workflow-type: tm+mt
source-wordcount: '109'
ht-degree: 11%

---

# Implementazione di RTP su Wordpress Enterprise {#implementing-rtp-on-wordpress-enterprise}

Per implementare [!UICONTROL RTP tag], seguire le istruzioni di installazione riportate di seguito:

1. Passa a **[!UICONTROL Account Settings]**.

   a. Se hai già ricevuto il tag JavaScript dal Supporto tecnico - continua con il passaggio 3.

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. In [!UICONTROL Domain], individuare il dominio pertinente e fare clic su **[!UICONTROL Generate Tag]**.

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. Copia il tag JavaScript RTP.

1. Accedi al tuo account [!DNL WordPress] come utente amministratore

   a. Sotto **[!UICONTROL Appearance]**, vai a **[!UICONTROL Custom JavaScript]**.
b. Incolla il tag JavaScript RTP subito dopo il codice esistente.

   ![](assets/image2014-12-3-17-3a51-3a46.png)

   >[!CAUTION]
   >
   >Quando si incolla il codice, ESCLUDI i seguenti tag:
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`
   >
   >Inserire SOLO lo script stesso.

1. Fai clic su **[!UICONTROL Update]**.
