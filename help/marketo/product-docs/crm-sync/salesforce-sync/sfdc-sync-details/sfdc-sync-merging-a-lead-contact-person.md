---
unique-page-id: 7515133
description: Sincronizzazione SFDC - Unione di lead/contatti/persone - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Unione di lead/contatti/persone
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---

# Sincronizzazione SFDC: unione di lead/contatti/persone {#sfdc-sync-merging-a-lead-contact-person}

A volte è meglio elencare semplicemente le regole. Eccoci qui:

* Quando si uniscono due lead in **Salesforce**, la sincronizzazione normale comunica a Marketo e ai lead di essere uniti automaticamente come persone in Marketo.
* Unione di due persone in **Marketo** richiama in realtà lo stesso processo di unione dei lead in Salesforce. Funziona comunque automaticamente.
* Unione di un **lead (persona) in un contatto** funziona allo stesso modo. Si finisce con un unico contatto su entrambi i lati.
* Durante l’unione, viene sommato il punteggio predefinito.

>[!NOTE]
>
>L’unione di 3 lead (persone) con un punteggio di 10 ciascuno genera il risultato di 1 lead (persona) con un punteggio di 30.

* I valori dei campi in conflitto vengono ricavati dal &quot;record vincente&quot;. (Record = lead o contatto risultante)
* Se il &quot;record perdente&quot; (quello che sta scomparendo) ha un valore e il record vincente non ha alcun valore, manterremo il record perdente. In altre parole, &quot;Un certo valore è meglio di nessun valore&quot;.
* Tutti gli elementi del registro attività vengono uniti.

>[!NOTE]
>
>Approfondimento per ulteriori informazioni su [unione di persone in Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md).
