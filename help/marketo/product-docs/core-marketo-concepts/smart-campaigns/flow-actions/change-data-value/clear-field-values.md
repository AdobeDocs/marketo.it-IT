---
unique-page-id: 1147324
description: Cancella valori campo - Documentazione Marketo - Documentazione del prodotto
title: Cancella valori campo
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---

# Cancella valori campo {#clear-field-values}

[Modifica valore dati](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) è grandioso, ma come puoi _rimuovere_ il valore completamente? Buona domanda!

1. Nel passaggio del flusso, scegli il campo da cancellare e digita **NULL** (tutto maiuscole) come **Nuovo valore**.

   ![](assets/image2015-3-19-10-3a6-3a14.png)

1. Boom! Scommetto che non lo sapevi! Al termine del passaggio del flusso, il valore del campo scelto viene cancellato.

   ![](assets/image2015-3-19-10-3a11-3a9.png)

   >[!CAUTION]
   >
   >Se si lascia vuoto il nuovo valore o si immette semplicemente uno SPAZIO, il campo non verrà effettivamente vuoto. È necessario digitare NULL. Inoltre, ricorda che i passaggi di flusso non possono essere annullati dopo l’esecuzione.
