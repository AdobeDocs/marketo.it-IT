---
unique-page-id: 10096583
description: "Prossima generazione [!DNL Munchkin] Domande frequenti sul tracciamento - Documentazione di Marketo - Documentazione del prodotto"
title: "Prossima generazione [!DNL Munchkin] Domande frequenti sul tracciamento"
exl-id: 283189ac-c817-479a-b896-91233980608c
source-git-commit: 1a6f029b8c9665ecd7fcc066004d88ee6c915505
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 0%

---

# Prossima generazione [!DNL Munchkin] Domande frequenti sul tracciamento {#next-generation-munchkin-tracking-faq}

Siamo entusiasti di annunciare che presto inizieremo un rollout graduale della nostra tecnologia di tracciamento web di nuova generazione.

Ecco le cose più importanti da sapere:

* Con la versione Q1 stiamo rimuovendo il filtro per elenchi avanzati &quot;È anonimo&quot; (già eseguito)
* Stiamo aumentando il numero di eventi web (Visita pagina web, Collegamento selezionato su pagina web) che è possibile acquisire
* Il tuo [!DNL Munchkin] il codice non verrà modificato, pertanto non sono necessari aggiornamenti sul sito web

## Quando sarà attiva la mia iscrizione a Marketo [!DNL Munchkin] V2? {#when-will-my-marketo-subscription-be-on-munchkin-v}

Non abbiamo ancora una data esatta, ma tornate qui per aggiornamenti.

## Dovrò apportare modifiche al mio [!DNL Munchkin] tracciamento sul sito web? {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

No. Il [!DNL Munchkin] il codice di tracciamento rimane invariato. Non è necessario apportare modifiche al sito Web.

>[!NOTE]
>
>Questa modifica non influisce sulla personalizzazione web (personalizzazione in tempo reale). Continua a identificare visitatori web anonimi e noti e a personalizzare i contenuti in tempo reale per tali visitatori.

## Perché Marketo ha rimosso il filtro &quot;È anonimo&quot; dagli elenchi avanzati? {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

Abbiamo modificato il modo in cui le persone anonime interagiscono con le campagne intelligenti. Prima hanno condotto una campagna intelligente, proprio come le persone conosciute. Il filtro &quot;È anonimo&quot; veniva utilizzato per specificare che solo persone conosciute o solo anonime potevano passare attraverso la campagna.

Con [!DNL Munchkin] V2, continueremo a monitorare tutte le attività anonime; tuttavia, non è più possibile applicare filtri alle persone anonime. Nel punto di conversione (quando la persona diventa nota in Marketo), tutte le attività che si sono verificate quando la persona era anonima vengono aggiunte al registro delle attività della persona e in questo momento passano attraverso le campagne per le quali si qualifica.

Se utilizzi già questo filtro in un elenco avanzato (ad esempio, in una campagna avanzata o in un rapporto), non viene rimosso automaticamente dall’elenco avanzato. Per ulteriori dettagli, consulta di seguito.

>[!NOTE]
>
>**Trigger**: pagina Web Visite, pagina Web è pagina determinazione prezzi\
>**Flusso**: modifica punteggio +10 e momento di interesse
>**Web**: pagina Determinazione prezzi visualizzata
>
>Con [!DNL Munchkin] V2: se una persona anonima visita la pagina dei prezzi, non entra immediatamente nella campagna. Nel momento in cui la persona anonima si farà conoscere, faremo una campagna su di lei. Lei:
>
>* Ottieni un punteggio di 10
>
>* L’attività Pagina web deve essere impostata sulla data corretta (quando è stata effettivamente visitata)
>
>* Avere un Momento di Interesse registrato per lei (con la data in cui ha effettivamente visitato la pagina, non quando è diventata nota)
>
>* Registra un’attività &quot;Nuova persona&quot;, come avviene attualmente


## Cosa succede ai miei elenchi avanzati che hanno già il filtro &quot;È anonimo&quot;? {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

Dopo il rilascio della versione invernale del 16, se disponi di campagne Smart precedenti con una Smart List contenente il filtro &quot;È anonimo&quot;, accadrà una di due cose:

1. Se l’elenco avanzato dispone del filtro &quot;È anonimo = Falso&quot;, non si verifica nulla. Lo ignoreremo e basta.
1. Se l’elenco avanzato dispone del filtro &quot;È anonimo = True&quot;, questa campagna avrà esito negativo e ti verrà inviata una notifica.

## Uso Marketo da un po&#39;. Come faccio a sapere quali delle mie campagne utilizzano il filtro &quot;È anonimo&quot;? {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

Prima di apportare questa modifica, abbiamo inviato diverse notifiche settimanali alla tua casella in entrata Notifiche con un elenco di elenchi avanzati, campagne avanzate e rapporti che utilizzano il filtro &quot;È anonimo&quot;. Questi possono aiutarti a identificare dove stai attualmente utilizzando questo filtro.

Rivedi le campagne e identifica dove &quot;È anonimo&quot; è impostato su True, in quanto sono interessate. Nella maggior parte dei casi, i clienti utilizzano questa impostazione per assegnare un punteggio. Per informazioni sul funzionamento di queste campagne, consulta l’esempio precedente.

## Vorrei una documentazione più dettagliata. Dove posso trovarlo? {#id-like-more-detailed-documentation-where-can-i-find-it}

Consulta questi collegamenti:

[Panoramica degli aggiornamenti dei lead anonimi](https://nation.marketo.com/docs/DOC-2937){target="_blank"}

[Aggiornamenti dei lead anonimi - Modifiche nell’interfaccia utente di Marketo](https://nation.marketo.com/docs/DOC-2938){target="_blank"}

[Aggiornamenti dei lead anonimi - Azione del cliente necessaria](https://nation.marketo.com/docs/DOC-2939){target="_blank"}

[Aggiornamenti lead anonimi - Rapporti di Analytics](https://nation.marketo.com/docs/DOC-2940){target="_blank"}

[Aggiornamenti lead anonimi - Pianificazione rilascio](https://nation.marketo.com/docs/DOC-2961){target="_blank"}

[Aggiornamenti lead anonimi - Sotto il cappuccio](https://nation.marketo.com/docs/DOC-2962){target="_blank"}

[Promozione lead anonimo per lead noto - [!DNL Munchkin] Comportamento V2](https://nation.marketo.com/docs/DOC-2963){target="_blank"}

## Ho altre domande! Come faccio a rispondergli? {#i-have-more-questions-how-do-i-get-them-answered}

Contatta il numero [community](https://nation.marketo.com/){target="_blank"}. You can also contact [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}. Saranno felici di rispondere alle vostre domande.
