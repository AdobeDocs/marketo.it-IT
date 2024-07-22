---
unique-page-id: 4719332
description: Distribuire il JavaScript RTP - Documentazione Marketo - Documentazione del prodotto
title: Distribuire il JavaScript RTP
exl-id: ef96a7f4-3942-4325-bb0f-7647ff2b33b6
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---

# Distribuire il JavaScript RTP {#deploy-the-rtp-javascript}

Per generare e configurare il tag RTP, seguire le istruzioni di installazione riportate di seguito

## Genera tag {#generate-tag}

1. Accedi al tuo account RTP. Vai a **Impostazioni account**.

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. In **Dominio** e **Configurazione dominio**, individuare il dominio pertinente e fare clic su **Genera tag**.

   ![](assets/image2014-12-1-23-3a5-3a35.png)

1. Copiare e incollare il tag Web Personalization (RTP) nel sito Web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copiare il tag JavaScript RTP e incollarlo come primo script nell&#39;intestazione delle pagine, tra i tag `<head> </head>`.

   Assicurati che il tag venga visualizzato su tutte le pagine, incluse le pagine di destinazione e i sottodomini. Per verificarlo, fai clic con il pulsante destro del mouse sulla pagina del tuo sito web. Vai a Visualizza Source pagina in un browser web. Ricerca: &quot;RTP&quot;.

1. Tag impostato su **ON**.

   Verificare che l&#39;opzione Tag sia impostata su ON. Dovresti iniziare a visualizzare il flusso di dati nella scheda dell’organizzazione.

   Ora hai impostato con il tag RTP e sei pronto per iniziare a [creare segmenti](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) e campagne in tempo reale.

1. Verifica che il tag sia su tutte le pagine.
