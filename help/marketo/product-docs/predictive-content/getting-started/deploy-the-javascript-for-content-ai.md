---
unique-page-id: 11385053
description: Implementare JavaScript per IA per la gestione dei contenuti - Documentazione di Marketo - Documentazione del prodotto
title: Implementare JavaScript per IA per la gestione dei contenuti
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# Implementare JavaScript per IA per la gestione dei contenuti {#deploy-the-javascript-for-content-ai}

Per utilizzare Predictive Content (Contenuto predittivo), devi generare e impostare il tag RTP (Web Personalization).

## Genera tag {#generate-tag}

1. Accedi al tuo account Predictive Content. Vai a **Impostazioni account**.

   ![](assets/settings-dropdown-account-hands.png)

1. In entrata **Configurazione del dominio**, individua il dominio pertinente e fai clic su **Genera tag**.

   ![](assets/generate-tag.png)

1. Copia e incolla il tag di personalizzazione web nel HTML del sito web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copia il tag JavaScript di Personalizzazione web e incollalo come primo script nell’intestazione delle pagine, tra `<head> </head>` tag. Vedi più dettagliato [istruzioni di implementazione qui](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Verifica che il tag venga visualizzato su tutte le pagine, incluse le pagine di destinazione e i sottodomini. Per verificarlo, fai clic con il pulsante destro del mouse sulla pagina del tuo sito web. Vai a **Visualizza origine pagina** in un browser web. Ricerca: &quot;RTP&quot;.

1. Conferma che il tag sia impostato su **ATTIVATO**.
