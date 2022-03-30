---
unique-page-id: 10096583
description: Domande frequenti sul monitoraggio Munchkin di nuova generazione - Documenti Marketo - Documentazione del prodotto
title: Domande frequenti sul monitoraggio Munchkin di nuova generazione
exl-id: 283189ac-c817-479a-b896-91233980608c
source-git-commit: 6ad418c8f4056b9a2fb31b0ac995692f0c618795
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 0%

---

# Domande frequenti sul monitoraggio Munchkin di nuova generazione {#next-generation-munchkin-tracking-faq}

Siamo entusiasti di annunciare che presto inizieremo un&#39;implementazione graduale della nostra tecnologia di web tracking di nuova generazione.

Ecco le cose più importanti da sapere:

* Stiamo rimuovendo il filtro &quot;Is Anonymous&quot; Smart List con la versione Q1 (già fatto)
* Stiamo aumentando il numero di eventi web (Visita pagina web, Clic link su pagina web) che possiamo acquisire
* Il tuo codice Munchkin non verrà modificato, quindi non sono necessari aggiornamenti sul tuo sito web

## Quando sarà il mio abbonamento Marketo su Munchkin V2? {#when-will-my-marketo-subscription-be-on-munchkin-v}

Non abbiamo ancora una data esatta, ma controlla qui per gli aggiornamenti.

## Dovrò apportare delle modifiche al mio monitoraggio Munchkin sul mio sito web? {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

No. Il codice di tracciamento Munchkin rimane lo stesso. Non è necessario apportare modifiche al sito web.

>[!NOTE]
>
>Questa modifica non interessa Web Personalization (Real-Time Personalization). Continua a identificare visitatori web anonimi e noti e a personalizzare contenuti in tempo reale per questi visitatori.

## Perché Marketo ha rimosso il filtro &quot;È anonimo&quot; dagli elenchi smart? {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

Abbiamo modificato il modo in cui le persone anonime interagiscono con le campagne intelligenti. Prima scorrevano attraverso una campagna intelligente, proprio come persone conosciute. Il filtro &quot;È anonimo&quot; è stato utilizzato per specificare che la campagna attraversa solo persone conosciute o anonime.

Con Munchkin V2, continueremo a monitorare tutte le attività anonime; tuttavia, non puoi più applicare filtri a persone anonime. Al momento della conversione (quando la persona viene conosciuta in Marketo), tutte le attività che si sono verificate quando la persona era anonima vengono aggiunte al registro delle attività della persona e in questo momento scorrono attraverso le campagne per le quali si qualifica.

Se utilizzi già questo filtro in un elenco avanzato (ad esempio, in una campagna avanzata o in un rapporto), non viene rimosso automaticamente dall’elenco avanzato. Per ulteriori informazioni, consulta la sezione seguente.

>[!NOTE]
>
>**Trigger**: Visita pagina Web, pagina Web è la pagina Prezzi\
>**Flusso**: Cambia punteggio +10 e momento interessante
>**Web**: Pagina dei prezzi visualizzati
>
>Con Munchkin V2, se una persona anonima visita la pagina dei prezzi, non accede alla campagna immediatamente. Al momento in cui la persona anonima si conoscerà, lanceremo questa campagna su di lei. Sarà:
>
>* Ottieni un punteggio di 10
>
>* Imposta l’attività Pagina web sulla data corretta (quando è stata effettivamente visitata)
>
>* Avere un momento interessante registrato per lei (con la data in cui ha effettivamente visitato la pagina, non quando è diventato conosciuto)
>
>* Registrare un’attività &quot;Nuova persona&quot;, come avviene oggi


## Cosa succede ai miei Smart List che dispongono già del filtro &quot;Is Anonymous&quot;? {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

Dopo la versione invernale del 16, se disponi di vecchie campagne intelligenti con una lista intelligente che contiene il filtro &quot;È anonimo&quot;, si verifica una delle due cose seguenti:

1. Se l’Elenco avanzato ha il filtro &quot;Is Anonymous = False&quot;, non succederà nulla. Lo ignoreremo e basta.
1. Se l’Elenco avanzato ha il filtro &quot;Is Anonymous = True&quot;, questa campagna avrà esito negativo e ti verrà inviata una notifica.

## Uso Marketo da un po&#39;. Come faccio a sapere quale delle mie campagne utilizza il filtro &quot;È anonimo&quot;? {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

Prima di apportare questa modifica, abbiamo inviato diverse notifiche settimanali alla tua casella in entrata Notifiche con un elenco di Smart List, Smart Campaigns e Reports che utilizzano il filtro &quot;È anonimo&quot;. Queste possono aiutarti a identificare la posizione in cui stai utilizzando il filtro.

Esaminali e identifica dove hai impostato &quot;Is Anonymous&quot; su True, in quanto queste sono le campagne interessate. Nella maggior parte dei casi, i clienti utilizzano questa impostazione per ottenere un punteggio. Vedi l’esempio precedente per capire come funzioneranno queste campagne.

## Vorrei una documentazione più dettagliata. Dove posso trovarlo? {#id-like-more-detailed-documentation-where-can-i-find-it}

Dai un’occhiata a questi collegamenti:

[Panoramica degli aggiornamenti dei lead anonimi](https://nation.marketo.com/docs/DOC-2937)

[Aggiornamenti dei lead anonimi - Modifiche all’interno dell’interfaccia utente di Marketo](https://nation.marketo.com/docs/DOC-2938)

[Aggiornamenti anonimi dei lead - Necessità di un intervento del cliente](https://nation.marketo.com/docs/DOC-2939)

[Aggiornamenti dei lead anonimi - Rapporti di Analytics](https://nation.marketo.com/docs/DOC-2940)

[Aggiornamenti dei lead anonimi - Pianificazione del rilascio](https://nation.marketo.com/docs/DOC-2961)

[Aggiornamenti Anonimi Di Piombo - Sotto Il Cappuccio](https://nation.marketo.com/docs/DOC-2962)

[Promozione di lead anonimi a lead noti - Munchkin V2 Comportamento](https://nation.marketo.com/docs/DOC-2963)

## Ho altre domande! Come le faccio rispondere? {#i-have-more-questions-how-do-i-get-them-answered}

Si prega di contattare [community](https://nation.marketo.com/). È inoltre possibile contattare [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support). Saranno felici di rispondere alle vostre domande.
