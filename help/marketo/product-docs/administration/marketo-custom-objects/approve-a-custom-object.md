---
unique-page-id: 10094188
description: Approvare un oggetto personalizzato - Documentazione di Marketo - Documentazione del prodotto
title: Approvare un oggetto personalizzato
exl-id: 8bae94df-91fe-4722-8c75-c26df882c65d
source-git-commit: 4a33b192cc22550c75769b383e261ac0a86e7ddb
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Approvare un oggetto personalizzato {#approve-a-custom-object}

È necessario approvare un oggetto personalizzato prima di poterlo utilizzare. Il processo è leggermente diverso per i nuovi oggetti personalizzati e per quelli che hai modificato.

## Approva un nuovo oggetto personalizzato {#approve-a-new-custom-object}

Hai creato un nuovo oggetto personalizzato. Ecco come approvarlo.

1. Vai a **[!UICONTROL Amministratore]** area.

   ![](assets/approve-a-custom-object-1.png)

1. Clic **[!UICONTROL Oggetti personalizzati Marketo]**.

   ![](assets/approve-a-custom-object-2.png)

1. Selezionate un oggetto in stato Bozza.

   ![](assets/approve-a-custom-object-3.png)

1. Fai clic su **[!UICONTROL Azioni oggetto personalizzato]** a discesa e selezionare **[!UICONTROL Approva oggetto]**.

   ![](assets/approve-a-custom-object-4.png)

1. Lo stato cambia in [!UICONTROL Approvato].

   ![](assets/approve-a-custom-object-5.png)

   >[!NOTE]
   >
   >Un oggetto personalizzato utilizzato in una _struttura uno-a-molti_ per essere approvato, deve essere presente almeno un campo di deduplicazione, un campo di collegamento, un nome di oggetto collegato e un nome di campo collegato.
   >
   >Un oggetto personalizzato utilizzato in una _struttura many-to-many_ **non** quando lo approvi, è necessario un campo collegamento, un nome di oggetto collegato o un nome di campo collegato, in quanto si trovano nell’oggetto intermedio.
   >
   >Un oggetto personalizzato utilizzato come _oggetto intermedio_ richiede un campo collegamento, un nome oggetto collegato e un nome campo collegato, ma **non** richiede un campo di deduplicazione.
   >
   >Consulta [Informazioni sugli oggetti personalizzati di Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) per ulteriori informazioni.

Tutto qui! Ora puoi selezionare l’oggetto personalizzato nei vincoli dei filtri e dei trigger da utilizzare nelle campagne.

## Approvare un oggetto personalizzato modificato {#approve-an-edited-custom-object}

Dopo aver modificato un oggetto personalizzato approvato, è necessario approvare la bozza per ripristinare lo stato Approvato dell&#39;oggetto personalizzato.

1. Quando si modifica un oggetto personalizzato già approvato, viene visualizzato un messaggio [!UICONTROL Approvato con bozza] stato.

   ![](assets/approve-a-custom-object-6.png)

1. Quando sei pronto ad approvare la bozza, fai clic sul pulsante **[!UICONTROL Azioni oggetto personalizzato]** a discesa e selezionare **[!UICONTROL Approva oggetto]**.

   ![](assets/approve-a-custom-object-7.png)

1. Un’anteprima mostra gli elementi modificati nella bozza. Clic **[!UICONTROL Approva]**.

   ![](assets/approve-a-custom-object-8.png)
