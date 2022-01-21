---
unique-page-id: 2950396
description: Priorità, Urgenza, Punteggio relativo e Migliori offerte - Documenti Marketo - Documentazione del prodotto
title: Priorità, Urgenza, Punteggio relativo e Migliori offerte
exl-id: 391aae00-e4f5-4fb1-8728-f5224276dfc2
source-git-commit: 15263f9c23c958499aaa2e4e6491b4962c617358
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 0%

---

# Priorità, Urgenza, Punteggio relativo e Migliori offerte {#priority-urgency-relative-score-and-best-bets}

Marketo Sales Insight sceglie i migliori lead e contatti in base alla loro priorità. La priorità di un lead o di un contatto ha due componenti: urgenza e punteggio relativo.

![](assets/priority-urgency-relative-score-and-best-bets-1.png)

Questi sono derivati dal punteggio iniziale, una misura dell&#39;interesse della persona nei prodotti. Più alto è il punteggio, più è probabile che rispondano positivamente a una chiamata dal team di vendita.

>[!NOTE]
>
>Sono necessarie diverse campagne di punteggio per ottenere il valore completo di priorità, urgenza e punteggio relativo.  Se le campagne di valutazione sono insufficienti o non disponibili, questi campi non saranno utili.

## Urgenza {#urgency}

Le fiamme rappresentano l&#39;urgenza — quanto è cambiato il punteggio iniziale di questa persona di recente. Un&#39;elevata urgenza (più fiamme) significa che il punteggio di questo lead è aumentato notevolmente ultimamente; è un buon segno che questo lead è interessato alla tua offerta. Dovrebbe seguire questa persona rapidamente!

Ad esempio, un lead che ha richiesto una demo e ha visitato diverse pagine web avrà probabilmente un’urgenza molto elevata. Un lead che non ha visitato la tua pagina web o aperto le tue e-mail avrà una bassa urgenza. Usa l’urgenza per assegnare la priorità a chi deve essere contattato dopo.

![](assets/priority-urgency-relative-score-and-best-bets-2.png)

## Punteggio relativo {#relative-score}

Le stelle rappresentano il punteggio relativo — una misura del punteggio iniziale di questa persona rispetto a quello di tutti gli altri. Un punteggio relativo elevato significa che questa persona è probabilmente più interessata e informata sulla tua offerta rispetto a persone con punteggi relativi inferiori.

Se due lead hanno la stessa urgenza, è possibile utilizzare il punteggio relativo per indicare quale si merita una prima chiamata. Quella con il punteggio relativo più alto potrebbe reagire più favorevolmente alla tua offerta rispetto a quella più bassa.

## Migliori offerte {#best-bets}

Le migliori scommesse sono i vostri lead e contatti con la massima urgenza e il punteggio relativo. Solo i lead che possiedi sono visibili in tale elenco e l’elenco viene aggiornato in seguito alla modifica dei punteggi dei lead.

>[!NOTE]
>
>Se le tue migliori scommesse non corrispondono ai migliori lead e contatti che possiedi, parla con qualcuno della tua azienda che ha accesso a Marketo sull&#39;aggiornamento della tua [Regole di valutazione](/help/marketo/getting-started/quick-wins/simple-scoring.md).

### Calcolo dell’urgenza e del punteggio relativo

Per calcolare il numero di stelle e fiamme, i lead e i contatti vengono prima ordinati per punteggio o variazione di punteggio (rispettivamente per Punteggio relativo e Urgenza). Poi sono divisi in livelli — il livello superiore riceve il maggior numero di stelle o fiamme, quello successivo ne riceve meno, e così via.

Quando i punteggi cambiano, i valori di urgenza, priorità e punteggio relativo vengono immediatamente ricalcolati. I livelli di urgenza e punteggio relativo vengono calcolati automaticamente ogni notte sui server Marketo.

>[!NOTE]
>
>Il conteggio di Urgenza relativa (fiamme) e Punteggio relativo (stelle) sono numeri interi in Marketo. I valori possibili per ciascuno sono 0-3.
