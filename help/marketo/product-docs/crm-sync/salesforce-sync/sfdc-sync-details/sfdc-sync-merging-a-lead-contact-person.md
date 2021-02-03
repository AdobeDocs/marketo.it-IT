---
unique-page-id: 7515133
description: Sincr. SFDC - Unione di un lead/contatto/persona - Documenti Marketo - Documentazione del prodotto
title: Sincr. SFDC - Unione di un lead/contatto/persona
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# Sincr. SFDC: Unione di un lead/contatto/persona {#sfdc-sync-merging-a-lead-contact-person}

A volte è meglio elencare le regole. Ecco:

* Quando si uniscono due lead in **Salesforce**, la sincronizzazione normale indica Marketo e i lead vengono uniti automaticamente come persone in Marketo.
* L&#39;unione di due persone in **Marketo** in realtà richiama lo stesso processo di unione come lead in Salesforce. Funziona ancora automaticamente.
* L&#39;unione di un **lead (persona) in un contatto** funziona allo stesso modo. Si finisce con un unico contatto su entrambi i lati.
* Durante l&#39;unione, il punteggio predefinito viene sommato.

>[!NOTE]
>
>L’unione di 3 lead (persone) con punteggi di 10 ciascuno darà come risultato un risultato di 1 lead (persona) con un punteggio di 30.

* I valori dei campi in conflitto sono ricavati dal &quot;record vincente&quot;. (Record = il lead o contatto risultante)
* Se il &quot;record di perdita&quot; (quello che sta scomparendo) aveva un valore e il record di vincita non ne ha uno, manterremo il record di perdita. In altre parole, &quot;Alcuni valori sono migliori di nessun valore.&quot;
* Tutti gli elementi del registro attività vengono uniti.

>[!NOTE]
>
>Indagine approfondita per ulteriori informazioni sull [unione di persone in Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md).
