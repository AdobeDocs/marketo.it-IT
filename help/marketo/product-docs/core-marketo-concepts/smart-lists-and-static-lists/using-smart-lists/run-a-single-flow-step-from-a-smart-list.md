---
unique-page-id: 557322
description: Scopri come eseguire un singolo passaggio di flusso da un elenco avanzato. Esegui un'azione di flusso per le persone selezionate dall'elenco.
title: Eseguire un passaggio di flusso singolo da un elenco avanzato
exl-id: 1ac5795b-1906-4f94-bd0a-570d55c9357b
feature: Smart Lists
TQID: 'https://experienceleague.adobe.com/GdWQiObUSnllii3M8x1bTuHRByAtg-UF03V-3sOuI9I'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
subfeature_v2:
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
    internal-label: Smart lists
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 10%
---
# Eseguire un passaggio di flusso singolo da un elenco avanzato {#run-a-single-flow-step-from-a-smart-list}

Se desideri eseguire un passaggio di flusso una tantum, puoi utilizzare un singolo passaggio di flusso all’interno di un elenco avanzato invece di creare un’intera campagna avanzata.

>[!PREREQUISITES]
>
>[Creare un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. Passa a **[!UICONTROL Marketing Activities]**.

   ![](assets/run-a-single-flow-step-from-a-smart-list-1.png)

1. Selezionare un elenco o un elenco avanzato contenente persone, quindi passare alla scheda **[!UICONTROL People]**.

   ![](assets/run-a-single-flow-step-from-a-smart-list-2.png)

   >[!TIP]
   >
   >Questa funzionalità è disponibile sia per gli elenchi statici che per gli elenchi avanzati.

1. Fai clic su **[!UICONTROL Select All]**. È inoltre possibile utilizzare **Ctrl/Comando** e fare clic per selezionare alcuni record manualmente.

   ![](assets/run-a-single-flow-step-from-a-smart-list-3.png)

   >[!NOTE]
   >
   >Se i risultati si estendono su più pagine, facendo clic su **[!UICONTROL Select All]** verranno selezionate tutte le persone in tutte le pagine.

1. In **[!UICONTROL Person Actions]**, selezionare il passaggio di flusso desiderato. In questo esempio viene utilizzato [Modifica valore dati](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}.

   ![](assets/run-a-single-flow-step-from-a-smart-list-4.png)

1. Trova e seleziona un **[!UICONTROL Attribute]**. In questo esempio prenderemo tutte le persone che hanno lo stato &quot;California&quot; e lo cambieremo in &quot;CA&quot;.

   ![](assets/run-a-single-flow-step-from-a-smart-list-5.png)

1. Immetti un nuovo valore. Fai clic su **[!UICONTROL Run Now]**.

   ![](assets/run-a-single-flow-step-from-a-smart-list-6.png)

1. Se si modificano i valori dei dati per un numero elevato di persone, potrebbe essere necessario confermare la modifica digitando il numero. Fai clic su **[!UICONTROL Go For It]**.

   ![](assets/run-a-single-flow-step-from-a-smart-list-7.png)

Lo stato del singolo passaggio di flusso viene visualizzato nell’angolo in alto a destra.

![](assets/run-a-single-flow-step-from-a-smart-list-8.png)

Al termine, aggiorna l’elenco e vedrai le informazioni aggiornate.
