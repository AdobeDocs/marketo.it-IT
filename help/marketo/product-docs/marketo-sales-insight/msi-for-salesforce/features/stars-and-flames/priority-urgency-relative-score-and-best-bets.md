---
unique-page-id: 2950396
description: Priorità, Urgenza, Punteggio relativo e Migliori Scommesse - Marketo Docs - Documentazione prodotto
title: Priorità, Urgenza, Punteggio relativo e migliori risultati
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 0%

---


# Priorità, Urgenza, Punteggio relativo e Best Bets {#priority-urgency-relative-score-and-best-bets}

Visione vendite Marketo sceglie i migliori lead e contatti in base alla loro priorità. La priorità di un lead o di un contatto ha due componenti: urgenza e punteggio relativo.

![](assets/one.png)

Questi sono derivati dal punteggio iniziale, una misura dell&#39;interesse della persona nei vostri prodotti. Più alto è il punteggio, più probabilità risponderanno positivamente a una chiamata dal team di vendita.

>[!NOTE]
>
>Per ottenere il valore completo di priorità, urgenza e punteggio relativo, sono necessarie diverse campagne di valutazione.  Se le campagne di punteggio sono troppo poche o nulle, questi campi non saranno utili.

## Urgenza {#urgency}

Le fiamme rappresentano l&#39;urgenza — quanto il punteggio iniziale di questa persona è cambiato di recente. Un&#39;urgenza elevata (più fiamme) significa che il punteggio di questo lead è aumentato notevolmente ultimamente; è un buon segno che questo lead è interessato alla vostra offerta. Dovrebbe seguire questa persona rapidamente!

Ad esempio, un lead che ha richiesto una demo e ha visitato diverse pagine Web avrà probabilmente un&#39;urgenza molto elevata. Un lead che non ha visitato la pagina Web o aperto le e-mail avrà una bassa urgenza. Utilizzate l&#39;urgenza per assegnare priorità a chi deve essere contattato dopo.

![](assets/two.png)

## Punteggio relativo {#relative-score}

Le stelle rappresentano un punteggio relativo — una misura del modo in cui il punteggio iniziale di questa persona viene confrontato con quello di tutti gli altri. Un punteggio relativo elevato significa che questa persona è probabilmente più interessata e informata sulla vostra offerta rispetto alle persone con punteggi relativi inferiori.

Se due lead hanno la stessa urgenza, puoi usare il punteggio relativo per indicare quale merita una chiamata prima. Quello con il punteggio relativo più alto potrebbe reagire più favorevolmente alla vostra offerta rispetto a quella più bassa.

## Best Bets {#best-bets}

Le migliori Scommesse sono i vostri lead e contatti con la massima urgenza e il punteggio relativo. Nell’elenco sono visibili solo i lead di proprietà e l’elenco viene aggiornato in seguito alla modifica dei punteggi dei lead.

>[!NOTE]
>
>Se le migliori puntate non corrispondono ai migliori lead e contatti che possedete, parlate con qualcuno della vostra azienda che ha accesso a Marketo sull&#39;aggiornamento delle [regole di punteggio](../../../../../getting-started/quick-wins/simple-scoring.md).

### Modalità di calcolo dell&#39;urgenza e del punteggio relativo

Per calcolare il numero di stelle e fiamme, i lead e i contatti vengono ordinati in base al punteggio o alla variazione del punteggio (rispettivamente per Valutazione relativa e Urgenza). Poi sono divisi in livelli — il livello superiore riceve il maggior numero di stelle o fiamme, il successivo riceve meno, e così via.

Con la modifica dei punteggi, i valori di urgenza, priorità e punteggio relativo vengono immediatamente ricalcolati. I livelli di urgenza e valutazione relativa vengono calcolati automaticamente ogni notte sui server Marketo.

>[!NOTE]
>
>Il conteggio Urgenza relativa (fiamme) e Valutazione relativa (stelle) sono numeri interi in Marketo. I valori possibili per ciascun valore sono 0-3.

>[!MORELIKETHIS]
>
>* [Informazioni sulle vendite di Marketo](https://docs.marketo.com/display/docs/marketo+sales+insight)

