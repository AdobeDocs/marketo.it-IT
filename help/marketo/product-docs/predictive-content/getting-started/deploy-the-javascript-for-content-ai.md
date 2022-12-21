---
unique-page-id: 11385053
description: Distribuzione di JavaScript per Content-AI - Documenti Marketo - Documentazione del prodotto
title: Distribuzione di JavaScript per Content-AI
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# Distribuzione di JavaScript per Content-AI {#deploy-the-javascript-for-content-ai}

Per utilizzare il contenuto predittivo, devi generare e impostare il tag RTP (Web Personalization).

## Genera tag {#generate-tag}

1. Accedi al tuo account Predictive Content . Vai a **Impostazioni account**.

   ![](assets/settings-dropdown-account-hands.png)

1. In **Configurazione del dominio**, individua il dominio interessato e fai clic su **Genera tag**.

   ![](assets/generate-tag.png)

1. Copia e incolla il tag di personalizzazione web nel HTML del sito web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copia il tag JavaScript di personalizzazione web e incollalo come primo script nell’intestazione delle pagine, tra `<head> </head>` tag. Vedi più dettagliata [istruzioni di implementazione qui](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Verifica che il tag sia visualizzato in tutte le pagine, incluse le pagine di destinazione e i sottodomini. Per controllare, fai clic con il pulsante destro del mouse sulla pagina del sito web. Vai a **Visualizza origine pagina** in un browser web. Ricerca: &quot;RTP&quot;.

1. Conferma che l’opzione Tag sia impostata su **ON**.
