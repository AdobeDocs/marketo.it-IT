---
description: Scheda Mappa di coinvolgimento - Documentazione di Marketo - Documentazione del prodotto
title: Scheda Mappa di coinvolgimento
hide: true
hidefromtoc: true
exl-id: f54b9258-451b-4607-b5a9-f8627c6f420a
source-git-commit: 3c7eb2fc2e64898e12f08743225c0b802bf97474
workflow-type: tm+mt
source-wordcount: '913'
ht-degree: 0%

---

# Scheda Mappa di coinvolgimento {#engagement-map-tab}

Engagement Map è rappresentato tramite una serie di schede di trigger, filtri e flusso. Facendo clic su ogni scheda vengono visualizzate ulteriori informazioni.

Panoramica trigger: questa scheda mostra il numero di trigger nella campagna. Facendo clic su di esso verrà visualizzata una scheda per ogni trigger, nonché un pannello a tendina con le seguenti informazioni:

* Campagna a cui appartiene il trigger
* Elenco dei nomi dei trigger
* Pulsante &quot;Modifica attivatore&quot;

  ![](assets/engagement-map-tab-1.png)

Dettagli trigger: questa scheda mostra il nome del trigger. Facendo clic su di esso verrà visualizzato un pannello a tendina con le seguenti informazioni:

* Campagna a cui appartiene il trigger
* Elenco dei vincoli associati al trigger
* Pulsante &quot;Modifica attivatore&quot;

  ![](assets/engagement-map-tab-2.png)

Filtro: facendo clic su questa scheda viene visualizzato un pannello a tendina con le seguenti informazioni:

* Campagna a cui appartiene il trigger
* Numero stimato di persone idonee per il filtro
* Elenco dei filtri e dei rispettivi vincoli
* Pulsante &quot;Modifica filtro&quot;

  ![](assets/engagement-map-tab-3.png)

Passaggi di flusso: se un passaggio di flusso include scelte, questa scheda mostra il nome del passaggio di flusso. Facendo clic su di esso verrà visualizzato un pannello a tendina con le seguenti informazioni:

* Campagna a cui appartiene il passaggio Flusso
* Elenco delle condizioni di scelta associate alla fase del flusso
* Pulsante &quot;Modifica flusso&quot;

  ![](assets/engagement-map-tab-4.png)

Passaggi di flusso: in caso contrario _non_ includi eventuali scelte, questa scheda mostrerà gli attributi associati al passaggio di flusso. Facendo clic su di esso verrà visualizzato un pannello a tendina con le seguenti informazioni:

* Campagna a cui appartiene il passaggio Flusso
* Elenco di attributi associati al passaggio del flusso
* Pulsante &quot;Modifica flusso&quot;

  ![](assets/engagement-map-tab-5.png)

## Passaggio di flusso per le campagne Esegui e Richiedi {#flow-step-for-execute-and-request-campaigns}

* Se il passaggio di flusso Esegui o Richiedi campagna non include opzioni, nella scheda viene visualizzato il nome della campagna. Facendo clic sulla scheda viene visualizzato un pannello a tendina con le seguenti informazioni:

   * Campagna a cui appartiene il passaggio di flusso
   * Pulsante &quot;Modifica flusso&quot;
   * Elenco di attributi associati al passaggio del flusso
   * Pulsante &quot;Visualizza elenco&quot;, che apre un elenco di campagne che utilizzano la specifica campagna di richiesta/esecuzione

>[!NOTE]
>
>Puoi modificare i passaggi del flusso da una campagna principale. Per modificare le campagne nidificate, devi passare alla campagna tramite il collegamento presente nel pannello a tendina.

![](assets/engagement-map-tab-6.png)

![](assets/engagement-map-tab-7.png)

* Se il passaggio di flusso Esegui o Richiedi campagna include delle scelte, la scheda mostra il nome della campagna. Facendo clic sulla scheda viene visualizzato un pannello a tendina con le seguenti informazioni:

   * Campagna a cui appartiene il passaggio di flusso
   * Elenco delle condizioni di scelta associate alla fase del flusso
   * Pulsante &quot;Modifica flusso&quot;

  ![](assets/engagement-map-tab-8.png)

  ![](assets/engagement-map-tab-9.png)

* Se una campagna Execute (Esegui) o Request (Richiedi) include delle scelte, facendo clic sulla scheda del flusso si espande per mostrare tutte le scelte nelle singole schede. Facendo clic sulla scheda di scelta si espanderà la campagna associata alla scelta specifica e si visualizzerà un pannello a tendina con le seguenti informazioni:

   * Campagna a cui appartiene la scelta
   * Pulsante &quot;Modifica scelta&quot;
   * Elenco delle condizioni di scelta associate alla fase del flusso
   * Pulsante &quot;Visualizza elenco&quot;, che apre un elenco di campagne che utilizzano la specifica campagna di richiesta/esecuzione

  ![](assets/engagement-map-tab-10.png)

## Visualizzazione di una campagna di esecuzione nidificata {#visualizing-a-nested-execute-campaign}

Esegui le campagne eseguite in serie con la campagna principale. Le persone idonee per una campagna eseguibile completano tutti i passaggi del flusso dalla campagna e tornano alla campagna principale per continuare attraverso i passaggi del flusso di questa campagna.

Di seguito è riportato un esempio di campagna avanzata, &quot;Campaign A&quot;, che include un passaggio di esecuzione del flusso della campagna. Considera &quot;Campagna A&quot; come la tua campagna principale.

![](assets/engagement-map-tab-11.png)

1. Facendo clic sulla scheda del flusso di esecuzione della campagna, si espande per visualizzare i dettagli della &quot;Campagna B&quot;.
1. &quot;Campagna B&quot; include un filtro che divide il pubblico in due gruppi: qualificato e non qualificato.
1. Il pubblico qualificato attraversa i passaggi del flusso associati alla &quot;Campagna B&quot;.
1. Tutti i tipi di pubblico (qualificati e non qualificati) tornano alla &quot;Campagna A&quot; e passano al passaggio di flusso successivo.

   ![](assets/engagement-map-tab-12.png)

Puoi fare clic sul passaggio del flusso Esegui campagna in &quot;Campaign B&quot;, che si espanderà per mostrare le schede di scelta e la campagna associate a ciascuna scelta.

![](assets/engagement-map-tab-13.png)

## Visualizzazione di una campagna di richieste {#visualizing-request-campaign}

Le campagne di richiesta vengono eseguite in parallelo alla campagna principale. Le persone idonee per una campagna di richieste completano tutti i passaggi del flusso dalla campagna e quindi escono dalla campagna. Contemporaneamente, lo stesso gruppo di persone passa attraverso i passaggi del flusso della campagna principale.

Di seguito è riportato un esempio di campagna avanzata, &quot;Campaign A&quot;, che include un passaggio di flusso della campagna di richiesta. Considera &quot;Campagna A&quot; come la tua campagna principale.

![](assets/engagement-map-tab-14.png)

1. Facendo clic sulla scheda del flusso della campagna di richiesta si espanderà per visualizzare i dettagli della &quot;Campagna B&quot;
1. &quot;Campagna B&quot; include un filtro che divide il pubblico in due gruppi: qualificato e non qualificato.
1. Il pubblico qualificato attraversa i passaggi del flusso associati alla &quot;Campagna B&quot;.
1. Allo stesso tempo, tutti i tipi di pubblico passano ai passaggi di flusso successivi nella &quot;Campagna A&quot;.

   ![](assets/engagement-map-tab-15.png)

Puoi approfondire le campagne nidificate se uno dei passaggi del flusso include un’altra campagna di richiesta facendo clic sulla scheda del flusso per visualizzare i dettagli della campagna.

![](assets/engagement-map-tab-16.png)

Di seguito è riportato un esempio di campagna di richiesta con scelte.

![](assets/engagement-map-tab-17.png)

## Gestione degli errori {#error-handling}

Gli errori negli elenchi avanzati e nei passaggi del flusso vengono evidenziati da un’icona di errore nella scheda. Inoltre, un messaggio di errore corrispondente verrà visualizzato nel pannello a tendina.

Di seguito è riportato un esempio di errore in un trigger che viene visualizzato nella scheda panoramica trigger, nel pannello a tendina e nella scheda trigger di dettaglio.

![](assets/engagement-map-tab-18.png)

![](assets/engagement-map-tab-19.png)

**Gli errori nelle schede dei filtri possono includere:**

* Errore nell’elenco avanzato che impedirà la visualizzazione del pubblico qualificato

* Errore nella logica del filtro

* Errore o assenza di vincoli in uno o più filtri

  ![](assets/engagement-map-tab-20.png)

>[!NOTE]
>
>Gli errori all’interno di una campagna nidificata non saranno visibili finché non fai clic su per espandere la campagna nidificata.
