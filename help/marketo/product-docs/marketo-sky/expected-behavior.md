---
description: Comportamento previsto - Documentazione di Marketo - Documentazione del prodotto
title: Comportamento previsto
hide: true
hidefromtoc: true
exl-id: d19130cf-186e-4aad-be32-6aad18c9d08b
source-git-commit: fb77478cdcd2b455e9f2359e16aca50143ce492c
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# Comportamento previsto {#expected-behavior}

In questo articolo troverai informazioni sul comportamento previsto associato alle Predictive Audiences (PA).

## Considerazioni su dati e privacy

* Tutte le operazioni di elaborazione dei dati richieste per i modelli AI/ML hanno luogo in Nord America.
* I modelli AI/ML non utilizzano informazioni specifiche sul lead come nome o cognome, genere, e-mail, numeri di contatto, ecc. I modelli utilizzano solo attributi generali derivati da firmographics e dai registri attività.

**Per Predictive Audiences, puoi aspettarti il seguente comportamento**

* PA è accessibile sia in Marketo Sky che nell’esperienza Marketo Classic. Sono disponibili le seguenti caratteristiche specifiche:
   * Filtri predittivi - [!DNL Sky/Classic]
   * Registrazioni previste - [!DNL Sky/Classic]
   * Previsioni di probabilità a livello di lead - [!DNL Sky/Classic]
   * Obiettivi e tracciamento - [!DNL Sky] solo
   * Approfondimenti e raccomandazioni - [!DNL Sky] solo
* Richieste di attivazione iniziale **24-48 ore** per il completamento di tutti i processi dopo l&#39;abilitazione di PA. Vedrai tutte le funzionalità Predictive Audiences e Predictive Filters nell’interfaccia, ma possono essere necessarie fino a 24 ore prima che queste funzioni inizino a funzionare.
* **Le previsioni vengono generate solo per le nuove campagne create dopo l’attivazione della funzione.**

**Ci sono alcune considerazioni aggiuntive specifiche ai filtri predittivi**:

* I filtri di registrazione e probabilità di partecipazione possono essere utilizzati solo con programmi di eventi o webinar. I filtri Lookalike e Unsubscribe possono essere utilizzati nei programmi di e-mail, eventi e webinar.
* Puoi applicare filtri predittivi a una campagna intelligente anche se il programma principale viene creato prima che i filtri predittivi siano abilitati.
* I filtri predittivi non sono disponibili per le campagne trigger.
* Per eseguire una campagna intelligente, i filtri di probabilità devono essere utilizzati insieme ad altri filtri regolari.
* La funzione Regole salvate non è disponibile per l’utilizzo in campagne che contengono filtri predittivi.
* È possibile utilizzare **fino a 5** filtri predittivi in un elenco avanzato.
* I filtri predittivi possono elaborare una **massimo 1 milione di lead qualificati**.
* Puoi avere **fino a 50 programmi attivi** con filtri predittivi. Un programma attivo è qualsiasi programma che utilizza filtri predittivi ed è stato pianificato almeno una volta.

## Quando le registrazioni previste non sono disponibili?

Le registrazioni previste non saranno disponibili nei seguenti casi d’uso:

* se il programma è stato creato prima dell’aggiunta di Predictive Audiences
* quando gli stati del programma non sono mappati agli stati del sistema
* quando non ci sono membri nel programma
* quando non vi sono stati precedenti programmi simili negli ultimi 6 mesi che corrispondono ai criteri richiesti
