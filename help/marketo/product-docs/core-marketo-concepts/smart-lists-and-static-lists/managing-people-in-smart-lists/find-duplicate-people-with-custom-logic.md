---
unique-page-id: 2952636
description: Trova persone duplicate con logica personalizzata - Documentazione Marketo - Documentazione del prodotto
title: Trova persone duplicate con logica personalizzata
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
feature: Smart Lists
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '124'
ht-degree: 0%

---

# Trova persone duplicate con logica personalizzata {#find-duplicate-people-with-custom-logic}

Marketo Engage dispone di un elenco avanzato del sistema che trova le persone duplicate in base ai loro indirizzi e-mail. Se desideri utilizzare un altro campo per trovare duplicati con, ecco come.

>[!PREREQUISITES]
>
>[Creare un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. Passare all&#39;area **[!UICONTROL Marketing Activities]**.

![](assets/ma-2.png)

1. Selezionare l&#39;elenco avanzato e fare clic sulla scheda **[!UICONTROL Smart List]**.

   ![](assets/two-4.png)

1. Trovare e trascinare il filtro **[!UICONTROL Duplicate Fields]** nell&#39;area di lavoro.

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

   Fine. Esegui Smart List per trovare persone con lo stesso valore nel campo selezionato in precedenza.
