---
unique-page-id: 2949158
description: Integrare RTP con Google Analytics - Marketo Docs - Documentazione prodotto
title: Integrare RTP con Google Analytics
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 0%

---


# Integrare RTP con Google Analytics {#integrate-rtp-with-google-analytics}

>[!NOTE]
>
>Universal Analytics è ora lo standard operativo e tutte le proprietà di Google sono state aggiornate a Universal Analytics.
>
>Questo articolo mostra come utilizzare il vecchio Google Standard Analytics, ma ti consigliamo di passare a Universal Analytics.
>
>Se non utilizzi già il codice di monitoraggio [analytics.js](https://developers.google.com/analytics/devguides/collection/analyticsjs/), Google consiglia vivamente di riassegnare il sito per utilizzarlo. Google ha dichiarato obsoleti i seguenti prodotti:
>
>* ga.js
>* urchin.js
>* Snippet WAP/lato server
>* YT/MO
>* Variabili personalizzate
>* Variabili definite dall&#39;utente

>
>
Scopri come integrare [Web Personalization con Universal Analytics](integrate-rtp-with-google-universal-analytics.md)

## Introduzione {#introduction}

Analizza le tue analisi web da un nuovo punto di vista utilizzando il flusso diretto di dati da Marketing a Real-Time Personalization (RTP) al tuo account Google Analytics (GA). Misura le tue visite web in GA in base a organizzazioni, industrie e campagne RTP. Puoi visualizzare metriche quali i tipi di settori o segmenti RTP in GA e come eseguono e generano lead in base a diverse origini di traffico (social, pagate, organiche), analizzare i tassi di click-through delle campagne e misurare l’impatto delle campagne di personalizzazione sul tuo sito web. Sfruttate questa capacità per ottenere il massimo vantaggio dal vostro account RTP

**Audience Analytics  RTP**

Con l&#39;integrazione, hai una nuova dimensione nel tuo account GA. RTP ottimizza automaticamente le dashboard con:

1. Organizzazioni e industrie
1. Segmenti personalizzati in RTP
1. Elenchi marketing basati su account

Concentrati sulle tue prospettive chiave per il settore B2B. Analizzare i canali per settori e segmenti mirati.

## Rapporto canale {#channel-report}

![](assets/image2014-11-28-16-3a39-3a28.png)

Il dashboard RTP B2B ti aiuta a capire la suddivisione dei visitatori in base alla segmentazione verticale e RTP. Puoi vedere le prestazioni dei visitatori in base al settore finanziario e alle diverse campagne di marketing (a pagamento, organiche, social). Il dashboard fornisce inoltre una panoramica di alto livello delle prestazioni dei segmenti RTP ed effettua delle esercitazioni per mostrare le principali organizzazioni che visitano il sito.

## Flusso comportamentale {#behavioral-flow}

![](assets/image2014-11-28-16-3a40-3a43.png)

Il rapporto sul flusso di comportamento (vedi immagine) visualizza il percorso in cui i visitatori passano da una pagina o un evento all’altra. L&#39;esempio di immagine mostra il percorso di tutti i visitatori provenienti dal settore finanziario. Questo rapporto può aiutarvi a scoprire quali contenuti tengono i visitatori coinvolti nel sito.

## Prestazioni RTP {#rtp-performance}

Misurate le campagne RTP e collegatele alla media complessiva del sito. Scopri in che modo queste campagne influiscono sulle metriche del tuo sito web e utilizzali per concentrare le tue attività di personalizzazione sui target giusti. Generate rapporti personalizzati per comprendere meglio le prestazioni delle campagne di personalizzazione.

![](assets/image2014-11-28-16-3a47-3a0.png)

## Impostazione di RTP con Google Analytics {#setting-up-rtp-with-google-analytics}

1. Aggiungi l&#39;e-mail [`[email protected]`](https://docs.marketo.com/cdn-cgi/l/email-protection#0674727628616734466b67746d6372692865696b) come utente Leggi e analizza nel tuo account GA. Per ulteriori dettagli, vedere [qui](https://support.google.com/analytics/answer/2884495?hl=en).
1. Nel tuo account RTP. Vai a **Impostazioni account**.

   ![](assets/image2014-11-28-16-3a54-3a40.png)

1. In **Impostazioni account**, **Domain** e **Analytics**
1. Fare clic su** Google Analytics.**
1. Attivate le **Variabili personalizzate** e **Eventi** pertinenti per aggiungere questi dati dalla RTP alle Google Analytics.
1. Immettere il numero **Slot** per inviare i dati della variabile personalizzata (il valore predefinito è 1,2).

![](assets/image2014-11-28-17-3a0-3a17.png)

Fare clic su **SAVE**.

>[!NOTE]
>
>Per inviare i dati del segmento a GA, nella sezione [Edit Segment page](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) della piattaforma RTP, selezionare la casella di controllo **Send Event to Google Analytics on Segment Match** (Invia evento a  su Segment Match).

## Impostazione dei rapporti sulle Google Analytics con i dati RTP {#setting-up-google-analytics-reports-with-rtp-data}

Nelle Google Analytics è possibile utilizzare dashboard, segmentazione GA e reporting per visualizzare i dati RTP:

* [I ](https://support.google.com/analytics/answer/1068216?hl=en) dashboard forniscono una panoramica delle prestazioni del sito Web.
* Un segmento GA è destinato a filtrare i visitatori nell’interfaccia GA e visualizzare il traffico per segmento. Vedere come creare un segmento [qui](https://support.google.com/analytics/answer/3124493?hl=en).
* Creazione di [report personalizzati](https://support.google.com/analytics/answer/1033013?hl=en) per visualizzare e/o impostare le e-mail pianificate. Vedere in Personalizzazione > Nuovo rapporto personalizzato.
