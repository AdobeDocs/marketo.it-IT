---
unique-page-id: 2360370
description: Come far corrispondere gli stati del programma e gli stati della campagna Salesforce prima della sincronizzazione - Documenti Marketo - Documentazione del prodotto
title: Come far corrispondere gli stati del programma e gli stati della campagna Salesforce prima della sincronizzazione
exl-id: 623676ff-ce63-484f-8467-71127fa40fe0
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# Come far corrispondere gli stati del programma e gli stati della campagna Salesforce prima della sincronizzazione {#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

Questo articolo descrive come correggere un errore di stato incompatibile e mappare gli stati prima della sincronizzazione del programma Marketo e della campagna Salesforce.

## Cosa fare se si riceve un messaggio di errore {#what-do-you-do-if-you-received-an-error-message}

Se tenti di eseguire la sincronizzazione con una campagna Salesforce esistente che contiene lead e la campagna contiene uno o più stati incompatibili, viene visualizzato un messaggio di errore. Un programma Marketo e una campagna Salesforce *non* sincronizza se gli stati non sono una corrispondenza esatta.

![](assets/image2015-7-22-9-3a23-3a29.png)

Da questo messaggio di errore puoi scegliere di:

1. Seleziona una campagna diversa a cui eseguire la sincronizzazione dal menu a discesa, OPPURE
1. È possibile annullare, correggere gli errori di stato e cercare di eseguire la sincronizzazione una volta che gli errori sono stati riparati. Per correggere gli errori di stato, eseguire una delle operazioni seguenti:

   * Accedi a Salesforce e rimuovi o rinomina gli Stati membri della campagna incompatibili per eseguire la mappatura sugli stati del programma Marketo utilizzati per il tipo di canale associato al tuo programma Marketo.
   * Modifica gli stati del programma in Marketo per eseguire il mapping agli stati membri della campagna Salesforce che hai installato. Questa è una funzione di amministrazione di Marketo. Per maggiori dettagli, vedi [Creare un canale del programma](/help/marketo/product-docs/administration/tags/create-a-program-channel.md).
