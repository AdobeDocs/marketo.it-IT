---
unique-page-id: 557322
description: Eseguire un singolo passaggio di flusso da un elenco avanzato - Documenti Marketo - Documentazione del prodotto
title: Eseguire un singolo passaggio di flusso da un elenco avanzato
exl-id: 1ac5795b-1906-4f94-bd0a-570d55c9357b
feature: Smart Lists
source-git-commit: 8a5903fa5313e34f448f833f20ab8e3624cf23e6
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Eseguire un singolo passaggio di flusso da un elenco avanzato {#run-a-single-flow-step-from-a-smart-list}

Se desideri eseguire un passaggio di flusso una tantum, puoi utilizzare un singolo passaggio di flusso all’interno di un elenco avanzato invece di creare un’intera campagna avanzata.

>[!PREREQUISITES]
>
>[Creare un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. Vai a **[!UICONTROL Attività di marketing]**.

   ![](assets/login-marketing-activities-1.png)

1. Seleziona un elenco o un elenco avanzato contenente persone, quindi vai alla scheda **[!UICONTROL Persone]**.

   ![](assets/smartlistpeopletab-hands.png)

   >[!TIP]
   >
   >Questa funzionalità è disponibile sia per gli elenchi statici che per gli elenchi avanzati.

1. Fare clic su **[!UICONTROL Seleziona tutto]**. È inoltre possibile utilizzare **Ctrl/Comando** e fare clic per selezionare alcuni record manualmente.

   ![](assets/smartlist-selectallhand.png)

   >[!NOTE]
   >
   >Se i risultati si estendono su più pagine, facendo clic su **[!UICONTROL Seleziona tutto]** verranno selezionate tutte le persone in tutte le pagine.

1. In **[!UICONTROL Azioni persona]**, seleziona il passaggio di flusso desiderato. In questo esempio utilizzeremo [Modifica valore dati](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}.

   ![](assets/personactions-hands.png)

1. Trova e seleziona un **[!UICONTROL attributo]**. In questo esempio prenderemo tutte le persone che hanno lo stato &quot;California&quot; e lo cambieremo in &quot;CA&quot;.

   ![](assets/runaction-hands.png)

1. Immetti un nuovo valore. Fare clic su **[!UICONTROL Esegui ora]**.

   ![](assets/runactionnewvalue-hands.png)

1. Se i valori dei dati vengono modificati per un numero elevato di persone, potrebbe essere necessario confermare la modifica digitando il numero. Fai Clic Su **[!UICONTROL Vai]**.

   ![](assets/changedatavalue.jpg)

Ottimo lavoro! Lo stato del singolo passaggio di flusso viene visualizzato nell’angolo in alto a destra.

![](assets/completesingleflowaction.jpg)

Al termine, aggiorna l’elenco e vedrai le informazioni aggiornate.
