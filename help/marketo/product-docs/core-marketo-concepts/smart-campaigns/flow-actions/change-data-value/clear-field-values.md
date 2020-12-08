---
unique-page-id: 1147324
description: Cancella valori dei campi - Documenti Marketo - Documentazione prodotto
title: Cancella valori campo
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---


# Cancella valori campo {#clear-field-values}

** [Modifica valore](../../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)dati** è ottimo, ma come si *rimuove* completamente il valore? Buona domanda!

1. Nella fase di flusso, scegliete il campo da cancellare e digitate in **NULL **(tutti i caps) come **Nuovo valore**.

   ![](assets/image2015-3-19-10-3a6-3a14.png)

1. Boom! Scommetto che non lo sapevate! Al termine del passaggio del flusso, il valore del campo scelto viene cancellato.

   ![](assets/image2015-3-19-10-3a11-3a9.png)

   >[!CAUTION]
   >
   >Lasciare vuoto il nuovo valore o semplicemente immettere SPACE non svuoterà il campo. È necessario digitare NULL. Inoltre, ricordate, i passaggi di flusso non possono essere annullati dopo l&#39;esecuzione.

   ![(sorridere)](assets/smile.svg)

A proposito, questa piccola tecnica è all&#39;esame di certificazione Marketo. Non dica loro che abbiamo detto così!