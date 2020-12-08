---
unique-page-id: 7515133
description: Sincr. SFDC -Unione di un lead/contatto/persona - Documenti Marketo - Documentazione del prodotto
title: Sincr. SFDC - Unione di un lead/contatto/persona
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---


# Sincr. SFDC: Unione di un lead/contatto/persona {#sfdc-sync-merging-a-lead-contact-person}

>[!NOTE]
>
>**FYI**
>
>Marketo sta ora standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che l&#39;iscrizione contenga lead/lead e la persona/persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

A volte è meglio elencare le regole. Ecco:

* Quando si uniscono due lead in **Salesforce**, la sincronizzazione normale indica a Marketo che i lead vengono uniti automaticamente come persone in Marketo.
* L&#39;unione di due persone in **Marketo** richiama in realtà lo stesso processo dell&#39;unione di due persone come lead in Salesforce. Funziona ancora automaticamente.
* L’unione di un **lead (persona) in un contatto** funziona allo stesso modo. Si finisce con un unico contatto su entrambi i lati.
* Durante l&#39;unione, il punteggio predefinito viene sommato.

>[!NOTE]
>
>**Esempio**
>
>L’unione di 3 lead (persone) con punteggi di 10 ciascuno darà come risultato un risultato di 1 lead (persona) con un punteggio di 30.

* I valori dei campi in conflitto sono ricavati dal &quot;record vincente&quot;. (Record = il lead o contatto risultante)
* Se il &quot;record di perdita&quot; (quello che sta scomparendo) aveva un valore e il record di vincita non ne ha uno, manterremo il record di perdita. In altre parole, &quot;Alcuni valori sono migliori di nessun valore.&quot;
* Tutti gli elementi del registro attività vengono uniti.

>[!NOTE]
>
>**Tubo profondo**
>
>Immergiti in profondità per maggiori informazioni sull&#39; [unione di persone a Marketo](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md).

