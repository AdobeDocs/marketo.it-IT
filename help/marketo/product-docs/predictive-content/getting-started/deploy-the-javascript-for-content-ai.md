---
unique-page-id: 11385053
description: Distribuzione di JavaScript per Content-AI - Marketo Docs - Documentazione prodotto
title: Distribuzione di JavaScript per Content-AI
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---


# Distribuzione di JavaScript per Content-AI {#deploy-the-javascript-for-content-ai}

>[!NOTE]
>
>A seconda della data di acquisto, l’iscrizione a Marketo può includere contenuti predittivi di marketing o contenuti`<sup>AI</sup>`. Per gli utenti che utilizzano contenuti predittivi, Marketo attiva le funzioni di analisi dei contenuti`<sup>AI</sup>` fino al 30 aprile 2018. Per mantenere queste funzionalità oltre tale data, contatta il tuo Customer Success Manager di Marketo per effettuare l&#39;aggiornamento al contenuto`<sup>AI</sup>`di Marketo.

Per utilizzare il contenuto predittivo, è necessario generare e impostare la RTP (Web Personalization) `tag.`

## Genera tag {#generate-tag}

1. Accedete al vostro account Predictive Content. Vai a Impostazioni **** account.

   ![](assets/settings-dropdown-account-hands.png)

1. In Configurazione **** dominio, individua il dominio appropriato e fai clic su **Genera tag.**

   ![](assets/generate-tag.png)

1. Copiate e incollate il tag Personalizzazione Web nell’HTML del sito Web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copiate il tag JavaScript di Web Personalization e incollatelo come primo script nell’intestazione delle pagine, tra i `<head> </head>` tag . Consulta le istruzioni [di implementazione più dettagliate qui](http://docs.marketo.com/display/docs/rtp+tag+implementation) [.](http://pages2.marketo.com/rtp-implementation.html)

1. Verifica che il tag sia visualizzato su tutte le pagine, incluse le pagine di destinazione e i sottodomini. Per controllare questa funzione, fai clic con il pulsante destro del mouse sulla `website’s` pagina. Vai a **Visualizza origine** pagina in un browser Web. Ricerca: &quot;RTP&quot;.
1. Verificate che l&#39;opzione Tag sia impostata su **ON**.

