---
unique-page-id: 2360370
description: Come abbinare gli stati del programma e degli stati delle campagne Salesforce prima della sincronizzazione - Documentazione di Marketo - Documentazione del prodotto
title: Come abbinare gli stati del programma e degli stati delle campagne Salesforce prima della sincronizzazione
exl-id: 623676ff-ce63-484f-8467-71127fa40fe0
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# Come abbinare gli stati del programma e degli stati delle campagne Salesforce prima della sincronizzazione {#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

Questo articolo descrive come correggere un errore di stato incompatibile e mappare gli stati prima della sincronizzazione di Marketo Program e Salesforce Campaign.

## Cosa fare se si riceve un messaggio di errore {#what-do-you-do-if-you-received-an-error-message}

Se tenti di eseguire la sincronizzazione con una campagna Salesforce esistente che contiene lead e la campagna contiene uno o più stati incompatibili, viene visualizzato un messaggio di errore. Un programma Marketo e una campagna Salesforce *non* sincronizza se gli stati non corrispondono esattamente.

![](assets/image2015-7-22-9-3a23-3a29.png)

Da questo messaggio di errore, puoi scegliere di:

1. Seleziona un’altra campagna da sincronizzare dal menu a discesa, OPPURE
1. È possibile annullare l&#39;operazione, correggere gli errori di stato e provare a eseguire la sincronizzazione una volta corretti gli errori. Per correggere gli errori di stato, effettuare una delle seguenti operazioni:

   * Accedi a Salesforce, quindi rimuovi o rinomina gli Stati membri della campagna incompatibili da mappare sugli stati del programma Marketo utilizzati per il tipo di canale associato al programma Marketo.
   * Modifica gli stati del programma in Marketo per eseguire il mapping agli stati membri della campagna Salesforce impostati. Questa è una funzione di amministrazione di Marketo. Per ulteriori informazioni, consulta [Creare un canale del programma](/help/marketo/product-docs/administration/tags/create-a-program-channel.md).
