---
unique-page-id: 10094188
description: Approvare un oggetto personalizzato - Documenti Marketo - Documentazione del prodotto
title: Approvare un oggetto personalizzato
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# Approva un oggetto personalizzato {#approve-a-custom-object}

È necessario approvare un oggetto personalizzato prima di poterlo utilizzare. Il processo è leggermente diverso per i nuovi oggetti personalizzati e per quelli modificati.

## Approva un nuovo oggetto personalizzato {#approve-a-new-custom-object}

È stato creato un nuovo oggetto personalizzato. Ecco come approvarlo.

1. In Amministratore, fare clic su **Contrassegna oggetti personalizzati** e selezionare un oggetto che si trova nello stato Bozza.

   ![](assets/one.png)

1. Fare clic sul menu a discesa **Azioni oggetto personalizzate** e selezionare **Approva oggetto**.

   ![](assets/two.png)

1. Lo stato diventa Approvato.

   ![](assets/three.png)

   >[!NOTE]
   >
   >Un oggetto personalizzato utilizzato in una struttura _uno-a-molti_ deve avere almeno un campo di deduplicazione, un campo di collegamento, un nome oggetto collegato e un nome campo collegato da approvare.
   >
   >Un oggetto personalizzato utilizzato in una struttura _molti-a-molti_ **non** necessita di un campo di collegamento, di un nome oggetto collegato o di un nome campo collegato al momento dell&#39;approvazione (perché risiedono nell&#39;oggetto intermedio).
   >
   >Un oggetto personalizzato utilizzato come oggetto _intermediario_ richiede un campo di collegamento, un nome oggetto collegato e un nome campo collegato, ma **non richiede un campo duplicato.**
   >
   >Per ulteriori informazioni, vedere [Informazioni sugli oggetti personalizzati Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md).

È tutto! Ora puoi selezionare l&#39;oggetto personalizzato nei vincoli dei filtri e degli attivatori da utilizzare nelle campagne.

## Approvare un oggetto personalizzato modificato {#approve-an-edited-custom-object}

Dopo aver modificato un oggetto personalizzato approvato, è necessario approvare la bozza per restituire l&#39;oggetto personalizzato a uno stato Approvato.

1. Quando si modifica un oggetto personalizzato già approvato, viene ricevuto lo stato Approvato con bozza.

   ![](assets/four.png)

1. Quando si è pronti per approvare la bozza, fare clic sul menu a discesa **Azioni oggetto personalizzate** e selezionare **Approva oggetto**.

   ![](assets/five-1.png)

1. Un&#39;anteprima mostra gli elementi modificati nella bozza. Fare clic su **Approva**.

   ![](assets/six-1.png)
