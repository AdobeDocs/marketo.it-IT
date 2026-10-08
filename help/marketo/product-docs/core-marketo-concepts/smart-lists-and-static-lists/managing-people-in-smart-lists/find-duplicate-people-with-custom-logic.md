---
unique-page-id: 2952636
description: Scopri come trovare persone duplicate con logica personalizzata. Crea un elenco avanzato per identificare i duplicati in base ai criteri.
title: Trovare persone duplicate con logica personalizzata
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
feature: Smart Lists
TQID: 'https://experienceleague.adobe.com/-NvWt-eEzngL0QY7Kyl6lfjd75WcoQmcq3IiN7Uc6-w'
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
source-wordcount: '135'
ht-degree: 17%
---
# Trovare persone duplicate con logica personalizzata {#find-duplicate-people-with-custom-logic}

Marketo Engage dispone di un elenco avanzato del sistema che trova le persone duplicate in base ai loro indirizzi e-mail. Se desideri utilizzare un altro campo per trovare duplicati con, segui i passaggi seguenti.

>[!PREREQUISITES]
>
>[Creare un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. Passa alla schermata **[!UICONTROL Marketing Activities]**.

![](assets/ma-2.png)

1. Selezionare l&#39;elenco avanzato e fare clic sulla scheda **[!UICONTROL Smart List]**.

   ![](assets/two-4.png)

1. Trova e trascina il filtro **[!UICONTROL Duplicate Fields]** nell&#39;area di lavoro.

   ![](assets/three-4.png)

1. Scegli una delle quattro opzioni disponibili:

   * [!UICONTROL Email Address]
   * [!UICONTROL Full Name]
   * [!UICONTROL Last Name]
   * [!UICONTROL Updated At]

   >[!NOTE]
   >
   >Tutti i campi, ad eccezione di Indirizzo e-mail, fanno distinzione tra maiuscole e minuscole. Pertanto, se si utilizza &quot;john doe&quot; nel campo Nome completo, _not_ restituirà risultati per John Doe.

   ![](assets/four-2.png)

   Esegui Smart List per trovare persone con lo stesso valore nel campo selezionato in precedenza.
