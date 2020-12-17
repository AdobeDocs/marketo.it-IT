---
unique-page-id: 2949413
description: Aggiunta di un vincolo a un filtro di elenco avanzato - Documenti Marketo - Documentazione prodotto
title: Aggiunta di un vincolo a un filtro elenco avanzato
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---


# Aggiungere un vincolo a un filtro elenco avanzato {#add-a-constraint-to-a-smart-list-filter}

Durante la creazione di elenchi avanzati, alcuni filtri presentano opzioni avanzate denominate *limitazioni. *Queste sono condizioni aggiuntive che è possibile aggiungere a filtri e attivatori per aiutare a restringere ulteriormente la ricerca.

In questo esempio, aggiungiamo alcuni vincoli a un filtro ** [Valore dati modificato](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)** per individuare le persone che hanno subito una modifica dello stato da MQL a SQL.

>[!PREREQUISITES]
>
>* [Creare un elenco avanzato](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
>* [Usare il filtro &quot;Valore dati modificato&quot; in un elenco avanzato](use-the-data-value-changed-filter-in-a-smart-list.md)

>



1. Andate a **Marketing Activities**.

   ![](assets/ma-1.png)

1. Selezionare l&#39;elenco smart con un filtro a cui si desidera aggiungere un vincolo e fare clic sulla scheda **Smart List**.

   ![](assets/two-3.png)

1. In **Aggiungi vincolo**, selezionare **Valore precedente**.

   ![](assets/three-3.png)

1. Immettere il **Valore precedente**. In questo esempio stiamo utilizzando MQL.

   ![](assets/four-2.png)

1. In **Aggiungi vincolo**, selezionare **Nuovo valore**.

   ![](assets/five.png)

1. Immettere il **Nuovo valore**. In questo esempio stiamo utilizzando SQL.

   ![](assets/six.png)

1. Ben fatto! Fare clic sulla scheda **Persone** per vedere tutte le persone che hanno avuto una **Stato** modifica da **MQL** a **SQL** negli ultimi 30 giorni.

