---
unique-page-id: 11385053
description: Distribuzione di JavaScript per Content-AI - Marketo Docs - Documentazione prodotto
title: Distribuzione di JavaScript per Content-AI
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---


# Distribuzione di JavaScript per Content-AI {#deploy-the-javascript-for-content-ai}

>[!NOTE]
>
>A seconda della data di acquisto, l&#39;iscrizione a Marketo può includere contenuti predittivi di marketing o contenuti`<sup>AI</sup>`. Per gli utenti che utilizzano Predictive Content, Marketo attiva le funzioni di Content`<sup>AI</sup>` Analytics fino al 30 aprile 2018. Per mantenere queste funzionalità oltre tale data, contatta il tuo Customer Success Manager di Marketo per effettuare l&#39;aggiornamento a Contenuto di Marketo`<sup>AI</sup>`.

Per utilizzare il contenuto predittivo, è necessario generare e impostare la RTP (Web Personalization) `tag.`

## Genera tag {#generate-tag}

1. Accedete al vostro account Predictive Content. Vai a **Impostazioni account**.

   ![](assets/settings-dropdown-account-hands.png)

1. In **Configurazione dominio**, individuare il dominio appropriato e fare clic su **Genera tag.**

   ![](assets/generate-tag.png)

1. Copiate e incollate il tag Personalizzazione Web nell’HTML del sito Web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copiate il tag JavaScript di Web Personalization e incollatelo come primo script nell&#39;intestazione delle pagine, tra i tag `<head> </head>`. Vedere le istruzioni di implementazione più dettagliate [qui](https://docs.marketo.com/display/docs/rtp+tag+implementation) [.](https://pages2.marketo.com/rtp-implementation.html)

1. Verifica che il tag sia visualizzato su tutte le pagine, incluse le pagine di destinazione e i sottodomini. Per verificare il problema, fai clic con il pulsante destro del mouse sulla pagina `website’s`. Vai a **Visualizza origine pagina** in un browser Web. Ricerca: &quot;RTP&quot;.
1. Verificare che l&#39;opzione Tag sia impostata su **ON**.

