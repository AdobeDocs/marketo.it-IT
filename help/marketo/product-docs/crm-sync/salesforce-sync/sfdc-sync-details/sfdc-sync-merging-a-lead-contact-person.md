---
unique-page-id: 7515133
description: Sincr. SFDC - Unione di un lead/contatto/persona - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Unione di un lead/contatto/persona
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---

# Sincr. SFDC: Unione di un lead/contatto/persona {#sfdc-sync-merging-a-lead-contact-person}

A volte è meglio elencare le regole. Ecco:

* Quando si uniscono due lead in **Salesforce**, la sincronizzazione normale comunica a Marketo e i lead vengono uniti automaticamente come persone in Marketo.
* Unione di due persone **Marketo** richiama effettivamente lo stesso processo di unione dei lead in Salesforce. Funziona ancora automaticamente.
* Unione di un **condurre (persona) in un contatto** funziona allo stesso modo. Si finisce con un unico contatto da entrambi i lati.
* Durante l’unione, il punteggio predefinito viene sommato.

>[!NOTE]
>
>L’unione di 3 lead (persone) con punteggi di 10 ciascuno darà il risultato di 1 lead (persona) con un punteggio di 30.

* I valori di campo in conflitto sono ricavati dal &quot;record vincente&quot;. (Record = lead o contatto risultante)
* Se il &quot;record perdente&quot; (quello che sta scomparendo) aveva un valore e il record vincente non ne ha, manterremo il record perdente. In altre parole, &quot;Alcuni valori sono migliori di nessun valore.&quot;
* Tutti gli elementi del registro attività vengono uniti.

>[!NOTE]
>
>Approfondimento per maggiori informazioni [unione di persone in Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md).
