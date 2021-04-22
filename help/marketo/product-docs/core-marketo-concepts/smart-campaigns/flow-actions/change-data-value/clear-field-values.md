---
unique-page-id: 1147324
description: Valori dei campi chiari - Documenti Marketo - Documentazione del prodotto
title: Cancella valori campo
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---

# Cancella valori campo {#clear-field-values}

[Cambiare il ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) valore dei dati è ottimo, ma come si  __ rimuove completamente il valore? Buona domanda!

1. Nel passaggio di flusso, scegli il campo da cancellare e digita **NULL** (tutti i maiuscoli) come **Nuovo valore**.

   ![](assets/image2015-3-19-10-3a6-3a14.png)

1. Boom! Scommetto che non lo sapevate! Al termine del passaggio del flusso, il valore del campo scelto viene cancellato.

   ![](assets/image2015-3-19-10-3a11-3a9.png)

   >[!CAUTION]
   >
   >Lasciando vuoto il nuovo valore o semplicemente immettendo uno SPACE, il campo non verrà svuotato. Devi digitare NULL. Inoltre, ricorda, i passaggi di flusso non possono essere annullati dopo l’esecuzione.
