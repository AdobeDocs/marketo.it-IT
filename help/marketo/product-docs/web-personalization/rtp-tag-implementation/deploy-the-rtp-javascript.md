---
unique-page-id: 4719332
description: Distribuzione di JavaScript RTP - Documenti Marketo - Documentazione prodotto
title: Implementare il codice JavaScript RTP
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---


# Implementare il codice JavaScript RTP {#deploy-the-rtp-javascript}

Per generare e impostare il tag RTP, seguire le istruzioni di installazione riportate di seguito

## Genera tag {#generate-tag}

1. Accedi al tuo account RTP. Vai a **Impostazioni account**.

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. In **Domain** e **Domain Configuration**, individuare il dominio appropriato e fare clic su **Generate Tag.**

   ![](assets/image2014-12-1-23-3a5-3a35.png)

1. Copiate e incollate il tag Web Personalization (RTP) nel sito Web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copiate il tag JavaScript RTP e incollatelo come primo script nell’intestazione delle pagine, tra i tag `<head> </head>`.

   Accertatevi che il tag sia visualizzato su tutte le pagine, incluse le pagine di destinazione e i sottodomini. Per verificare il problema, fate clic con il pulsante destro del mouse sulla pagina del sito Web. Vai a Visualizza origine pagina in un browser Web. Ricerca: &quot;RTP&quot;.

1. È possibile impostare l&#39;opzione di attivazione/disattivazione tag su **ON**.

   Verificate che l&#39;opzione Tag sia attivata. Dovresti iniziare a visualizzare il flusso di dati nella scheda Organizzazione.

   Ora hai impostato il tag RTP e sei pronto per iniziare [la creazione di segmenti](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) e di campagne in tempo reale!

1. Verifica che il tag si trovi su tutte le pagine.

>[!MORELIKETHIS]
>
>* [Implementazione tag RTP](https://docs.marketo.com/display/docs/rtp+tag+implementation)

