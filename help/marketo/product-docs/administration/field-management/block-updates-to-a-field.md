---
unique-page-id: 2360291
description: Blocca gli aggiornamenti a un campo in modo che il primo valore scritto venga mantenuto per tutta la durata del record.
title: Bloccare gli aggiornamenti a un campo
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
feature: Field Management
source-git-commit: e894ece3a643113fd3e1d8df9f8addefea5553f5
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 10%

---

# Bloccare gli aggiornamenti a un campo {#block-updates-to-a-field}

Il blocco degli aggiornamenti di un campo consente di scrivere nel campo una volta e di mantenere il valore originale per la durata del campo. Questo può essere utile per un campo come [!UICONTROL Person Source].

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Passa alla schermata **[!UICONTROL Admin]**.

   ![](assets/block-updates-to-a-field-1.png)

1. Fai clic su **[!UICONTROL Field Management]**.

   ![](assets/block-updates-to-a-field-2.png)

1. Trovare il campo, selezionarlo, quindi in **[!UICONTROL Field Actions]** fare clic su **[!UICONTROL Block Field Updates]**.

   ![](assets/block-updates-to-a-field-3.png)

   >[!NOTE]
   >
   >È inoltre possibile bloccare gli aggiornamenti ai [campi personalizzati dei membri del programma](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md).

1. Selezionare **[!UICONTROL Input Sources]** da bloccare e fare clic su **[!UICONTROL Apply]**.

   ![](assets/block-updates-to-a-field-4.png)

   >[!CAUTION]
   >
   >Durante l&#39;importazione di un elenco, lo stato di un campo bloccato nell&#39;anteprima di importazione viene visualizzato solo se il campo viene riconosciuto automaticamente da Marketo in base al nome del campo corrispondente a _esattamente_ (o se sono stati stabiliti alias). Se il campo viene scelto manualmente dall’elenco a discesa Campo Marketo, lo stato di blocco non viene visualizzato nell’anteprima di importazione, ma l’operazione di blocco degli aggiornamenti continua a essere implementata.
