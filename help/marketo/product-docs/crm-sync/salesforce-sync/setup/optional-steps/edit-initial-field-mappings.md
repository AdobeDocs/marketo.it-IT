---
unique-page-id: 4719287
description: Modifica mappature campi iniziali - Documentazione Marketo - Documentazione del prodotto
title: Modifica mappature campi iniziali
exl-id: 320613d1-3845-4e05-a704-0db0f8027dc8
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# Modifica mappature campi iniziali {#edit-initial-field-mappings}

>[!NOTE]
>
>Questa funzione è accessibile solo prima della sincronizzazione iniziale con Salesforce. Una volta premuto il pulsante **[!UICONTROL Sincronizza ora]**, non sarà più possibile eseguire questa operazione.

Durante la sincronizzazione iniziale con Salesforce, Marketo Engage combina automaticamente campi personalizzati con nomi simili in un singolo campo sul lato Marketo per garantire che i dati possano essere scambiati sia con oggetti Lead che con oggetti Contact nel CRM. Questo articolo spiega come personalizzare queste mappature.

## Mappa campi non mappati {#map-unmapped-fields}

Quando trovi un campo nella cartella [!UICONTROL Campi non mappati], significa che non è mappato a un campo simile sul lead o sul contatto in Salesforce. Puoi ripararlo.

1. Fare clic su **[!UICONTROL Modifica mapping]**.

![](assets/image2014-12-9-13-3a31-3a0.png)

1. Apri la cartella **[!UICONTROL Campi personalizzati non mappati]**.

   ![](assets/two.png)

1. Trascina un campo personalizzato non mappato su un altro per mapparlo.

   >[!NOTE]
   >
   >È possibile modificare solo le mappature di campi personalizzate. Non è possibile modificare le mappature di campi standard.

   ![](assets/three.png)

1. Al termine, fai clic su **[!UICONTROL Fine mappature]**.

   ![](assets/four.png)

## Interrompi mappatura esistente {#break-existing-mapping}

Se sul lead e sull&#39;oggetto contatto sono presenti campi con lo stesso nome, Marketo li mapperà automaticamente. Puoi considerarli diversi e conservare dati diversi. Interrompi la mappatura in questo modo.

1. Fare clic su **[!UICONTROL Modifica mapping]**.

   ![](assets/image2014-12-9-13-3a31-3a37.png)

1. Evidenzia un campo mappato e fai clic su **[!UICONTROL Interrompi mappatura]** per separare i campi.

   ![](assets/image2014-12-9-13-3a31-3a47.png)

1. Al termine, fai clic su **[!UICONTROL Fine mappature]**.

   ![](assets/image2014-12-9-13-3a31-3a58.png)

   Bello! La sincronizzazione iniziale è quasi terminata.

## Ripristina schema {#reset-schema}

1. Se apporti alcune modifiche allo schema in Salesforce mentre lavori sulle mappature, puoi richiamarle facendo clic su **[!UICONTROL Reimposta schema]**.

   * Tutte le modifiche di mappatura verranno reimpostate.
   * Se si ripristina lo schema, verranno aggiunti e non rimossi solo i campi (anche se li si nasconde all&#39;utente di sincronizzazione).

   ![](assets/image2014-12-9-13-3a32-3a8.png)
