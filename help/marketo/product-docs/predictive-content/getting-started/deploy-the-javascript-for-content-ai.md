---
unique-page-id: 11385053
description: Distribuire JavaScript per IA per la gestione dei contenuti - Documentazione Marketo - Documentazione del prodotto
title: Distribuire JavaScript per IA per la gestione dei contenuti
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# Distribuire JavaScript per IA per la gestione dei contenuti {#deploy-the-javascript-for-content-ai}

Per utilizzare Contenuto predittivo, è necessario generare e impostare il tag RTP (Web Personalization).

## Genera tag {#generate-tag}

1. Accedi al tuo account Predictive Content. Vai a **Impostazioni account**.

   ![](assets/settings-dropdown-account-hands.png)

1. In **Configurazione dominio**, individuare il dominio pertinente e fare clic su **Genera tag**.

   ![](assets/generate-tag.png)

1. Copiare e incollare il tag Personalization Web nelle HTML del sito Web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copiare il tag Web Personalization JavaScript e incollarlo come primo script nell&#39;intestazione delle pagine, tra i tag `<head> </head>`. Consulta [istruzioni di implementazione dettagliate qui](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Verifica che il tag venga visualizzato su tutte le pagine, incluse le pagine di destinazione e i sottodomini. Per verificarlo, fai clic con il pulsante destro del mouse sulla pagina del tuo sito web. Vai a **Visualizza pagina Source** in un browser Web. Ricerca: &quot;RTP&quot;.

1. Verificare che il tag sia impostato su **ON**.
