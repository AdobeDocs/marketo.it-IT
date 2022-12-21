---
unique-page-id: 6848705
description: Procedure consigliate - Come organizzare i programmi - Documentazione Marketo - Documentazione del prodotto
title: 'Procedure consigliate: come organizzare i programmi'
exl-id: 018a3fbd-b741-4005-9695-56958063d71a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 0%

---

# Best practice: Organizzare i programmi {#best-practice-how-to-organize-your-programs}

Sono disponibili diversi modi per organizzare l’albero nelle attività di marketing e i contenuti di un singolo programma. Tuttavia, alcuni modi sono migliori e aiuteranno le persone nel tuo reparto marketing.

>[!TIP]
>
>Un giorno, (quando vieni promosso!) qualcun altro cercherà di dare un senso ai tuoi programmi. Una buona organizzazione li aiuterà ad essere produttivi rapidamente.

## Cartelle {#folders}

In Attività di marketing, devi utilizzare le cartelle per organizzare i programmi. La struttura consigliata si trova nell’esempio seguente:

>[!NOTE]
>
>**Esempio**
>
>* Programmi di marketing attivi
   >   * E-mail
   >   * Eventi
      >      * Eventi live / Roadshow
      >      * Fiere commerciali
      >      * Webinar
   >   * Newsletter
   >   * Infermiera
   >   * Contenuto web
   >   * Moduli web
>* Apprendimento
>* Operativo
   >   * Ciclo di vita
   >   * Punteggio
   >   * Gestione dati
>* Approfondimenti vendite
   >   * Momenti interessanti
   >   * E-mail di vendita
   >   * Campagne richieste di vendita
>* **Archivia**
   >   * Archiviare gli eventi
      >      * Archivio 2012
      >      * Archivio 2013


Ognuno di questi menzionati nell’esempio è una cartella. Notate come si chiamano tutti in modo univoco. È possibile disporre di nomi duplicati (più semplici) delle cartelle all&#39;interno dei programmi INSIDE, ma non nella radice della struttura.

>[!TIP]
>
>La cartella &quot;Archivia&quot; è un tipo speciale di cartella progettata per rimuovere elementi dagli elenchi selezionati e dal reporting. Questo aiuterà il tuo sistema a funzionare più rapidamente. Scopri [ulteriori informazioni sulle cartelle](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md).

È certamente possibile aggiungere più cartelle come si ritiene opportuno. Tieni presente che le future generazioni di esperti di marketing della tua azienda vivranno con le tue decisioni su come assegnare un nome o organizzare le cose.

## Denominazione degli schemi {#naming-schemes}

La denominazione è fondamentale, in quanto le funzionalità di Marketo utilizzano tutte un linguaggio comune per comunicare. Per i programmi, devi denominarli qualcosa di unico. **Due programmi non possono avere lo stesso nome**. Si consiglia di utilizzare il formato seguente:

[Abbreviazione del tipo di programma] [YYYY]-[MM]-[DD opzionale] [Descrizione breve]

>[!NOTE]
>
>**Esempio**
>
>Esempio di nomi di programma:
>
>1. ES 2015-09-21 Introduzione ai Widget
>1. Newsletter NL 2015-06
>1. Argomento del webinar WBN 2015-12-01 qui


I nomi dei programmi devono essere univoci nell&#39;abbonamento, anche in diversi [aree di lavoro](/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md).  Per le risorse locali all’interno dei programmi, la regola è di **mantieni il nome semplice**. Basta nominare un invito &quot;Invito&quot;, invece di &quot;2015 June Webinar Invitation&quot;. Poiché si trovano in un programma, il programma principale viene automaticamente incluso nel nome quando lo si sceglie altrove. In altre parole, le risorse locali devono essere univoche all’interno del programma. Puoi avere centinaia di risorse denominate &quot;Invite&quot;, ciascuna in un programma diverso e non ti farà preoccupare.

## Token {#tokens}

I token utilizzano cartelle e programmi come veicolo per impostare le variabili da utilizzare per pagine di destinazione, e-mail e altre risorse.

L’organizzazione di cui sopra consente di inserire token nella cartella Evento in modo che vengano suddivisi in cascata in tutti gli eventi.

>[!NOTE]
>
>**Esempio**
>
>**Indirizzo dell&#39;azienda**. Utilizza un token invece di scriverlo ogni volta. In questo modo è possibile aggiornarlo in un unico punto senza dover creare molte bozze. Quindi, sostituisci il token come necessario in una cartella di livello inferiore.

## Eventi {#events}

Un evento ha solitamente molte parti mobili, tra cui: inviti, pagine di destinazione, moduli, widget social e campagne avanzate. La migliore pratica per organizzarli per facilità d&#39;uso è quella della fase dell&#39;Evento. Esempio di ricerca di un evento nella struttura delle cartelle.

![](assets/capture.png)

## Programmi di coinvolgimento {#engagement-programs}

Scopri [tutti i programmi di coinvolgimento](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/understanding-engagement-programs.md). Il modo migliore per organizzare il programma di coinvolgimento è con le cartelle. Crea una cartella per ogni flusso e poi inserisci le e-mail o i programmi in quella cartella. Includi una cartella di archivio in ogni flusso quando il contenuto non è aggiornato e vuoi rimuoverlo.

## Programmi operativi {#operational-programs}

Vengono utilizzati a scopo di pulizia dei dati. Disporre di cartelle per le date di esecuzione dei programmi e quindi archiviare le cartelle. Rendendo il programma operativo, lo si sta omettendo dal reporting, che è buono per questo tipo di attività.

## Nidificazione dei programmi e-mail {#nesting-email-programs}

I programmi e-mail sono progettati per essere il tuo strumento per la blasting della posta. Puoi inserirli in Eventi o altri programmi per promozioni, inviti e promemoria. Sono dotati di un dashboard cool e di altre funzionalità di test A/B. Inoltre, sono facilmente manipolabili nella visualizzazione della pianificazione del programma.

Puoi anche creare un programma e-mail come programma autonomo. I programmi e-mail non sono consentiti all’interno di altri programmi e-mail. Sarebbe folle!

## Clonazione {#cloning}

Una delle caratteristiche più interessanti di Marketo è la capacità di clonare programmi. Questo significa che puoi impostare un programma &quot;template&quot; che ha tutte le campagne intelligenti e le e-mail che desideri. Configuralo in anticipo e quindi clonalo per la tua prossima iniziativa di marketing.

>[!TIP]
>
>Osserva i Modelli evento nell’esempio nella parte superiore. Inserisci i tuoi diversi tipi di eventi per una facile clonazione.

Alcuni utenti possono anche astrarre la maggior parte del testo nelle e-mail e nelle pagine di destinazione nei token. Questo consente di clonare e quindi modificare i token. Infine, vai alla visualizzazione programmazione programma e regola le date e hai finito. Voila!

## Riepilogo {#summary}

Come potete vedere, c&#39;è molta energia in Marketo. Abbiamo trattato le basi qui, ma consideriamo alcune [servizi aggiuntivi da Marketo Experts](https://www.marketo.com/services/) per perfezionare e impostarsi per il successo.
