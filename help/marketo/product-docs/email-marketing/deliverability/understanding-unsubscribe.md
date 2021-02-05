---
unique-page-id: 7514918
description: Informazioni sull'annullamento della sottoscrizione - Documenti Marketo - Documentazione prodotto
title: Informazioni su Annulla sottoscrizione
translation-type: tm+mt
source-git-commit: 615ddd6ffdb3873baa159d440db7b24f3a07e6b0
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# Informazioni sull&#39;annullamento della sottoscrizione {#understanding-unsubscribe}

In realtà ci sono diversi tipi di unsubscribes integrati in Marketo. Sono tutti rappresentati da campi sull&#39;oggetto persona, proprio come Nome.

>[!NOTE]
>
>Marketo sta cambiando termini come Blacklist e Whitelist per  Inserii nell&#39;elenco Bloccati e  Inserire nell&#39;elenco Consentiti nel nostro prodotto. Nel corso di questo aggiornamento, i vecchi termini possono essere visualizzati nella nostra interfaccia utente e nelle schermate della documentazione, nonché i nuovi termini nel nostro testo della documentazione. Ci scusiamo per ogni confusione.

Tutti questi campi sono incorporati nell’iscrizione a Marketo. Sono tutti di tipo booleano (casella di controllo). Possono essere utilizzati nei passaggi di flusso di Forms o [Change Data Value](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md).

## Annulla sottoscrizione {#unsubscribed}

Viene utilizzato nella pagina standard di annullamento dell’iscrizione. Se una persona seleziona questa casella o fa clic sul collegamento per annullare la sottoscrizione in un messaggio e-mail, non riceverà più e-mail di marketing. Tuttavia, riceveranno [e-mail operative](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

## Marketing sospeso {#marketing-suspended}

Questo campo è impostato dall’utente per l’inserimento di utenti in un’iscrizione temporanea. Le persone possono ottenere questo stato solo se vengono modificate manualmente o se viene utilizzato un passaggio di modifica del valore dei dati.

## E-mail sospesa {#email-suspended}

Questo stato blocca la spedizione di una persona per 24 ore dopo l&#39;esecuzione di un duro rimbalzo. Dopo 24 ore, la persona sarà di nuovo inviabile.

>[!NOTE]
>
>E-mail sospesa rimarrà selezionata anche dopo la fine del periodo di 24 ore, in modo da poter fare riferimento a persone che sono state storicamente contrassegnate come tali. Per vedere se la persona è inviabile, basta calcolare 24 ore dopo il momento della sospensione dell&#39;e-mail.

##  Inserire nell&#39;elenco Bloccati {#blocklisted}

[Usate questo per persone come i concorrenti](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md). Chiunque desideri ricevere **no** e-mail: operative, di marketing, ecc. Non ottengono niente!

![](assets/image2015-5-18-12-3a6-3a40.png)
