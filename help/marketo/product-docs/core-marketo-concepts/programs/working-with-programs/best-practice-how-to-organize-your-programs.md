---
unique-page-id: 6848705
description: 'Best practice: come organizzare i programmi - Documentazione di Marketo - Documentazione del prodotto'
title: 'Best practice: come organizzare i programmi'
exl-id: 018a3fbd-b741-4005-9695-56958063d71a
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 0%

---

# Best practice: come organizzare i programmi {#best-practice-how-to-organize-your-programs}

Esistono diversi modi per organizzare la struttura nelle attività di marketing e i contenuti di un singolo programma. Tuttavia, alcuni modi sono migliori e aiuteranno le persone nel tuo reparto di marketing.

>[!TIP]
>
>Un giorno, (quando ricevi una promozione!) qualcun altro cercherà di dare un senso ai vostri programmi. Una buona organizzazione li aiuterà a essere produttivi rapidamente.

## Cartelle {#folders}

In Attività di marketing è necessario utilizzare le cartelle per organizzare i programmi. La struttura consigliata è nel seguente esempio:

>[!NOTE]
>
>**Esempio**
>
>* Programmi di marketing attivi
>   * E-mail
>   * Eventi
>      * Eventi live/Roadshow
>      * Fiere
>      * Webinar
>   * Newsletter
>   * Allevamento
>   * Contenuto web
>   * Moduli web
>* Apprendimento
>* Operativo
>   * Ciclo di vita
>   * Punteggio
>   * Gestione dati
>* Insight sulle vendite
>   * Momenti di interesse
>   * E-mail vendite
>   * Campagne con richiesta di vendita
>* **Archivia**
>   * Archivia eventi
>      * Archivio 2012
>      * Archivio 2013

Ognuno di questi elementi menzionati nell’esempio è una cartella. Osserva come tutti hanno un nome univoco. È possibile avere nomi duplicati (più semplici) di cartelle all&#39;interno di programmi, ma non nella directory principale della struttura.

>[!TIP]
>
>La cartella &quot;Archivia&quot; è un tipo speciale di cartella progettata per rimuovere elementi da elenchi selezionati e rapporti. In questo modo il sistema sarà più veloce. Scopri [ulteriori informazioni sulle cartelle](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md).

Puoi certamente aggiungere altre cartelle in base alle tue esigenze. Tieni presente che le generazioni future di esperti di marketing nella tua azienda convivranno con le tue decisioni su come denominare/organizzare le cose.

## Schemi di denominazione {#naming-schemes}

La denominazione è fondamentale, in quanto tutte le funzionalità di Marketo utilizzano un linguaggio comune per comunicare. Per i programmi, è necessario assegnare loro un nome univoco. **Non è possibile assegnare lo stesso nome a due programmi**. Si consiglia di utilizzare il seguente formato:

[Abbreviazione del tipo di programma] [AAAA]-[MM]-[DD opzionale] [Descrizione breve]

>[!NOTE]
>
>**Esempio**
>
>Esempi di nomi dei programmi:
>
>1. ES 2015-09-21 Introduzione al widget
>1. Newsletter NL 2015-06
>1. Webinar WBN 2015-12-01 Argomento qui

I nomi dei programmi devono essere univoci nell’abbonamento, anche in [workspace](/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md).  Per le risorse locali all’interno dei programmi, la regola è **mantieni il nome semplice**. È sufficiente denominare un invito &quot;Invito&quot; invece di &quot;Invito al webinar di giugno 2015&quot;. Poiché questi elementi sono inclusi in un programma, il programma padre fa automaticamente parte del nome quando lo si sceglie altrove. In altre parole, le risorse locali devono essere univoche all’interno del programma. Puoi avere centinaia di risorse denominate &quot;Invita&quot;, ciascuna in un programma diverso e non ti disturberà.

## Token {#tokens}

I token utilizzano cartelle e programmi come veicolo per impostare le variabili da utilizzare per le pagine di destinazione, le e-mail e altre risorse.

L’organizzazione di cui sopra ti consente di inserire token nella cartella Evento in modo che si propaghi in cascata in tutti gli eventi.

>[!NOTE]
>
>**Esempio**
>
>**Indirizzo aziendale**. Utilizza un token invece di scriverlo ogni volta. In questo modo è possibile aggiornarla in un unico punto senza dover creare molte bozze. Quindi esegui l’override del token in base alle esigenze in una cartella di livello inferiore.

## Eventi {#events}

Un evento in genere include molte parti mobili, tra cui inviti, pagine di destinazione, moduli, widget social e campagne intelligenti. La best practice per organizzarli in modo semplice è la fase dell’Evento. Di seguito è riportato un esempio di come la struttura delle cartelle deve cercare un evento.

![](assets/capture.png)

## Programmi di coinvolgimento {#engagement-programs}

Scopri [tutto sui programmi di coinvolgimento](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/understanding-engagement-programs.md). Il modo migliore per organizzare il programma di coinvolgimento è con le cartelle. Crea una cartella per ogni flusso, quindi inserisci le e-mail o i programmi in tale cartella. Includi una cartella di archivio in ogni flusso quando il contenuto diventa obsoleto e desideri rimuoverlo.

## Programmi operativi {#operational-programs}

Vengono utilizzati a scopo di pulizia dei dati. Avere cartelle per le date di esecuzione dei programmi e quindi archiviare le cartelle. Rendendo operativo il programma, si omette di eseguirne il reporting, il che è positivo per questo tipo di attività.

## Nidificazione dei programmi e-mail {#nesting-email-programs}

I programmi e-mail sono progettati per essere lo strumento di gestione della posta elettronica. Puoi inserirli all’interno di Eventi o altri programmi per promozioni, inviti e promemoria. Sono dotati di una dashboard fredda e di altre funzioni di test A/B. Inoltre, possono essere facilmente manipolati nella visualizzazione della pianificazione del programma.

Puoi anche creare un programma e-mail come programma autonomo. I programmi e-mail non sono consentiti all’interno di altri programmi e-mail. Sarebbe da pazzi!

## Duplicazione {#cloning}

Una delle funzionalità più interessanti di Marketo è la possibilità di clonare i programmi. Ciò significa che puoi impostare un &quot;modello&quot; di programma contenente tutte le campagne intelligenti e le e-mail che desideri. Configuralo in anticipo e clonalo per la tua prossima iniziativa di marketing.

>[!TIP]
>
>Osserva i Modelli di evento nell’esempio in alto. Inserisci i diversi tipi di eventi per una clonazione semplice.

Alcuni utenti astraggono persino la maggior parte del testo nelle e-mail e nelle pagine di destinazione in token. Questo consente di clonare e quindi modificare i token. Infine, passare alla visualizzazione della programmazione del programma e modificare le date e si è terminato. Voilà!

## Riepilogo {#summary}

Come potete vedere, Marketo ha una grande potenza. Abbiamo trattato le nozioni di base qui, ma consideriamo alcune [servizi aggiuntivi forniti dagli esperti Marketo](https://www.marketo.com/services/) per perfezionare la sintonizzazione e prepararsi al successo.
