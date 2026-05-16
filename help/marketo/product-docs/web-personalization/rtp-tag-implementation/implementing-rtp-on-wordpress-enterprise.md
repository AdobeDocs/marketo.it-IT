---
unique-page-id: 4720215
description: Scopri come implementare rtp su wordpress enterprise in Marketo Engage, incluso l’implementazione di rtp su wordpress. Utilizza questa guida per completare il passaggio successivo.
title: Implementazione di RTP su Wordpress Enterprise
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
feature: Web Personalization
TQID: https://experienceleague.adobe.com/S0LvRrD1V6hkWN5L5TlnoaIqcDvXLjfm5do2-1WQTNw
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: e2290edd-b061-4880-9d79-dee306cf5aa9id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 109
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

   a. In **[!UICONTROL Appearance]**, vai a **[!UICONTROL Custom JavaScript]**.
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
