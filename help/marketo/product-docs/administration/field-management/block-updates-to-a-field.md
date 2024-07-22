---
unique-page-id: 2360291
description: Blocca aggiornamenti a un campo - Documentazione di Marketo - Documentazione del prodotto
title: Blocca aggiornamenti a un campo
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Blocca aggiornamenti a un campo {#block-updates-to-a-field}

Il blocco degli aggiornamenti di un campo consente di scrivere nel campo una volta e di mantenere il valore originale per la durata del campo. Questo può essere utile per un campo come [!UICONTROL Source] persona.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Vai all&#39;area **[!UICONTROL Amministratore]**.

   ![](assets/block-updates-to-a-field-1.png)

1. Fare clic su **[!UICONTROL Gestione campi]**.

   ![](assets/block-updates-to-a-field-2.png)

1. Trova il campo, selezionalo, quindi in **[!UICONTROL Azioni campo]** fai clic su **[!UICONTROL Blocca aggiornamenti campo]**.

   ![](assets/block-updates-to-a-field-3.png)

   >[!NOTE]
   >
   >È inoltre possibile bloccare gli aggiornamenti ai [campi personalizzati dei membri del programma](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md).

1. Selezionare le **[!UICONTROL Origini di input]** che si desidera bloccare e fare clic su **[!UICONTROL Applica]**.

   ![](assets/block-updates-to-a-field-4.png)

   >[!CAUTION]
   >
   >Durante l&#39;importazione di un elenco, lo stato di un campo bloccato nell&#39;anteprima di importazione viene visualizzato solo se il campo viene riconosciuto automaticamente da Marketo in base al nome del campo corrispondente a _esattamente_ (o se sono stati stabiliti alias). Se il campo viene scelto manualmente dall’elenco a discesa Campo Marketo, lo stato di blocco non viene visualizzato nell’anteprima di importazione, ma l’operazione di blocco degli aggiornamenti continua a essere implementata.
