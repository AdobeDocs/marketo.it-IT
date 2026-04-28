---
unique-page-id: 10096583
description: Domande frequenti sul rollout di tracciamento di nuova generazione [!DNL Munchkin] e sulla modifica del filtro Is Anonymous.
title: 'Domande frequenti sul tracciamento di nuova generazione [!DNL Munchkin] '
exl-id: 283189ac-c817-479a-b896-91233980608c
feature: Administration, Munchkin Tracking Code
hide: true
hidefromtoc: true
source-git-commit: 40f06a5391f2f7263bea0c5b8cefc1f3a607c68c
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# Domande frequenti sul tracciamento di [!DNL Munchkin] di nuova generazione {#next-generation-munchkin-tracking-faq}

Marketo sta implementando la tecnologia di tracciamento web di nuova generazione in più fasi.

Ecco le cose più importanti da sapere:

* Il filtro Elenco avanzato &quot;È anonimo&quot; è stato rimosso
* Il numero di eventi web (Visita pagina web, Collegamento cliccato su pagina web) che Marketo può acquisire è in aumento
* Il codice [!DNL Munchkin] non verrà modificato, quindi non sono richiesti aggiornamenti sul sito Web

## Quando avverrà la sottoscrizione a Marketo in [!DNL Munchkin] V2? {#when-will-my-marketo-subscription-be-on-munchkin-v}

Non è ancora disponibile una data esatta. Controlla la pagina per aggiornamenti.

## Dovrò apportare delle modifiche al mio tracciamento di [!DNL Munchkin] sul mio sito Web? {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

No. Il codice di tracciamento [!DNL Munchkin] rimane invariato. Non è necessario apportare modifiche al sito Web.

>[!NOTE]
>
>Questa modifica non influisce su Web Personalization (Real-Time Personalization). Continua a identificare visitatori web anonimi e noti e a personalizzare i contenuti in tempo reale per tali visitatori.

## Perché Marketo ha rimosso il filtro &quot;È anonimo&quot; dagli elenchi avanzati? {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

Marketo ha modificato il modo in cui le persone anonime interagiscono con le campagne intelligenti. Prima hanno condotto una campagna intelligente, proprio come le persone conosciute. Il filtro &quot;È anonimo&quot; veniva utilizzato per specificare che solo persone conosciute o solo anonime potevano passare attraverso la campagna.

Con [!DNL Munchkin] V2, Marketo continuerà a tenere traccia di tutte le attività anonime, ma non sarà più possibile applicare filtri alle persone anonime. Nel punto di conversione (quando la persona diventa nota in Marketo), tutte le attività che si sono verificate quando la persona era anonima vengono aggiunte al registro delle attività della persona e in questo momento passano attraverso le campagne per le quali si qualifica.

Se utilizzi già questo filtro in un elenco avanzato (ad esempio, in una campagna avanzata o in un rapporto), non viene rimosso automaticamente dall’elenco avanzato. Per ulteriori dettagli, consulta di seguito.

>[!NOTE]
>
>**Trigger**: pagina Web Visite, pagina Web è pagina determinazione prezzi >**Flusso**: modifica punteggio +10 e momento di interesse >**Web**: pagina determinazione prezzi visualizzata
>
>Con [!DNL Munchkin] V2, se una persona anonima visita la pagina dei prezzi, non entra immediatamente nella campagna. Nel momento in cui la persona anonima diventa nota, Marketo esegue questa campagna su di loro. Essi:
>
>* Ottieni un punteggio di 10
>
>* L’attività Pagina web è impostata sulla data corretta (quando è stata effettivamente visitata)
>
>* Hanno registrato un momento di interesse (con la data in cui hanno effettivamente visitato la pagina, non quando sono diventati noti)
>
>* Registra un’attività &quot;Nuova persona&quot;, come avviene attualmente

## Cosa succede ai miei elenchi avanzati che hanno già il filtro &quot;È anonimo&quot;? {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

Dopo il rilascio della versione invernale del 16, se disponi di vecchie campagne intelligenti con una lista avanzata con il filtro &quot;È anonimo&quot; al suo interno, accadrà una di due cose:

1. Se l’elenco avanzato dispone del filtro &quot;È anonimo = Falso&quot;, non si verifica nulla. Viene ignorato.
1. Se l’elenco avanzato dispone del filtro &quot;Is Anonymous = True&quot; (È anonimo = True), questa campagna avrà esito negativo e verrà inviata una notifica.

## Uso Marketo da un po&#39;. Come faccio a sapere quali delle mie campagne utilizzano il filtro &quot;È anonimo&quot;? {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

Prima di questa modifica, Marketo inviava diverse notifiche settimanali alla casella in entrata delle notifiche con un elenco di elenchi avanzati, campagne avanzate e rapporti che utilizzano il filtro &quot;È anonimo&quot;. Questi possono aiutarti a identificare dove stai attualmente utilizzando questo filtro.

Rivedili e individua dove &quot;È anonimo&quot; è impostato su True, in quanto queste sono le campagne interessate. Nella maggior parte dei casi, questa impostazione viene utilizzata per qualche tipo di punteggio. Per informazioni sul funzionamento di queste campagne, consulta l’esempio precedente.

## Vorrei una documentazione più dettagliata. Dove posso trovarlo? {#id-like-more-detailed-documentation-where-can-i-find-it}

Consulta questi collegamenti:

[Panoramica degli aggiornamenti dei lead anonimi](https://nation.marketo.com/docs/DOC-2937){target="_blank"}

[Aggiornamenti dei lead anonimi - Modifiche nell’interfaccia utente di Marketo](https://nation.marketo.com/docs/DOC-2938){target="_blank"}

[Aggiornamenti dei lead anonimi - Azione del cliente necessaria](https://nation.marketo.com/docs/DOC-2939){target="_blank"}

[Aggiornamenti lead anonimi - Rapporti di Analytics](https://nation.marketo.com/docs/DOC-2940){target="_blank"}

[Aggiornamenti lead anonimi - Pianificazione rilascio](https://nation.marketo.com/docs/DOC-2961){target="_blank"}

[Aggiornamenti lead anonimi - Sotto il cappuccio](https://nation.marketo.com/docs/DOC-2962){target="_blank"}

[Promozione lead anonimo a lead noto - Comportamento  [!DNL Munchkin] V2](https://nation.marketo.com/docs/DOC-2963){target="_blank"}

## Ho altre domande! Come faccio a rispondergli? {#i-have-more-questions-how-do-i-get-them-answered}

Visita la [community Marketo](https://experienceleaguecommunities.adobe.com/){target="_blank"}. È inoltre possibile contattare il Supporto tecnico Marketo. Loro sono felici di rispondere alle vostre domande.
