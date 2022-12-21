---
description: Comportamento previsto - Documenti Marketo - Documentazione del prodotto
title: Comportamento previsto
hide: true
hidefromtoc: true
exl-id: d19130cf-186e-4aad-be32-6aad18c9d08b
source-git-commit: d229d152cbdae4f6b2e35700b85052d9c0b748d6
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---

# Comportamento previsto {#expected-behavior}

In questo articolo troverai informazioni sul comportamento previsto associato a Predictive Audiences (PA).

## Considerazioni sui dati e sulla privacy

* Tutti i processi di elaborazione dei dati richiesti per i modelli AI/ML si svolgono in Nord America.
* I modelli AI/ML non utilizzano informazioni specifiche sui lead quali nomi o cognomi, genere, e-mail, numeri di contatto, ecc. I modelli utilizzano solo gli attributi generali derivati dalla grafica dinamica e dai log delle attività.

**Per Predictive Audiences, puoi aspettarti il seguente comportamento**

* L’applicazione a pagina singola è accessibile sia in Marketo Sky che nell’esperienza Marketo Classic. La disponibilità di funzioni specifiche è la seguente:
   * Filtri predittivi - [!DNL Sky/Classic]
   * Registrazioni previste - [!DNL Sky/Classic]
   * Previsioni di probabilità a livello di lead - [!DNL Sky/Classic]
   * Obiettivi e tracciamento - [!DNL Sky] only
   * Informazioni e raccomandazioni - [!DNL Sky] only
* [Attivazione iniziale](/help/marketo/product-docs/marketo-sky/getting-started-with-predictive-audiences.md) prende **24-48 ore** per il completamento di tutti i processi dopo l’abilitazione di PA. Vedrai tutte le funzionalità Predictive Audiences e Predictive Filters nell&#39;interfaccia, ma potrebbero essere necessarie fino a 24 ore per iniziare a funzionare queste funzioni.
* **Le previsioni verranno generate solo per le nuove campagne create dopo l’attivazione della funzione.**

**Esistono alcune considerazioni aggiuntive specifiche per i filtri predittivi**:

* I filtri di probabilità di registrazione e partecipazione possono essere utilizzati solo con programmi evento o webinar. I filtri lookalike e Annulla sottoscrizione possono essere utilizzati nei programmi e-mail, evento e webinar.
* Puoi applicare filtri predittivi a una campagna intelligente anche se il programma principale viene creato prima che i filtri predittivi siano abilitati.
* I filtri predittivi non sono disponibili per le campagne di attivazione.
* Per eseguire una campagna avanzata, è necessario utilizzare i filtri di probabilità insieme ad altri filtri normali.
* La funzione Regole salvate non è disponibile per l’utilizzo in campagne che contengono filtri predittivi.
* È possibile utilizzare **fino a 5** filtri predittivi in un elenco avanzato.
* I filtri predittivi possono elaborare un **massimo 1 milione di lead qualificati**.
* Può **fino a 50 programmi attivi** con filtri predittivi. Un programma attivo è qualsiasi programma che utilizza filtri predittivi ed è stato pianificato almeno una volta.

## Quando non sono disponibili le registrazioni previste?

Le registrazioni previste non saranno disponibili nei seguenti casi d’uso:

* se il programma è stato creato prima dell&#39;aggiunta di Predictive Audiences
* quando gli stati del programma non sono mappati sugli stati del sistema
* quando non vi sono membri nel programma
* quando negli ultimi 6 mesi non esistono programmi simili che soddisfino i criteri richiesti
