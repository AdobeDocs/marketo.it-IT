---
description: Intestazioni pagina di destinazione - Documenti Marketo - Documentazione del prodotto
title: Intestazioni pagina di destinazione
exl-id: 58eaa0cd-2a2b-4abe-9180-f60a2a1dcc87
source-git-commit: 05129f546cf2ba0df5c608485adf73c26d4b4f1e
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# Intestazioni pagina di destinazione {#landing-page-headers}

Segui i passaggi riportati di seguito per personalizzare alcune delle intestazioni HTTP sui domini della pagina di destinazione.

1. In Marketo, fai clic su **Amministratore**.

   ![](assets/landing-page-headers-1.png)

1. Fai clic su **Pagine di destinazione**.

   ![](assets/landing-page-headers-2.png)

1. Fai clic su **Modifica** accanto a Intestazioni HTTP della pagina di destinazione.

   ![](assets/landing-page-headers-3.png)

1. Scegli le impostazioni desiderate e fai clic su **Salva** al termine.

   ![](assets/landing-page-headers-4.png)

<table>
 <tr>
  <td><strong>Strict-Transport-Security</strong></td>
  <td>Utilizza questo per garantire che le connessioni alle pagine di destinazione vengano sempre servite tramite HTTPS (deve essere impostato solo per gli abbonamenti con pagine di destinazione protette da SSL)</td>
 </tr>
 <tr>
  <td><strong>Opzioni X-Frame</strong></td>
  <td>Consente di definire se le risorse ospitate dal Marketo Engage possono essere incorporate o meno in pagine web esterne</td>
 </tr>
</table>

>[!CAUTION]
>
>È importante esaminare queste impostazioni con il team IT per determinare a cosa devono essere impostati i criteri aziendali. Le impostazioni errate possono impedire ad alcuni visitatori di accedere alle pagine di destinazione.
