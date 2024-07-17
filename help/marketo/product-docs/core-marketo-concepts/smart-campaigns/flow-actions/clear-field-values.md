---
unique-page-id: 1147324
description: Cancella valori campo - Documentazione Marketo - Documentazione del prodotto
title: Cancella valori campo
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '95'
ht-degree: 0%

---

# Cancella valori campo {#clear-field-values}

[Cambia valore dati](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) è ottimo, ma come _rimuovi_ completamente il valore? Buona domanda!

1. Nel passaggio del flusso, scegli il campo da cancellare e digita in **NULL** (tutte maiuscole) come **Nuovo valore**.

   ![](assets/clear-field-values-1.png)

1. Al termine del passaggio del flusso, il valore del campo scelto viene cancellato.

   ![](assets/clear-field-values-2.png)

   >[!CAUTION]
   >
   >Se si lascia vuoto il nuovo valore o si immette semplicemente uno SPAZIO, il campo non verrà effettivamente vuoto. È necessario digitare NULL. Inoltre, ricorda che i passaggi di flusso non possono essere annullati dopo l’esecuzione.
