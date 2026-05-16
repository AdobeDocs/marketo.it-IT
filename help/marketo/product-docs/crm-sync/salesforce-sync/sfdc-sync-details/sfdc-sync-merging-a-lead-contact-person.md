---
unique-page-id: 7515133
description: Comprendi come funziona l’unione di lead, contatti e persone in Salesforce e Marketo. Scopri le regole di unione per punteggi, valori di campo e registri di attività.
title: Sincronizzazione SFDC - Unione di lead/contatti/persone
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/alPa6YMG0tgo08ruZAZlWhujV54iVcUMAAejXJbEQFw
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 204
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
