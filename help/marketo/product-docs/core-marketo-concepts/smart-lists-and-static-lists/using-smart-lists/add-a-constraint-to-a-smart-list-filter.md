---
unique-page-id: 2949413
description: Aggiunta di un vincolo a un filtro di elenco avanzato - Documenti Marketo - Documentazione prodotto
title: Aggiunta di un vincolo a un filtro elenco avanzato
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---


# Aggiunta di un vincolo a un filtro elenco avanzato {#add-a-constraint-to-a-smart-list-filter}

Durante la creazione di elenchi avanzati, alcuni filtri presentano opzioni avanzate denominate *limitazioni. *Queste sono condizioni aggiuntive che è possibile aggiungere a filtri e attivatori per aiutare a restringere ulteriormente la ricerca.

In questo esempio, aggiungiamo alcuni vincoli a un filtro ** Valore [dati modificato](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)** per individuare le persone che hanno subito una modifica dello stato da MQL a SQL.

>[!NOTE]
>
>**FYI**
>
>Marketo sta standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che nell&#39;abbonamento siano presenti lead/lead e persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

>[!PREREQUISITES]
>
>* [Creare un elenco avanzato](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
>* [Usare il filtro &quot;Valore dati modificato&quot; in un elenco avanzato](use-the-data-value-changed-filter-in-a-smart-list.md)

>



1. Vai a Attività **** di marketing.

   ![](assets/ma-1.png)

1. Selezionate l’elenco avanzato con un filtro a cui aggiungere un vincolo e fate clic sulla scheda Elenco **** avanzato.

   ![](assets/two-3.png)

1. In **Aggiungi vincolo**, selezionare Valore **** precedente.

   ![](assets/three-3.png)

1. Immettere il valore **** precedente. In questo esempio stiamo utilizzando MQL.

   ![](assets/four-2.png)

1. In **Aggiungi vincolo**, selezionare **Nuovo valore**.

   ![](assets/five.png)

1. Immettere il **nuovo valore**. In questo esempio stiamo utilizzando SQL.

   ![](assets/six.png)

1. Ben fatto! Fate clic sulla scheda **Persone** per vedere tutti gli utenti che hanno apportato una modifica **Stato** da **MQL** a **SQL** negli ultimi 30 giorni.

