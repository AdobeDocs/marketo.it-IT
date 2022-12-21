---
unique-page-id: 4719332
description: Distribuzione di JavaScript RTP - Documenti Marketo - Documentazione del prodotto
title: Distribuzione del JavaScript RTP
exl-id: ef96a7f4-3942-4325-bb0f-7647ff2b33b6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---

# Distribuzione del JavaScript RTP {#deploy-the-rtp-javascript}

Per generare e impostare il tag RTP, segui le istruzioni di installazione riportate di seguito

## Genera tag {#generate-tag}

1. Accedi al tuo account RTP. Vai a **Impostazioni account**.

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. In **Dominio** e **Configurazione del dominio**, individua il dominio interessato e fai clic su **Genera tag**.

   ![](assets/image2014-12-1-23-3a5-3a35.png)

1. Copia e incolla il tag di personalizzazione web (RTP, Web Personalization) nel sito web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copia il tag JavaScript RTP e incollalo come primo script nell’intestazione delle pagine, tra `<head> </head>` tag.

   Assicurati che il tag sia visualizzato su tutte le pagine, incluse le pagine di destinazione e i sottodomini. Per controllare, fai clic con il pulsante destro del mouse sulla pagina del sito web. Vai a Visualizza origine pagina in un browser web. Ricerca: &quot;RTP&quot;.

1. Imposta/disattiva tag su **ON**.

   Conferma che l’opzione Tag sia impostata su ON. Dovresti iniziare a visualizzare il flusso di dati nella scheda Organizzazione.

   Ora sei configurato con il tag RTP e pronto per l’avvio [creazione di segmenti](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) e campagne in tempo reale!

1. Verifica che il tag sia presente su tutte le pagine.
