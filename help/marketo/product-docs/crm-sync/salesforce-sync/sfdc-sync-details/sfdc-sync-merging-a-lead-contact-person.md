---
unique-page-id: 7515133
description: Sincronizzazione SFDC - Unione di lead/contatti/persone - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Unione di lead/contatti/persone
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 3%

---

# Sincronizzazione SFDC: unione di lead/contatti/persone {#sfdc-sync-merging-a-lead-contact-person}

A volte è meglio elencare semplicemente le regole. Eccoci qui:

* Quando si uniscono due lead in **[!DNL Salesforce]**, la sincronizzazione normale comunica a Marketo e i lead vengono uniti automaticamente come persone in Marketo.
* L&#39;unione di due persone in **Marketo** richiama lo stesso processo utilizzato per unirle come lead in [!DNL Salesforce]. Funziona comunque automaticamente.
* L&#39;unione di un **lead (persona) in un contatto** funziona allo stesso modo. Si finisce con un unico contatto su entrambi i lati.
* Durante l’unione, viene sommato il punteggio predefinito.

>[!NOTE]
>
>L’unione di 3 lead (persone) con un punteggio di 10 ciascuno genera il risultato di 1 lead (persona) con un punteggio di 30.

* I valori dei campi in conflitto vengono ricavati dal &quot;record vincente&quot;. (Record = lead o contatto risultante)
* Se il &quot;record perdente&quot; (quello che sta scomparendo) ha un valore e il record vincente non ha alcun valore, manterremo il record perdente. In altre parole, &quot;Un certo valore è meglio di nessun valore&quot;.
* Tutti gli elementi del registro attività vengono uniti.

>[!NOTE]
>
>Approfondisci per ulteriori informazioni sull&#39;unione di [persone in Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target="_blank"}.
