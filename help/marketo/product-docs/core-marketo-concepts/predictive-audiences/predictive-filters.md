---
description: Filtri predittivi - Documentazione Marketo - Documentazione del prodotto
title: Filtri predittivi
exl-id: 27736b80-cd8b-455d-9d73-c17d492d0906
feature: Predictive Audiences
source-git-commit: 9c9046d6ac889bef4ec8ab7add82fda8e72d73b4
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Filtri predittivi {#predictive-filters}

Come parte di Predictive Audiences, Marketo offre un gruppo di filtri basati su IA/ML in elenchi avanzati all’interno di campagne intelligenti.

![Immagine uno](assets/predictive-filters-1.png)

>[!NOTE]
>
>I filtri &quot;Probabile partecipazione&quot; e &quot;Probabile registrazione&quot; possono essere utilizzati solo nei programmi di eventi. &quot;Probabilità di annullare l’iscrizione&quot;, &quot;Lookalike of Program Members&quot; e &quot;Lookalike of Smart List Members&quot; possono essere utilizzati in tutti i tipi di programmi.

## Probabilità di partecipare {#likelihood-to-attend}

Questo filtro viene utilizzato per limitare efficacemente il pubblico. In questo modo puoi indirizzare e invitare i lead con una maggiore probabilità di **partecipazione** il tuo webinar o evento. Tieni presente che il programma &quot;Probabilità di partecipare&quot; sarà il programma dell’evento corrente.

![Immagine due](assets/predictive-filters-2.png)

## Probabilità di registrazione {#likelihood-to-register}

Simile a _Probabilità di partecipare_ , utilizza questo filtro per limitare il pubblico ed eseguire il targeting dei lead che hanno una maggiore probabilità di **registrazione** per il tuo webinar o evento.

![Immagine tre](assets/predictive-filters-3.png)

## Probabilità di annullare l’abbonamento {#likelihood-to-unsubscribe}

Questo filtra il pubblico in base alla probabilità che annulli l’abbonamento nelle due settimane successive. Puoi utilizzarlo per indirizzare i lead ad alto tasso di affaticamento in modo diverso e più efficace. La soglia per l’annullamento dell’iscrizione è dinamica e guidata da un modello di IA che considera diversi attributi, tra cui il lead time nel database e le attività lead.

![Immagine quattro](assets/predictive-filters-4.png)

>[!NOTE]
>
>I filtri Probabilità di partecipare/registrare/annullare l’abbonamento devono essere utilizzati insieme ad altri filtri standard.

## Lookalike dei membri del programma/Lookalike dei membri dell’elenco avanzato {#lookalike-of-members}

Questi due filtri consentono di espandere il pubblico corrente eseguendo il targeting di lead aggiuntivi simili ai membri di un altro programma o elenco avanzato. I filtri lookalike prendono in considerazione oltre 50 fattori, tra cui attributi di lead, attività e-mail, attività web e coinvolgimento.

Clic **[!UICONTROL Aggiungi vincolo]** per scegliere i criteri di successo per i membri dei programmi selezionati.

Fai clic su **+** per aggiungere facilmente più programmi/elenchi avanzati a un filtro.

![Immagine cinque](assets/predictive-filters-5.png)

## Aspetti da considerare {#things-to-note}

* Puoi applicare filtri predittivi a una campagna avanzata anche se il programma principale viene creato prima che i filtri predittivi siano abilitati.
* I filtri predittivi non sono disponibili per le campagne Trigger.
* La clonazione o lo spostamento di campagne che contengono filtri predittivi non è supportato.
* In un elenco avanzato è possibile utilizzare fino a 5 filtri predittivi.
* Se il Marketo Engage rileva un errore nella valutazione dei filtri predittivi, l’esecuzione della campagna si interrompe automaticamente e riceverai una notifica nel centro notifiche di Marketo.
* I filtri predittivi hanno attualmente un limite di input di 1 milione di persone qualificate.
* È possibile avere fino a 50 programmi attivi con filtri predittivi.
