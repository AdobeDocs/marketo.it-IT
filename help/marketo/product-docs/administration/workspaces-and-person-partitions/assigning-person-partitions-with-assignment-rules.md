---
unique-page-id: 2360327
description: Assegnazione di partizioni persona con regole di assegnazione - Documenti Marketo - Documentazione del prodotto
title: Assegnare partizioni persone con regole di assegnazione
exl-id: 6b54dcb7-8da9-466b-b153-099ebcb96424
feature: Partitions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 11%

---

# Assegnare partizioni persone con regole di assegnazione {#assigning-person-partitions-with-assignment-rules}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!PREREQUISITES]
>
>[Creare una partizione di persona](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md)

Quando si utilizzano le partizioni persona, impostare le regole di assegnazione per indirizzare le persone create dal CRM alle rispettive partizioni.

>[!NOTE]
>
>Solo le persone create in Marketo dal CRM e tramite l’API SOAP avranno regole di assegnazione applicate.

1. Passa alla schermata **[!UICONTROL Admin]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-1.png)

1. Fai clic su **[!UICONTROL Workspaces & Partitions]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-2.png)

1. Nella scheda **[!UICONTROL Person Partitions]**, fare clic su **[!UICONTROL Assignment Rules]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-3.png)

1. Fare clic su **[!UICONTROL Add Choice]** per aggiungere le condizioni per il routing delle persone nelle partizioni personali.

   ![](assets/assigning-person-partitions-with-assignment-rules-4.png)

1. Seleziona il campo su cui deve essere basata la condizione.

   ![](assets/assigning-person-partitions-with-assignment-rules-5.png)

1. Scegliere l&#39;operatore di scelta e immettere un valore.

   ![](assets/assigning-person-partitions-with-assignment-rules-6.png)

1. Selezionare la partizione persone in cui si desidera inserire le persone che soddisfano le condizioni.

   ![](assets/assigning-person-partitions-with-assignment-rules-7.png)

   >[!NOTE]
   >
   >Puoi aggiungere tutte le scelte che ti piacciono.

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-8.png)

Ed eccola qui! Hai assegnato regole per riempire le partizioni delle persone con le persone.

>[!NOTE]
>
>Se non viene soddisfatta nessuna delle condizioni precedenti, verrà applicata la scelta predefinita.
