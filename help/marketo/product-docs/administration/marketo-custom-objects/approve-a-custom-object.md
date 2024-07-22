---
unique-page-id: 10094188
description: Approvare un oggetto personalizzato - Documentazione di Marketo - Documentazione del prodotto
title: Approvare un oggetto personalizzato
exl-id: 8bae94df-91fe-4722-8c75-c26df882c65d
feature: Custom Objects
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# Approvare un oggetto personalizzato {#approve-a-custom-object}

È necessario approvare un oggetto personalizzato prima di poterlo utilizzare. Il processo è leggermente diverso per i nuovi oggetti personalizzati e per quelli che hai modificato.

## Approva un nuovo oggetto personalizzato {#approve-a-new-custom-object}

Hai creato un nuovo oggetto personalizzato. Ecco come approvarlo.

1. Vai all&#39;area **[!UICONTROL Amministratore]**.

   ![](assets/approve-a-custom-object-1.png)

1. Fare clic su **[!UICONTROL Oggetti personalizzati Marketo]**.

   ![](assets/approve-a-custom-object-2.png)

1. Selezionate un oggetto in stato Bozza.

   ![](assets/approve-a-custom-object-3.png)

1. Fai clic sul menu a discesa **[!UICONTROL Azioni oggetto personalizzato]** e seleziona **[!UICONTROL Approva oggetto]**.

   ![](assets/approve-a-custom-object-4.png)

1. Lo stato diventa [!UICONTROL Approvato].

   ![](assets/approve-a-custom-object-5.png)

   >[!NOTE]
   >
   >Un oggetto personalizzato utilizzato in una struttura _uno-a-molti_ deve avere almeno un campo di deduplicazione, un campo di collegamento, un nome di oggetto collegato e un nome di campo collegato da approvare.
   >
   >Un oggetto personalizzato utilizzato in una struttura _many-to-many_ **non richiede un campo collegamento, un nome di oggetto collegato o un nome di campo collegato quando viene approvato (perché risiedono nell&#39;oggetto intermedio).**
   >
   >Un oggetto personalizzato utilizzato come _oggetto intermedio_ richiede un campo di collegamento, un nome di oggetto collegato e un nome di campo collegato, ma **non richiede un campo di deduplicazione**.
   >
   >Per ulteriori informazioni, vedere [Informazioni sugli oggetti personalizzati di Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md).

Tutto qui! Ora puoi selezionare l’oggetto personalizzato nei vincoli dei filtri e dei trigger da utilizzare nelle campagne.

## Approvare un oggetto personalizzato modificato {#approve-an-edited-custom-object}

Dopo aver modificato un oggetto personalizzato approvato, è necessario approvare la bozza per ripristinare lo stato Approvato dell&#39;oggetto personalizzato.

1. Quando modifichi un oggetto personalizzato già approvato, riceve lo stato [!UICONTROL Approvato con bozza].

   ![](assets/approve-a-custom-object-6.png)

1. Quando sei pronto ad approvare la bozza, fai clic sul menu a discesa **[!UICONTROL Azioni oggetto personalizzato]** e seleziona **[!UICONTROL Approva oggetto]**.

   ![](assets/approve-a-custom-object-7.png)

1. Un’anteprima mostra gli elementi modificati nella bozza. Fai clic su **[!UICONTROL Approva]**.

   ![](assets/approve-a-custom-object-8.png)
