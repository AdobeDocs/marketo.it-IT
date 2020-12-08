---
unique-page-id: 4719287
description: Modifica mappature campi iniziali - Documenti Marketo - Documentazione prodotto
title: Modifica mappature campi iniziali
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# Modifica mappature campi iniziali {#edit-initial-field-mappings}

>[!NOTE]
>
>**Promemoria**
>
>Questa funzione è accessibile solo prima della sincronizzazione iniziale con Salesforce! Se si preme il pulsante **Sinc. ora** , non sarà più possibile eseguire questa operazione.

Durante la sincronizzazione iniziale con Salesforce, Marketo combina automaticamente i campi personalizzati con nomi simili in un unico campo sul lato Marketo per garantire che i dati possano essere scambiati con gli oggetti Lead e Contact del CRM. In questo articolo viene illustrato come personalizzare tali mappature.

## Mappa campi non mappati {#map-unmapped-fields}

Quando viene visualizzato un campo nella cartella Campi non mappati, significa che non è mappato a un campo simile sul lead o sul contatto in Salesforce. Potete ripararlo.

1. Fate clic su Modifica mappature.

![](assets/image2014-12-9-13-3a31-3a0.png)

1. Aprire la cartella Campi **personalizzati** non mappati.

   ![](assets/two.png)

1. Trascinate un campo personalizzato non mappato su un altro per mapparlo insieme.

   >[!NOTE]
   >
   >È possibile modificare solo le mappature dei campi personalizzate. Impossibile modificare le mappature dei campi standard.

   ![](assets/three.png)

1. Al termine, fate clic su **Fine mappe** .

   ![](assets/four.png)

## Interrompi mapping esistente {#break-existing-mapping}

Se avete campi con lo stesso nome sul lead e sull’oggetto di contatto Marketo li mapperà automaticamente. È possibile considerarli diversi e contenere dati diversi. Interrompete la mappatura in questo modo.

1. Fate clic su **Modifica mappature**.

   ![](assets/image2014-12-9-13-3a31-3a37.png)

1. Evidenzia un campo mappato e fai clic su **Mappatura** interruzioni per separare i campi.

   ![](assets/image2014-12-9-13-3a31-3a47.png)

1. Al termine, fate clic su **Fine mappe** .

   ![](assets/image2014-12-9-13-3a31-3a58.png)

   Bello! La sincronizzazione iniziale è quasi terminata.

## Ripristina schema {#reset-schema}

1. Se durante l&#39;elaborazione delle mappature si apportano delle modifiche allo schema in Salesforce, è possibile eseguire il pulling delle modifiche facendo clic su **Ripristina schema**.

   * Tutte le modifiche alla mappatura verranno ripristinate!
   * Reimpostando lo schema si aggiungeranno solo i campi, non li si rimuove (anche se li si nasconde dall&#39;utente della sincronizzazione).

   ![](assets/image2014-12-9-13-3a32-3a8.png)

