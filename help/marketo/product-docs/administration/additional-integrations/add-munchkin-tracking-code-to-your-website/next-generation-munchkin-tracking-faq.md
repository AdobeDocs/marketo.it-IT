---
unique-page-id: 10096583
description: Domande frequenti sul monitoraggio Munchkin di nuova generazione - Marketo Docs - Documentazione prodotto
title: Domande frequenti sul monitoraggio Munchkin di nuova generazione
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---


# Domande frequenti sul monitoraggio Munchkin di nuova generazione {#next-generation-munchkin-tracking-faq}

Siamo entusiasti di annunciare che presto inizieremo un&#39;implementazione graduale della nostra tecnologia di monitoraggio web di nuova generazione.

>[!NOTE]
>
>**FYI**
>
>Marketo sta standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che nell&#39;abbonamento siano presenti lead/lead e persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

Ecco le cose più importanti da sapere:

* Stiamo rimuovendo il filtro &quot;Is Anonymous&quot; Smart List con la release Q1 (già completata)
* Stiamo aumentando il numero di eventi Web (Visit Web Page, Clic Link on Web Page) che possiamo inserire
* Il codice Munchkin non verrà modificato, quindi non sono necessari aggiornamenti sul sito Web

## Quando sarà il mio abbonamento Marketo su Munchkin V2? {#when-will-my-marketo-subscription-be-on-munchkin-v}

Non abbiamo ancora una data esatta, ma ti preghiamo di controllare qui per gli aggiornamenti.

## Dovrò apportare delle modifiche al mio monitoraggio Munchkin sul mio sito web? {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

No. Il codice di monitoraggio Munchkin rimane lo stesso. Non è necessario apportare modifiche al sito Web.

>[!NOTE]
>
>Questa modifica non influisce sulla personalizzazione Web (Personalizzazione in tempo reale). Continua a identificare visitatori Web anonimi e noti e a personalizzare i contenuti in tempo reale per tali visitatori.

## Perché Marketo ha rimosso il filtro &quot;Is Anonymous&quot; dagli Smart List? {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

Abbiamo cambiato il modo in cui le persone anonime interagiscono con le campagne intelligenti. Prima, hanno lanciato una campagna intelligente, proprio come le persone conosciute. Il filtro &quot;È anonimo&quot; è stato utilizzato per specificare che solo le persone conosciute o anonime scorrono la campagna.

Con Munchkin V2, continueremo a monitorare tutte le attività anonime; tuttavia, non è più possibile applicare filtri a persone anonime. Al momento della conversione (quando la persona viene conosciuta in Marketo), tutte le attività che si verificavano quando la persona era anonima vengono aggiunte al registro delle attività della persona e in questo momento scorrono le campagne per le quali si qualifica.

Se utilizzate già questo filtro in un Smart List (ad esempio, in una Smart Campaign o in un Report), non viene rimosso automaticamente dall&#39;Smart List. Per ulteriori informazioni, consulta di seguito.

>[!NOTE]
>
>**Esempio**
>
>**Trigger**: Visita pagina Web, pagina Web è la pagina prezzi\
>**Flusso**: Modifica punteggio +10 e Momento interessante, **Web**: Pagina dei prezzi visualizzata
>
>Con Munchkin V2, se una persona anonima visita la pagina dei prezzi, non inserisce la campagna immediatamente. Nel momento in cui la persona anonima viene a conoscenza, eseguiremo questa campagna su di lei. Sarà:
>
>* Ottieni un punteggio di 10
   >
   >
* Impostate l&#39;attività Pagina Web sulla data corretta (quando è stata effettivamente visitata)
   >
   >
* Registrati un momento interessante per lei (con la data in cui ha effettivamente visitato la pagina, non quando è diventata nota)
   >
   >
* Registrare un&#39;attività di tipo &quot;Nuova persona&quot;, così come avviene oggi

>



## Cosa succede ai miei Smart List che hanno già il filtro &quot;Is Anonymous&quot;? {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

Dopo il rilascio invernale del &#39;16, se hai vecchie campagne intelligenti con una Smart List che contiene il filtro &quot;Is Anonymous&quot;, accadrà una delle due cose:

1. Se l’Elenco avanzato include il filtro &quot;È anonimo = Falso&quot;, non succederà nulla. Lo ignoreremo e basta.
1. Se l&#39;Elenco avanzato include il filtro &quot;È anonimo = Vero&quot;, la campagna avrà esito negativo e ti verrà inviata una notifica.

## Uso Marketo da un po&#39;. Come faccio a sapere quale delle mie campagne utilizza il filtro &quot;È anonimo&quot;? {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

Prima di apportare questa modifica, abbiamo inviato diverse notifiche settimanali alla casella in entrata delle notifiche con un elenco di Smart List, Smart Campaigns e Reports che utilizzano il filtro &quot;È anonimo&quot;. che possono aiutarvi a identificare la posizione in cui state utilizzando il filtro.

Esaminateli e identificate dove &quot;Is Anonymous&quot; è impostato su True, in quanto queste sono le campagne interessate. Nella maggior parte dei casi, i clienti utilizzano questa impostazione per ottenere un punteggio. Per informazioni sul funzionamento di queste campagne, consulta l’esempio precedente.

## Vorrei una documentazione più dettagliata. Dove posso trovarlo? {#id-like-more-detailed-documentation-where-can-i-find-it}

Consultate i seguenti collegamenti:

[Panoramica sugli aggiornamenti dei lead anonimi](https://nation.marketo.com/docs/DOC-2937)

[Aggiornamenti Dei Lead Anonimi - Modifiche All&#39;Interno Dell&#39;Interfaccia Di Marketo](https://nation.marketo.com/docs/DOC-2938)

[Aggiornamenti Dei Lead Anonimi - Necessità Dell&#39;Azione Del Cliente](https://nation.marketo.com/docs/DOC-2939)

[Aggiornamenti Dei Lead Anonimi - Report Di Analytics](https://nation.marketo.com/docs/DOC-2940)

[Aggiornamenti Dei Lead Anonimi - Pianificazione Delle Release](https://nation.marketo.com/docs/DOC-2961)

[Aggiornamenti Anonimi Del Piombo - Sotto Il Cappuccio](https://nation.marketo.com/docs/DOC-2962)

[Promozione anonima del lead - comportamento Munchkin V2](https://nation.marketo.com/docs/DOC-2963)

## Ho più domande! Come posso farle rispondere? {#i-have-more-questions-how-do-i-get-them-answered}

Per favore, contattate la [comunità](https://nation.marketo.com/welcome). Puoi anche inviare un&#39;e-mail a [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#4c3f393c3c233e380c212d3e27293823622f232162) Loro sarà felice di rispondere alle tue domande.
