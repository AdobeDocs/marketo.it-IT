---
unique-page-id: 2949158
description: Integrare RTP con Google Analytics - Documentazione Marketo - Documentazione del prodotto
title: Integrare RTP con Google Analytics
exl-id: a2bc0c17-dc23-435e-9480-857e97e6fd50
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# Integrare RTP con Google Analytics {#integrate-rtp-with-google-analytics}

>[!NOTE]
>
>Universal Analytics è ora lo standard operativo e tutte le proprietà in Google sono state aggiornate a Universal Analytics.
>
>Questo articolo illustra come utilizzare il vecchio Google Standard Analytics, ma si consiglia di passare a Universal Analytics.
>
>Se non utilizzi già [codice di tracciamento analytics.js](https://developers.google.com/analytics/devguides/collection/analyticsjs/), Google consiglia vivamente di rinominare il sito per utilizzarlo. I seguenti elementi sono diventati obsoleti da Google:
>
>* ga.js
>* urchin.js
>* WAP/snippet lato server
>* YT/MO
>* Variabili personalizzate
>* Variabili definite dall&#39;utente
>
>Scopri come integrare [Personalizzazione web con Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

## Introduzione {#introduction}

Analizza le analisi web da una nuova angolazione utilizzando il flusso diretto di dati da Marketo Real-Time Personalization (RTP) all’account Google Analytics (GA). Misura le visite web in GA in base a organizzazioni, settori e campagne RTP. Visualizza metriche quali i tipi di settori o di segmenti RTP in GA e il modo in cui eseguono e generano lead in base alle diverse origini di traffico (social, pagato, organico), analizzando i tassi di click-through sulle campagne e misurando l’impatto delle campagne di personalizzazione sul tuo sito web. Sfrutta questa possibilità per ottenere il massimo vantaggio dal tuo account RTP

**AUDIENCE ANALYTICS RTP**

Con l’integrazione, hai una nuova dimensione nel tuo account GA. RTP migliora automaticamente le dashboard con:

1. Organizzazioni e industrie
1. Segmenti personalizzati in RTP
1. Elenchi Account-Based Marketing

Concentrati sui tuoi potenziali clienti B2B chiave. Analizza i canali per settori e segmenti mirati.

## Rapporto canale {#channel-report}

![](assets/image2014-11-28-16-3a39-3a28.png)

Il dashboard B2B RTP ti aiuta a comprendere il raggruppamento dei visitatori in base ai segmenti verticali e RTP. Puoi vedere le prestazioni dei visitatori in base al settore finanziario e a diverse campagne di marketing (a pagamento, organiche, sociali). La dashboard fornisce inoltre una panoramica di alto livello delle prestazioni dei segmenti RTP ed esegue l’espansione per mostrare le principali organizzazioni che visitano il sito.

## Flusso comportamentale {#behavioral-flow}

![](assets/image2014-11-28-16-3a40-3a43.png)

Il rapporto di flusso del comportamento (vedi immagine) visualizza il percorso che i visitatori percorrono da una pagina o un evento all’altra. L’esempio dell’immagine mostra il percorso di tutti i visitatori del settore finanziario. Questo rapporto può aiutarti a scoprire quale contenuto mantiene i visitatori coinvolti con il tuo sito.

## Prestazioni RTP {#rtp-performance}

Misura le campagne RTP e le correla alla media complessiva del sito. Scopri in che modo queste campagne influiscono sulle metriche del sito web e utilizza questi dati per concentrare le tue attività di personalizzazione sui target giusti. Genera rapporti personalizzati per comprendere meglio le prestazioni delle campagne di personalizzazione.

![](assets/image2014-11-28-16-3a47-3a0.png)

## Impostazione di RTP con Google Analytics {#setting-up-rtp-with-google-analytics}

1. Aggiungi l’e-mail rtp.ga2@gmail.com come utente Read &amp; Analyze al tuo account GA. Per ulteriori dettagli, consulta [qui](https://support.google.com/analytics/answer/2884495?hl=en).

1. Nel tuo account RTP. Vai a **Impostazioni account**.

   ![](assets/image2014-11-28-16-3a54-3a40.png)

1. Sotto **Impostazioni account**, **Dominio** e **Analytics**.

1. Fai clic su **Google Analytics**.

1. Attiva la relativa **Variabili personalizzate** e **Eventi** per aggiungere questi dati da RTP a Google Analytics.

1. Inserisci il **Fessura** numero per inviare dati di variabili personalizzate (il valore predefinito è 1,2).

![](assets/image2014-11-28-17-3a0-3a17.png)

1. Clic **Salva**.

>[!NOTE]
>
>Per inviare i dati dei segmenti a GA, sotto [Pagina Modifica segmento](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) nella piattaforma RTP, seleziona la casella di controllo **Invia evento alle Google Analytics in corrispondenza del segmento**.

## Impostazione dei rapporti Google Analytics con i dati RTP {#setting-up-google-analytics-reports-with-rtp-data}

Nelle Google Analytics puoi utilizzare le dashboard, la segmentazione GA e il reporting per visualizzare i dati RTP:

* [Dashboard](https://support.google.com/analytics/answer/1068216?hl=en) fornisci una panoramica delle prestazioni del sito web.
* Un segmento GA ha lo scopo di filtrare i visitatori nell’interfaccia GA e visualizzare il traffico per segmento. Scopri come creare un segmento [qui](https://support.google.com/analytics/answer/3124493?hl=en).
* Creazione [rapporti personalizzati](https://support.google.com/analytics/answer/1033013?hl=en) per visualizzare e/o configurare le e-mail pianificate. Consulta in Personalizzazione > Nuovo rapporto personalizzato.
