---
unique-page-id: 4719287
description: Modifica mappature campi iniziali - Documentazione Marketo - Documentazione del prodotto
title: Modifica mappature campi iniziali
exl-id: 320613d1-3845-4e05-a704-0db0f8027dc8
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# Modifica mappature campi iniziali {#edit-initial-field-mappings}

>[!NOTE]
>
>Questa funzione è accessibile solo prima della sincronizzazione iniziale con Salesforce. Una volta **Sincronizza** non è più possibile.

Durante la sincronizzazione iniziale con Salesforce, Marketo combina automaticamente campi personalizzati con nomi simili in un unico campo sul lato Marketo per garantire che i dati possano essere scambiati sia con oggetti Lead che con oggetti Contact nel CRM. Questo articolo spiega come personalizzare queste mappature.

## Mappa campi non mappati {#map-unmapped-fields}

Quando visualizzi un campo nella cartella Campi non mappati, significa che non è mappato a un campo simile sul lead o sul contatto in Salesforce. Puoi ripararlo.

1. Clic **Modifica mappature**.

![](assets/image2014-12-9-13-3a31-3a0.png)

1. Apri **Campi personalizzati non mappati** cartella.

   ![](assets/two.png)

1. Trascina un campo personalizzato non mappato su un altro per mapparlo.

   >[!NOTE]
   >
   >È possibile modificare solo le mappature di campi personalizzate. Non è possibile modificare le mappature di campi standard.

   ![](assets/three.png)

1. Clic **Mappature finali** quando hai finito.

   ![](assets/four.png)

## Interrompi mappatura esistente {#break-existing-mapping}

Se sul lead e sull&#39;oggetto contatto sono presenti campi con lo stesso nome, Marketo li mapperà automaticamente. Puoi considerarli diversi e conservare dati diversi. Interrompi la mappatura in questo modo.

1. Clic **Modifica mappature**.

   ![](assets/image2014-12-9-13-3a31-3a37.png)

1. Evidenzia un campo mappato e fai clic su **Interrompi mappatura** per separare i campi.

   ![](assets/image2014-12-9-13-3a31-3a47.png)

1. Clic **Mappature finali** quando hai finito.

   ![](assets/image2014-12-9-13-3a31-3a58.png)

   Bello! La sincronizzazione iniziale è quasi terminata.

## Ripristina schema {#reset-schema}

1. Se apporti alcune modifiche allo schema in Salesforce mentre lavori sulle mappature, puoi richiamarle facendo clic su **Ripristina schema**.

   * Tutte le modifiche di mappatura verranno reimpostate.
   * Se si ripristina lo schema, verranno aggiunti e non rimossi solo i campi (anche se li si nasconde all&#39;utente di sincronizzazione).

   ![](assets/image2014-12-9-13-3a32-3a8.png)
