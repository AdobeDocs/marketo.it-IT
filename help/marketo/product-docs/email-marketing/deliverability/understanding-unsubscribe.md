---
unique-page-id: 7514918
description: Informazioni sull’annullamento dell’iscrizione - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni sull’annullamento dell’iscrizione
exl-id: 30866dc0-cdac-4e73-8dbf-d4b509012269
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 1%

---

# Informazioni sull’annullamento dell’iscrizione {#understanding-unsubscribe}

In realtà esistono diversi tipi di annullamento di abbonamenti incorporati in Marketo. Sono tutti rappresentati da campi sull’oggetto persona, proprio come Nome.

>[!NOTE]
>
>Marketo sta cambiando termini come Blacklist e Whitelist per Inserire nell&#39;elenco Bloccati e Inserire nell&#39;elenco Consentiti il nostro prodotto in modo da. Durante questo aggiornamento, potresti visualizzare i vecchi termini nell’interfaccia utente e nelle schermate della documentazione, nonché i nuovi termini nel testo della documentazione. Ci scusiamo per qualsiasi confusione.

Tutti questi campi sono incorporati nel tuo abbonamento Marketo. Sono tutti di tipo booleano (casella di controllo). Possono essere utilizzati in Forms o [Modifica valore dati](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) passaggi del flusso.

## Annulla l&#39;iscrizione {#unsubscribed}

Viene utilizzato nella pagina standard di annullamento dell’abbonamento. Se una persona seleziona questa casella o fa clic sul collegamento per annullare l’abbonamento in un’e-mail, non riceverà più e-mail di marketing. Tuttavia, riceveranno [e-mail operative](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

## Marketing sospeso {#marketing-suspended}

Questo campo viene impostato dall’utente per il posizionamento delle persone su un annullamento dell’abbonamento temporaneo. Le persone possono raggiungere questo stato solo se vengono modificate manualmente o se viene utilizzato un passaggio di flusso del valore dei dati di modifica.

## E-mail sospesa {#email-suspended}

Questo stato blocca la spedizione di una persona per 24 ore dopo che si è verificato un mancato recapito permanente. Dopo 24 ore, la persona sarà nuovamente disponibile per la posta.

>[!NOTE]
>
>Le e-mail sospese rimarranno controllate anche dopo il periodo di 24 ore, quindi puoi fare riferimento a persone che sono state storicamente contrassegnate come tali. Per vedere se la persona è inviabile, calcola semplicemente 24 ore dopo il momento della sospensione dell’e-mail.

## Inserire nell&#39;elenco Bloccati {#blocklisted}

[Utilizzalo per persone come i concorrenti](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md). Chiunque desideri ricevere **no** e-mail: operative, di marketing, ecc. Non ricevono nulla!

![](assets/image2015-5-18-12-3a6-3a40.png)
