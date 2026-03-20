---
unique-page-id: 11385053
description: Scopri come generare e inserire il tag Personalization web RTP per i contenuti predittivi. Copialo nell’intestazione della pagina, verifica la copertura e conferma che l’interruttore sia sempre attivo.
title: Distribuire JavaScript per i contenuti basati sull’IA
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
source-git-commit: cd7a000c415bedd561aa509e375ba0dee8e81d9f
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 8%

---

# Distribuire JavaScript per i contenuti basati sull’IA {#deploy-the-javascript-for-content-ai}

Per utilizzare Contenuto predittivo, è necessario generare e impostare il tag RTP (Web Personalization).

## Genera tag {#generate-tag}

1. Accedi al tuo account Predictive Content. Passa a **[!UICONTROL Account Settings]**.

   ![](assets/settings-dropdown-account-hands.png)

1. In **[!UICONTROL Domain Configuration]**, individuare il dominio pertinente e fare clic su **[!UICONTROL Generate Tag]**.

   ![](assets/generate-tag.png)

1. Copiare e incollare il tag Personalization Web nel HTML del sito Web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copiare il tag Web Personalization JavaScript e incollarlo come primo script nell&#39;intestazione delle pagine, tra i tag `<head> </head>`. Consulta [istruzioni di implementazione dettagliate qui](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Verifica che il tag venga visualizzato su tutte le pagine, incluse le pagine di destinazione e i sottodomini. Per verificarlo, fai clic con il pulsante destro del mouse sulla pagina del tuo sito web. Vai a **[!UICONTROL View Page Source]** in un browser Web. Ricerca: &quot;RTP&quot;.

1. Verificare che il tag sia impostato su **[!UICONTROL ON]**.
