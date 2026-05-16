---
description: Come personalizzare le intestazioni HTTP per i domini delle pagine di destinazione, tra cui Strict-Transport-Security e X-Frame-Options.
title: Intestazioni pagina di destinazione
exl-id: 58eaa0cd-2a2b-4abe-9180-f60a2a1dcc87
feature: Administration, Landing Pages
TQID: https://experienceleague.adobe.com/ecRuR4V-YCsesHZpm9UrP1rPlOjBCediq-9DtXZRfBo
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 134
ht-degree: 5%

---

# Intestazioni pagina di destinazione {#landing-page-headers}

Segui i passaggi seguenti per personalizzare alcune delle intestazioni HTTP nei domini della pagina di destinazione.

1. In Marketo, fare clic su **[!UICONTROL Admin]**.

   ![](assets/landing-page-headers-1.png)

1. Fai clic su **[!UICONTROL Landing Pages]**.

   ![](assets/landing-page-headers-2.png)

1. Fare clic su **[!UICONTROL Edit]** accanto a Intestazioni HTTP della pagina di destinazione.

   ![](assets/landing-page-headers-3.png)

1. Scegli le impostazioni desiderate e al termine fai clic su **[!UICONTROL Save]**.

   ![](assets/landing-page-headers-4.png)

<table>
 <tr>
  <td><strong>[!UICONTROL Strict-Transport-Security]</strong></td>
  <td>Utilizzalo per garantire che le connessioni alle pagine di destinazione vengano sempre servite tramite HTTPS (deve essere impostato solo per gli abbonamenti con pagine di destinazione protette da SSL)</td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL X-Frame-Options]</strong></td>
  <td>Consente di definire se le risorse in hosting Marketo Engage possono essere incorporate o meno in pagine web esterne</td>
 </tr>
</table>

>[!CAUTION]
>
>È importante rivedere queste impostazioni con il team IT per determinare su cosa devono essere impostati i criteri della tua organizzazione. Impostazioni errate possono impedire ad alcuni visitatori di accedere alle pagine di destinazione.
