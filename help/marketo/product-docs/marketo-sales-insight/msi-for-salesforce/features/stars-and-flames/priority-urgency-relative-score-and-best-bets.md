---
unique-page-id: 2950396
description: Priorità, urgenza, punteggio relativo e elementi di maggiore rilevanza - Documenti Marketo - Documentazione del prodotto
title: Priorità, urgenza, punteggio relativo e elementi di maggiore rilevanza
exl-id: 391aae00-e4f5-4fb1-8728-f5224276dfc2
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 0%

---

# Priorità, urgenza, punteggio relativo e elementi di maggiore rilevanza {#priority-urgency-relative-score-and-best-bets}

Marketo Sales Insight seleziona i contatti e i lead migliori in base alla loro priorità. La priorità di un lead o di un contatto ha due componenti: urgenza e punteggio relativo.

![](assets/priority-urgency-relative-score-and-best-bets-1.png)

Questi sono derivati dal punteggio di lead, una misura dell’interesse della persona per i tuoi prodotti. Maggiore è il punteggio, più è probabile che rispondano positivamente a una chiamata del team di vendita.

>[!NOTE]
>
>Sono necessarie diverse campagne di punteggio per ottenere il valore completo di priorità, urgenza e punteggio relativo.  Con un numero insufficiente di campagne di punteggio o senza campagne di punteggio, questi campi non saranno utili.

## Urgenza {#urgency}

Le fiamme rappresentano l&#39;urgenza — quanto il punteggio di vantaggio di questa persona è cambiato di recente. Un&#39;alta urgenza (più fiamme) significa che il punteggio di questo lead è aumentato molto di recente; è un buon segno che questo lead è interessato alla tua offerta. Dovresti seguire questa persona rapidamente!

Ad esempio, un lead che ha richiesto una demo e ha visitato diverse pagine web avrà probabilmente un’urgenza molto elevata. Un lead che non ha visitato la tua pagina web o aperto le tue e-mail avrà una bassa urgenza. Usa l’urgenza per assegnare la priorità a chi deve essere contattato successivamente.

![](assets/priority-urgency-relative-score-and-best-bets-2.png)

## Punteggio relativo {#relative-score}

Le stelle rappresentano il punteggio relativo: una misura di come il punteggio di testa di questa persona si confronta con quello di chiunque altro. Un punteggio relativo elevato significa che questa persona è probabilmente più interessata e informata sulla tua offerta rispetto alle persone con punteggi relativi più bassi.

Se due lead hanno la stessa urgenza, puoi utilizzare il punteggio relativo per indicare a quale lead si merita prima una telefonata. Quello con il punteggio relativo più alto potrebbe reagire più favorevolmente alla tua offerta rispetto a quella più bassa.

## Elementi di maggiore rilevanza {#best-bets}

Gli elementi di maggiore rilevanza sono i lead e i contatti con il punteggio relativo e di urgenza più elevato. Solo i lead di tua proprietà sono visibili in tale elenco, che viene aggiornato in base al cambiamento dei punteggi dei lead.

>[!NOTE]
>
>Se le tue scelte migliori non corrispondono ai contatti e ai lead migliori che possiedi, chiedi a qualcuno della tua azienda che ha accesso a Marketo di aggiornare i tuoi [Regole punteggio](/help/marketo/getting-started/quick-wins/simple-scoring.md).

### Calcolo dell’urgenza e del punteggio relativo

Per calcolare il numero di stelle e fiamme, i lead e i contatti vengono prima ordinati in base al punteggio o alla variazione del punteggio (rispettivamente per Punteggio relativo e Urgenza). Poi sono divisi in livelli — il livello superiore riceve più stelle o fiamme, quello successivo meno stelle e così via.

Man mano che i punteggi cambiano, i valori di urgenza, priorità e punteggio relativo vengono ricalcolati immediatamente. I livelli di urgenza e punteggio relativo vengono calcolati automaticamente ogni notte sui server Marketo.

>[!NOTE]
>
>I valori Urgenza relativa (fiamme) e Punteggio relativo (stelle) sono numeri interi in Marketo. I valori possibili per ciascuno sono 0-3.
