---
unique-page-id: 2951103
description: Note sulla versione - Febbraio 2013 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Febbraio 2013
exl-id: 9adfa676-09ea-497a-bcce-42300848b9d8
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Note sulla versione: febbraio 2013 {#release-notes-february}

La versione di febbraio include una funzionalità altamente richiesta, supporto per Apple Safari e altri piccoli miglioramenti.

## Supporto ufficiale per Apple Safari {#official-support-for-apple-safari}

Le versioni più recenti di Apple Safari per Mac e Windows sono completamente supportate per l’utilizzo con Gestione lead di Marketo. Nota: Safari su iOS non è completamente compatibile.

## Miglioramenti dei webhook {#webhooks-enhancements}

I webhook vengono migliorati per eseguire l’escape dei token nell’URL/payload e possono anche aggiornare i campi dei lead di Marketo analizzando le risposte XML/JSON dai sistemi di terze parti (non disponibile nella Spark SMB Edition).

## Endpoint API SOAP aggiornato {#updated-soap-api-endpoint}

L’endpoint API SOAP preferito è stato aggiornato, come illustrato in Admin -> SOAP API. Aggiorna le chiamate per utilizzare questo nuovo endpoint. Le chiamate API al vecchio endpoint sono obsolete, ma continueranno a funzionare. (API SOAP non disponibile nell’edizione Spark SMB)

## Supporto mobile per le schede Facebook {#mobile-support-for-facebook-tabs}

Le schede facebook pubblicate da Marketo rilevano i dispositivi mobili e li indirizzano a una pagina di destinazione. In questo modo l’utente otterrà il contenuto giusto sui dispositivi mobili su cui non sono supportate le schede Facebook (disponibili in Spark, Standard, Select SMB Editions e Marketo Social Marketing).

## Disponibile a breve: supporto per più modelli {#coming-soon-support-for-multiple-models}

Stiamo gettando le basi per supportare modelli di cicli di fatturato multipli, votati #1&#39;idea per RCA nella Comunità, in una versione futura. In questa versione, noterai alcune modifiche tra cui [Filtri per elenchi avanzati e Aggiungi scelte nei passaggi del flusso](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/find-all-leads-in-a-revenue-cycle-model.md) per supportare la selezione di un modello e di uno stadio. Stiamo inoltre spostando i campi Fase ricavi lead e Modello ciclo ricavi lead dalla scheda Griglia lead elenco avanzato.
