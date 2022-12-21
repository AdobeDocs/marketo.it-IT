---
unique-page-id: 7514918
description: Informazioni sull’annullamento dell’abbonamento - Documenti Marketo - Documentazione del prodotto
title: Informazioni sull’annullamento della sottoscrizione
exl-id: 30866dc0-cdac-4e73-8dbf-d4b509012269
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 1%

---

# Informazioni sull’annullamento della sottoscrizione {#understanding-unsubscribe}

Ci sono in realtà diversi tipi di annullamenti di abbonamenti integrati in Marketo. Sono tutti rappresentati dai campi dell’oggetto persona, proprio come Nome .

>[!NOTE]
>
>Marketo sta cambiando termini come Blacklist e Whitelist in Inserii nell&#39;elenco Bloccati e Inserire nell&#39;elenco Consentiti nel nostro prodotto. Durante questo aggiornamento, potresti vedere i vecchi termini nella nostra interfaccia utente e le schermate della documentazione, e i nuovi termini nel nostro testo della documentazione. Ci scusiamo per ogni confusione.

Tutti questi campi sono incorporati nell’abbonamento a Marketo. Sono tutti di tipo booleano (casella di controllo). Possono essere utilizzati in Forms o [Modifica valore dati](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) passaggi di flusso.

## Annulla l&#39;iscrizione {#unsubscribed}

Viene utilizzato nella pagina standard per l’annullamento dell’abbonamento. Se una persona controlla questa casella o fa clic sul collegamento per annullare l’abbonamento in un’e-mail, non riceverà più e-mail di marketing. Essi riceveranno tuttavia [e-mail operative](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

## Marketing sospeso {#marketing-suspended}

Questo campo viene impostato dall’utente per l’inserimento di persone in un annullamento temporaneo dell’abbonamento. Le persone possono ottenere questo stato solo se vengono modificate manualmente o se viene utilizzata una fase di modifica del flusso di dati.

## E-mail sospesa {#email-suspended}

Questo stato blocca l&#39;invio di messaggi a una persona per 24 ore dopo l&#39;esecuzione di un messaggio non recapitato. Dopo 24 ore, la persona sarà di nuovo inviabile.

>[!NOTE]
>
>E-mail sospesa rimarrà selezionata anche dopo la fine del periodo di 24 ore, in modo da poter fare riferimento alle persone che sono state segnalate storicamente come tali. Per vedere se la persona è inviabile, è sufficiente calcolare 24 ore dopo il momento della sospensione dell&#39;e-mail.

## Inserire nell&#39;elenco Bloccati {#blocklisted}

[Utilizza questo per persone come concorrenti](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md). Chiunque desideri ricevere **no** e-mail: operative, di marketing, ecc. Non ricevono nulla!

![](assets/image2015-5-18-12-3a6-3a40.png)
