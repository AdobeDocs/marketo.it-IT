---
unique-page-id: 2949158
description: Integrare RTP con Google Analytics - Documentazione Marketo - Documentazione del prodotto
title: Integrare RTP con le Google Analytics
exl-id: a2bc0c17-dc23-435e-9480-857e97e6fd50
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# Integrare RTP con le Google Analytics {#integrate-rtp-with-google-analytics}

>[!NOTE]
>
>Universal Analytics è ora lo standard operativo e tutte le proprietà in Google sono state aggiornate a Universal Analytics.
>
>Questo articolo mostra come utilizzare il vecchio Google Standard Analytics, ma ti consigliamo di passare ad Universal Analytics.
>
>Se non utilizzi già il [codice di tracciamento di analytics.js](https://developers.google.com/analytics/devguides/collection/analyticsjs/), Google consiglia vivamente di ritoccare il sito per utilizzarlo. Google dichiara obsoleti i seguenti prodotti:
>
>* ga.js
>* urchin.js
>* Frammenti lato server/WAP
>* YT/MO
>* Variabili personalizzate
>* Variabili definite dall&#39;utente
>
>Scopri come integrare [Personalizzazione web con Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

## Introduzione {#introduction}

Analizza le tue analisi web da un nuovo punto di vista utilizzando il flusso di dati diretto da Marketo Real-Time Personalization (RTP) al tuo account Google Analytics (GA). Misura le visite web in GA in base a organizzazioni, settori e campagne RTP. Visualizza metriche quali i tipi di settori o segmenti RTP in GA e come eseguono e generano lead in base a diverse fonti di traffico (social, paid, organic), analizza i tassi di click-through sulle campagne e misura l’impatto delle campagne di personalizzazione sul tuo sito web. Sfrutta questa capacità per trarre il massimo vantaggio dal tuo account RTP

**Audience Analytics RTP**

Con l’integrazione, hai una nuova dimensione nel tuo account GA. RTP migliora automaticamente le dashboard con:

1. Organizzazioni e industrie
1. Segmenti personalizzati in RTP
1. Elenchi Account-Based Marketing

Concentrati sui tuoi potenziali clienti B2B chiave. Analizzare i canali per settori e segmenti mirati.

## Rapporto canale {#channel-report}

![](assets/image2014-11-28-16-3a39-3a28.png)

Il dashboard RTP B2B ti aiuta a comprendere la suddivisione dei visitatori in base alla segmentazione verticale e RTP. Puoi vedere le prestazioni dei visitatori in base al settore finanziario e a diverse campagne di marketing (a pagamento, organiche, social). Il dashboard fornisce anche una panoramica di alto livello delle prestazioni dei segmenti RTP ed effettua delle esercitazioni per mostrare le principali organizzazioni che visitano il tuo sito.

## Flusso comportamentale {#behavioral-flow}

![](assets/image2014-11-28-16-3a40-3a43.png)

Il rapporto sul flusso di comportamento (vedi immagine) visualizza il percorso in cui i visitatori viaggiano da una pagina o un evento all’altra. L’esempio di immagine mostra il percorso di tutti i visitatori provenienti dal settore finanziario. Questo rapporto può aiutarti a scoprire quali contenuti mantengono i visitatori coinvolti nel tuo sito.

## Prestazioni RTP {#rtp-performance}

Misura le campagne RTP e le correla alla media complessiva del sito. Scopri in che modo queste campagne influiscono sulle metriche del tuo sito web e utilizzali per concentrare le tue attività di personalizzazione sui target giusti. Genera report personalizzati per comprendere meglio le prestazioni delle campagne di personalizzazione.

![](assets/image2014-11-28-16-3a47-3a0.png)

## Configurazione di RTP con Google Analytics {#setting-up-rtp-with-google-analytics}

1. Aggiungi l’e-mail rtp.ga2@gmail.com come utente di lettura e analisi al tuo account GA. Per ulteriori dettagli, consulta [qui](https://support.google.com/analytics/answer/2884495?hl=en).

1. Nel tuo account RTP. Vai a **Impostazioni account**.

   ![](assets/image2014-11-28-16-3a54-3a40.png)

1. Sotto **Impostazioni account**, **Dominio** e **Analytics**.

1. Fai clic su **Google Analytics**.

1. Accendere il pertinente **Variabili personalizzate** e **Eventi** per aggiungere questi dati da RTP a Google Analytics.

1. Inserisci il **Slot** numero da inviare dati di variabili personalizzate (il valore predefinito è 1,2).

![](assets/image2014-11-28-17-3a0-3a17.png)

1. Fai clic su **Salva**.

>[!NOTE]
>
>Per inviare i dati del segmento a GA, sotto la [Pagina Modifica segmento](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) nella piattaforma RTP, seleziona la casella di controllo **Invia evento a Google Analytics sulla corrispondenza del segmento**.

## Configurazione dei rapporti sulle Google Analytics con i dati RTP {#setting-up-google-analytics-reports-with-rtp-data}

In Google Analytics puoi utilizzare dashboard, segmentazione GA e reporting per visualizzare i dati RTP:

* [Dashboard](https://support.google.com/analytics/answer/1068216?hl=en) fornisce una panoramica delle prestazioni del sito web.
* Un segmento GA è destinato a filtrare i visitatori nell’interfaccia GA e a visualizzare il traffico per segmento. Scopri come creare un segmento [qui](https://support.google.com/analytics/answer/3124493?hl=en).
* Creazione [report personalizzati](https://support.google.com/analytics/answer/1033013?hl=en) per visualizzare e/o impostare le e-mail pianificate. Vedere in Personalizzazione > Nuovo rapporto personalizzato.
