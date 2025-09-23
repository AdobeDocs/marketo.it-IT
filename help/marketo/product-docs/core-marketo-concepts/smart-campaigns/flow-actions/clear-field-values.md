---
unique-page-id: 1147324
description: Cancella valori campo - Documentazione Marketo - Documentazione del prodotto
title: Cancellare valori campo
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '92'
ht-degree: 6%

---

# Cancellare valori campo {#clear-field-values}

[Cambia valore dati](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) è ottimo, ma come _rimuovi_ completamente il valore? Buona domanda!

1. Nel passaggio del flusso, scegli il campo da cancellare e digita **[!UICONTROL NULL]** (tutte maiuscole) come **[!UICONTROL New Value]**.

   ![](assets/clear-field-values-1.png)

1. Al termine del passaggio del flusso, il valore del campo scelto viene cancellato.

   ![](assets/clear-field-values-2.png)

   >[!CAUTION]
   >
   >Se si lascia vuoto il nuovo valore o si immette semplicemente uno SPAZIO, il campo non verrà effettivamente vuoto. È necessario digitare NULL. Inoltre, ricorda che i passaggi di flusso non possono essere annullati dopo l’esecuzione.
