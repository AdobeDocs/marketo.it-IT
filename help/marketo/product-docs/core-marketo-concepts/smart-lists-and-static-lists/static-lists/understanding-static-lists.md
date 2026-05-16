---
unique-page-id: 2949891
description: Scopri gli elenchi statici in Marketo per set fissi di persone. Utilizzare gli elenchi statici quando l'appartenenza viene gestita manualmente.
title: Informazioni sugli elenchi statici
exl-id: c37c1496-cf19-4e44-aaec-77b10669b9bf
feature: Static Lists
TQID: https://experienceleague.adobe.com/rRi3-6ZggKswYYLTZjUr5EBDNoMRirDc1KJgHbbDqP4
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
subfeature_v2:
  - id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 222
ht-degree: 4%

---

# Informazioni sugli elenchi statici {#understanding-static-lists}

Gli elenchi statici sono una delle funzioni più semplici e utili di Marketo. Si tratta di un elenco di nomi del database. Troverai molti motivi per utilizzarli.

>[!NOTE]
>
>Una singola persona nel database può trovarsi in molti elenchi statici diversi.

La differenza tra elenco statico e elenco avanzato è fondamentale per comprendere.

| Tipo | Logica |
|---|---|
| Elenco avanzato | In base a **regole definite** |
| Elenco statico | In base a **aggiunta/rimozione di ogni persona** |

>[!CAUTION]
>
>Uno degli errori più comuni consiste nel pensare di poter rimuovere una persona da un elenco &quot;eliminandola&quot;. **Errore**. Se si elimina la persona, verranno eliminati da **tutto il database**, non solo dall&#39;elenco.

## Modi per aggiungere o rimuovere persone da un elenco {#ways-to-add-remove-people-from-a-list}

1. Passaggio del flusso di Smart Campaign ([Aggiungi all&#39;elenco](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-to-list.md){target="_blank"}, [Rimuovi dall&#39;elenco](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-list.md){target="_blank"})

1. [Passaggio del flusso di azione singolo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/run-a-single-flow-step-from-a-smart-list.md){target="_blank"}
1. Trascinare le persone in un elenco nella struttura
1. [Importazione elenco](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md){target="_blank"}

## Alcuni utilizzi di un elenco statico {#some-uses-of-a-static-list}

* Elenco preselezionato per ricevere un messaggio di marketing.
* Una lista di &quot;concorrenti&quot; che usi per inviare messaggi di contro-intelligence maliziosi.
* Un elenco temporaneo di persone in un particolare stato, che vengono quindi rimosse da Smart Campaigns quando escono da tale stato.

>[!MORELIKETHIS]
>
>[Creare un elenco statico](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md){target="_blank"}
