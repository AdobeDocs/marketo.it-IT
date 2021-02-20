---
unique-page-id: 11385053
description: Distribuzione di JavaScript per Content-AI - Marketo Docs - Documentazione prodotto
title: Distribuzione di JavaScript per Content-AI
translation-type: tm+mt
source-git-commit: 06e0f5489e6375a97e2fe77834bf45fa41f23ea6
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---


# Distribuzione di JavaScript per Content-AI {#deploy-the-javascript-for-content-ai}

Per utilizzare Predictive Content, è necessario generare e impostare il tag RTP (Web Personalization).

## Genera tag {#generate-tag}

1. Accedete al vostro account Predictive Content. Vai a **Impostazioni account**.

   ![](assets/settings-dropdown-account-hands.png)

1. In **Configurazione dominio**, individuare il dominio appropriato e fare clic su **Genera tag**.

   ![](assets/generate-tag.png)

1. Copiate e incollate il tag Personalizzazione Web nell’HTML del sito Web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copiate il tag JavaScript di Web Personalization e incollatelo come primo script nell&#39;intestazione delle pagine, tra i tag `<head> </head>`. Consulta le istruzioni [di implementazione più dettagliate qui](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Verifica che il tag sia visualizzato su tutte le pagine, incluse le pagine di destinazione e i sottodomini. Per verificare il problema, fate clic con il pulsante destro del mouse sulla pagina del sito Web. Vai a **Visualizza origine pagina** in un browser Web. Ricerca: &quot;RTP&quot;.

1. Verificare che l&#39;opzione Tag sia impostata su **ON**.
