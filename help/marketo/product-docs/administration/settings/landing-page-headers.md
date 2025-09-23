---
description: Intestazioni pagina di destinazione - Documentazione Marketo - Documentazione del prodotto
title: Intestazioni pagina di destinazione
exl-id: 58eaa0cd-2a2b-4abe-9180-f60a2a1dcc87
feature: Administration, Landing Pages
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '122'
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
