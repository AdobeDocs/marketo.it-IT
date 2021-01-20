---
unique-page-id: 557322
description: Eseguire un singolo passaggio di flusso da un elenco avanzato - Marketo Docs - Documentazione prodotto
title: Eseguire un singolo passaggio di flusso da un elenco avanzato
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---


# Eseguire un singolo passaggio di flusso da un elenco avanzato {#run-a-single-flow-step-from-a-smart-list}

Se si desidera eseguire un solo passaggio di flusso una tantum, è possibile utilizzare un singolo passaggio di flusso all&#39;interno di un elenco smart invece di creare un&#39;intera campagna smart.

>[!PREREQUISITES]
>
>[Creare un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. Andate a **Marketing Activities**.

   ![](assets/login-marketing-activities-1.png)

1. Selezionate un elenco o un elenco smart con le persone al suo interno, quindi passate alla scheda **Persone**.

   ![](assets/smartlistpeopletab-hands.png)

   >[!TIP]
   >
   >Questa funzionalità è disponibile sia per gli elenchi statici che per gli elenchi avanzati.

1. Fare clic su **Seleziona tutto**. È inoltre possibile utilizzare **Ctrl/Cmd** e fare clic per selezionare alcuni record manualmente.

   ![](assets/smartlist-selectallhand.png)

   >[!NOTE]
   >
   >Se i risultati si estendono su più pagine, facendo clic su **Seleziona tutto** si selezioneranno tutte le persone su tutte le pagine.

1. In **Person** **Actions**, selezionare il passaggio di flusso desiderato. In questo esempio verrà utilizzato [Change Data Value](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md).

   ![](assets/personactions-hands.png)

1. Trovare e selezionare un **attributo**. In questo esempio prenderemo tutte le persone che hanno lo stato &quot;California&quot; e lo cambieremo in &quot;CA&quot;.

   ![](assets/runaction-hands.png)

1. Immettete un nuovo valore. Fare clic su **Esegui ora**.

   ![](assets/runactionnewvalue-hands.png)

1. Se si modificano i valori dei dati per un numero elevato di persone, potrebbe essere necessario confermare la modifica digitando il numero. Fare clic su **Vai per**.

   ![](assets/changedatavalue.jpg)

Impressionante lavoro! Nell’angolo in alto a destra viene visualizzato lo stato del singolo passaggio di scorrimento.

![](assets/completesingleflowaction.jpg)

Al termine, aggiorna l&#39;elenco e vedrai le informazioni aggiornate.
