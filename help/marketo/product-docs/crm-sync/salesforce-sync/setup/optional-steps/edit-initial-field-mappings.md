---
unique-page-id: 4719287
description: Modifica mappature campi iniziali - Documentazione Marketo - Documentazione del prodotto
title: Modificare le mappature campi iniziali
exl-id: 320613d1-3845-4e05-a704-0db0f8027dc8
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 3%

---

# Modificare le mappature campi iniziali {#edit-initial-field-mappings}

>[!NOTE]
>
>Questa funzione è accessibile solo prima della sincronizzazione iniziale con Salesforce. Una volta premuto il pulsante **[!UICONTROL Sync Now]**, non è più possibile eseguire questa operazione.

Durante la sincronizzazione iniziale con Salesforce, Marketo Engage combina automaticamente campi personalizzati con nomi simili in un singolo campo sul lato Marketo per garantire che i dati possano essere scambiati sia con oggetti Lead che con oggetti Contact nel CRM. Questo articolo spiega come personalizzare queste mappature.

## Mappa campi non mappati {#map-unmapped-fields}

Quando viene visualizzato un campo nella cartella [!UICONTROL Unmapped Fields], significa che non è mappato a un campo simile sul lead o sul contatto in Salesforce. Puoi ripararlo.

1. Fai clic su **[!UICONTROL Edit Mappings]**.

![](assets/image2014-12-9-13-3a31-3a0.png)

1. Aprire la cartella **[!UICONTROL Unmapped Custom Fields]**.

   ![](assets/two.png)

1. Trascina un campo personalizzato non mappato su un altro per mapparlo.

   >[!NOTE]
   >
   >È possibile modificare solo le mappature di campi personalizzate. Non è possibile modificare le mappature di campi standard.

   ![](assets/three.png)

1. Al termine, fare clic su **[!UICONTROL Finish Mappings]**.

   ![](assets/four.png)

## Interrompi mappatura esistente {#break-existing-mapping}

Se sul lead e sull&#39;oggetto contatto sono presenti campi con lo stesso nome, Marketo li mapperà automaticamente. Puoi considerarli diversi e conservare dati diversi. Interrompi la mappatura in questo modo.

1. Fai clic su **[!UICONTROL Edit Mappings]**.

   ![](assets/image2014-12-9-13-3a31-3a37.png)

1. Evidenziare un campo mappato e fare clic su **[!UICONTROL Break Mapping]** per separare i campi.

   ![](assets/image2014-12-9-13-3a31-3a47.png)

1. Al termine, fai clic su **[!UICONTROL Finish Mappings]**.

   ![](assets/image2014-12-9-13-3a31-3a58.png)

   Bello! La sincronizzazione iniziale è quasi terminata.

## Ripristina schema {#reset-schema}

1. Se si apportano alcune modifiche allo schema in Salesforce mentre si lavora sulle mappature, è possibile richiamare le modifiche facendo clic su **[!UICONTROL Reset Schema]**.

   * Tutte le modifiche di mappatura verranno reimpostate.
   * Se si ripristina lo schema, verranno aggiunti e non rimossi solo i campi (anche se li si nasconde all&#39;utente di sincronizzazione).

   ![](assets/image2014-12-9-13-3a32-3a8.png)
