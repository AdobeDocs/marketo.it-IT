---
unique-page-id: 2360370
description: Come far corrispondere gli stati dei programmi e gli stati delle campagne Salesforce prima della sincronizzazione - Documenti Marketo - Documentazione del prodotto
title: Come far corrispondere gli stati del programma e gli stati delle campagne Salesforce prima della sincronizzazione
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---


# Come far corrispondere gli stati dei programmi e gli stati delle campagne Salesforce prima della sincronizzazione {#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

Questo articolo descrive come risolvere un errore di stato incompatibile e mappare gli stati prima della sincronizzazione del programma Marketo e della campagna Salesforce.

## Cosa fare se hai ricevuto un messaggio di errore {#what-do-you-do-if-you-received-an-error-message}

Se provate a sincronizzare una campagna Salesforce esistente che contiene lead e la campagna contiene uno o più stati incompatibili, viene visualizzato un messaggio di errore. Un programma Marketo e una campagna Salesforce *non verranno sincronizzati* se gli stati non corrispondono esattamente.

![](assets/image2015-7-22-9-3a23-3a29.png)

Da questo messaggio di errore potete scegliere di:

1. Selezionate una campagna diversa a cui eseguire la sincronizzazione dal menu a discesa OPPURE
1. Potete annullare, correggere gli errori di stato e provare a eseguire la sincronizzazione una volta che gli errori sono stati corretti. Per correggere gli errori di stato, effettuate una delle seguenti operazioni:

   * Accedete a Salesforce e rimuovete o rinominate gli Stati membri della campagna incompatibili per mappare gli stati del programma Marketo utilizzati per il tipo di canale associato al programma Marketo.
   * Modifica gli stati del programma in Marketo per mappare gli stati membri della campagna Salesforce che hai installato. Questa è una funzione di amministrazione di Marketo. Per informazioni dettagliate, vedere [Creare un canale del programma](/help/marketo/product-docs/administration/tags/create-a-program-channel.md).
