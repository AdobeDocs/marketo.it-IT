---
unique-page-id: 557322
description: Eseguire un singolo passaggio di flusso da un elenco avanzato - Marketo Docs - Documentazione del prodotto
title: Eseguire un singolo passaggio di flusso da un elenco avanzato
exl-id: 1ac5795b-1906-4f94-bd0a-570d55c9357b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Eseguire un singolo passaggio di flusso da un elenco avanzato {#run-a-single-flow-step-from-a-smart-list}

Se desideri eseguire un solo passaggio di flusso una volta, puoi utilizzare un singolo passaggio di flusso all’interno di un elenco smart invece di creare un’intera campagna intelligente.

>[!PREREQUISITES]
>
>[Creare un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. Vai a **Attività di marketing**.

   ![](assets/login-marketing-activities-1.png)

1. Seleziona un elenco o un elenco smart con le persone incluse, quindi vai alla scheda **Persone** .

   ![](assets/smartlistpeopletab-hands.png)

   >[!TIP]
   >
   >Questa funzionalità è disponibile sia per gli elenchi statici che per gli elenchi avanzati.

1. Fare clic su **Seleziona tutto**. È inoltre possibile utilizzare **Ctrl/Cmd** e fare clic per selezionare alcuni record manualmente.

   ![](assets/smartlist-selectallhand.png)

   >[!NOTE]
   >
   >Se i risultati si estendono su più pagine, facendo clic su **Seleziona tutto** verranno selezionate tutte le persone in tutte le pagine.

1. In **Persona** **Azioni**, seleziona il passaggio di flusso desiderato. In questo esempio utilizzeremo [Cambia valore dati](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md).

   ![](assets/personactions-hands.png)

1. Trova e seleziona un **Attributo**. In questo esempio prenderemo tutte le persone che hanno lo stato &quot;California&quot; e lo cambieremo in &quot;CA&quot;.

   ![](assets/runaction-hands.png)

1. Immettere un nuovo valore. Fare clic su **Esegui ora**.

   ![](assets/runactionnewvalue-hands.png)

1. Se si modificano i valori dei dati per un numero elevato di persone, potrebbe essere necessario confermare la modifica digitando il numero. Fare clic su **Vai per**.

   ![](assets/changedatavalue.jpg)

Lavoro fantastico! Nell’angolo in alto a destra viene visualizzato lo stato del singolo passaggio di flusso.

![](assets/completesingleflowaction.jpg)

Al termine, aggiorna l’elenco e vedrai le informazioni aggiornate.
