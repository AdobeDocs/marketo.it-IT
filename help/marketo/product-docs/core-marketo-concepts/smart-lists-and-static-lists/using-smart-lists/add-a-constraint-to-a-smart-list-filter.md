---
unique-page-id: 2949413
description: Aggiungere un vincolo a un filtro di elenco avanzato - Documentazione di Marketo - Documentazione del prodotto
title: Aggiungere un vincolo a un filtro dell’elenco avanzato
exl-id: 5345019c-55e7-4afd-b583-90f1a687a71c
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 9%

---

# Aggiungere un vincolo a un filtro dell’elenco avanzato {#add-a-constraint-to-a-smart-list-filter}

Durante la creazione di un elenco avanzato, alcuni filtri dispongono di opzioni avanzate denominate &quot;vincoli&quot;. Si tratta di condizioni aggiuntive che puoi aggiungere ai filtri e ai trigger per restringere ulteriormente la ricerca.

In questo esempio, aggiungiamo alcuni vincoli a un filtro **[Valore dati modificato](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}** per trovare persone con uno stato cambiato da MQL a SQL.

>[!PREREQUISITES]
>
>* [Creare un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Utilizzare il filtro &quot;Valore dati modificato&quot; in un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md){target="_blank"}

1. Vai a **[!UICONTROL Marketing Activities]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-1.png)

1. Selezionare l&#39;elenco avanzato con un filtro a cui aggiungere un vincolo e fare clic sulla scheda **[!UICONTROL Smart List]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-2.png)

1. In **[!UICONTROL Add Constraint]**, selezionare **[!UICONTROL Previous Value]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-3.png)

1. Immettere **[!UICONTROL Previous Value]**. In questo esempio, utilizziamo MQL.

   ![](assets/add-a-constraint-to-a-smart-list-filter-4.png)

1. In **[!UICONTROL Add Constraint]**, selezionare **[!UICONTROL New Value]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-5.png)

1. Immetti il nuovo valore. In questo esempio, utilizziamo SQL.

   ![](assets/add-a-constraint-to-a-smart-list-filter-6.png)

1. Ben fatto! Fare clic sulla scheda **[!UICONTROL People]** per visualizzare tutte le persone che hanno avuto un cambiamento di stato da &quot;MQL&quot; a &quot;SQL&quot; negli ultimi 30 giorni.
