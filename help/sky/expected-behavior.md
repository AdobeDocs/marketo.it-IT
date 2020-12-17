---
title: comportamento previsto
description: Comportamento previsto
translation-type: tm+mt
source-git-commit: 642fd57105afff1031f18883c5809206f136b7c6
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---


# Comportamento previsto

<br> 

In questo articolo troverete informazioni sul comportamento previsto associato a Predictive Audiences (PA).

## Considerazioni sui dati e sulla privacy

* L&#39;elaborazione dei dati necessaria per i modelli AI/ML avviene in Nord America.
* I modelli AI/ML non utilizzano informazioni lead specifiche, quali nomi o cognomi, sesso, e-mail, numeri di contatto, ecc. I modelli utilizzano solo gli attributi generali derivati dalla grafica e dai registri attività.

## Per Predictive Audiences, puoi aspettarti il seguente comportamento:

* PA è accessibile sia in Marketo Sky che in Marketo Classic. La disponibilità di funzioni specifiche è la seguente:
   * Filtri predittivi - [!DNL Sky/Classic]
   * Registrazioni previste - [!DNL Sky/Classic]
   * Previsioni di probabilità a livello di lead - [!DNL Sky/Classic]
   * Obiettivi e monitoraggio - solo [!DNL Sky]
   * Approfondimenti e raccomandazioni - solo [!DNL Sky]
* [L&#39;](/help/sky/getting-started-with-predictive-audiences.md) attivazione iniziale richiede **24-48** ore per completare tutti i processi dopo l&#39;abilitazione dell&#39;PA. Nell&#39;interfaccia verranno visualizzate tutte le funzionalità Predictive Audiences (Pubblico predittivo) e Predictive Filters (Filtri predittivi), ma potrebbero essere necessarie fino a 24 ore prima che queste funzioni inizino a funzionare.
* **Le previsioni verranno generate solo per le nuove campagne create dopo l&#39;attivazione della funzione.**

## Esistono alcune considerazioni aggiuntive specifiche per i filtri predittivi:

* I filtri di registrazione e probabilità di partecipazione possono essere utilizzati solo con i programmi evento o webinar. I filtri per similarità e Annulla sottoscrizione possono essere utilizzati nei programmi e-mail, eventi e webinar.
* Potete applicare filtri predittivi a una campagna intelligente anche se il programma principale viene creato prima che siano abilitati i filtri predittivi.
* I filtri predittivi non sono disponibili per le campagne di attivazione.
* Per eseguire una campagna intelligente, è necessario utilizzare i filtri di probabilità insieme ad altri filtri regolari.
* La funzione Regole salvate non è disponibile per le campagne che contengono filtri predittivi.
* In un elenco avanzato è possibile utilizzare un massimo di 5 **filtri predittivi.**
* I filtri predittivi possono elaborare un **massimo di 1 milione di lead qualificati**.
* È possibile avere **fino a 50 programmi attivi** con filtri predittivi. Un programma attivo è qualsiasi programma che utilizza filtri predittivi ed è stato pianificato almeno una volta.

## Quando non sono disponibili le registrazioni previste?

Le registrazioni previste non saranno disponibili nei seguenti casi di utilizzo:

* se il programma è stato creato prima dell&#39;aggiunta di Pubblico predittivo
* quando gli stati del programma non sono mappati sugli stati del sistema
* in assenza di membri nel programma
* in assenza di programmi analoghi precedenti negli ultimi 6 mesi che soddisfano i criteri richiesti
