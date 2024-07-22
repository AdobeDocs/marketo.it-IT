---
unique-page-id: 7515131
description: Sincronizzazione SFDC - Eliminazione di un lead/contatto - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Eliminazione di un lead/contatto
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---

# Sincronizzazione SFDC: eliminazione di un lead/contatto {#sfdc-sync-deleting-a-lead-contact}

Ecco alcuni dettagli:

* Il Marketo Engage non elimina automaticamente le persone solo perché i lead sono stati eliminati in Salesforce. Piuttosto, il flag &quot;SFDC Is Deleted&quot; del campo è impostato su true. Se necessario, puoi disattivare questo campo per eliminarlo in Marketo.
* [Elimina persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md){target="_blank"} azione di flusso. In questo modo verrà eliminata una persona in MKTO, ma è possibile scegliere di eliminare anche `Salesforce`.

* [Elimina da SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md){target="_blank"} azione di flusso: elimina un lead in SFDC, ma puoi scegliere di eliminare anche una persona in Marketo.
* Se un lead viene eliminato in Salesforce (ma una persona non viene eliminata in Marketo) e successivamente viene eseguita l&#39;azione di flusso [Sincronizza con Salesforce](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}, verrà creato un nuovo lead in Salesforce.
