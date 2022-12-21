---
unique-page-id: 10094188
description: Approvare un oggetto personalizzato - Documenti Marketo - Documentazione del prodotto
title: Approvare un oggetto personalizzato
exl-id: 8bae94df-91fe-4722-8c75-c26df882c65d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Approvare un oggetto personalizzato {#approve-a-custom-object}

È necessario approvare un oggetto personalizzato prima di poterlo utilizzare. Il processo è leggermente diverso per i nuovi oggetti personalizzati e per quelli modificati.

## Approvare un nuovo oggetto personalizzato {#approve-a-new-custom-object}

È stato creato un nuovo oggetto personalizzato. Ecco come approvarlo.

1. In Admin, fai clic su **Oggetti personalizzati Marketo** e selezionare un oggetto in stato Bozza.

   ![](assets/one.png)

1. Fai clic sul pulsante **Azioni oggetto personalizzate** a discesa e seleziona **Approva oggetto**.

   ![](assets/two.png)

1. Lo stato diventa Approvato.

   ![](assets/three.png)

   >[!NOTE]
   >
   >Un oggetto personalizzato utilizzato in un _struttura uno-a-molti_ devono avere almeno un campo di deduplicazione, un campo di collegamento, un nome di oggetto collegato e un nome di campo collegato da approvare.
   >
   >Un oggetto personalizzato utilizzato in un _struttura molti-a-molti_ **non** quando lo si approva, è necessario disporre di un campo di collegamento, di un nome di oggetto collegato o di un nome di campo collegato, in quanto si trovano nell’oggetto intermedio.
   >
   >Un oggetto personalizzato utilizzato come _oggetto intermediario_ richiede un campo di collegamento, un nome oggetto collegato e un nome campo collegato, ma **non** richiede un campo di deduplicazione.
   >
   >Vedi [Informazioni sugli oggetti personalizzati Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) per ulteriori informazioni.

Tutto qui! Ora puoi selezionare l’oggetto personalizzato nei vincoli dei filtri e dei trigger da utilizzare nelle campagne.

## Approvare un oggetto personalizzato modificato {#approve-an-edited-custom-object}

Dopo aver modificato un oggetto personalizzato approvato, è necessario approvare la bozza per restituire l&#39;oggetto personalizzato a uno stato Approvato.

1. Quando si modifica un oggetto personalizzato già approvato, questo riceve uno stato Approvato con stato Bozza.

   ![](assets/four.png)

1. Quando sei pronto per approvare la bozza, fai clic sul pulsante **Azioni oggetto personalizzate** a discesa e seleziona **Approva oggetto**.

   ![](assets/five-1.png)

1. Nell&#39;anteprima vengono visualizzati gli elementi modificati nella bozza. Fai clic su **Approva**.

   ![](assets/six-1.png)
