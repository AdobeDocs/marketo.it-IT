---
unique-page-id: 7515131
description: Sincronizzazione SFDC - Eliminazione di un lead/contatto - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Eliminazione di un lead/contatto
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---

# Sincronizzazione SFDC: eliminazione di un lead/contatto {#sfdc-sync-deleting-a-lead-contact}

Ecco alcuni dettagli:

* Marketo non elimina automaticamente le persone solo perché i lead sono stati eliminati in Salesforce. Piuttosto, il flag &quot;SFDC Is Deleted&quot; del campo è impostato su true. Se necessario, puoi disattivare questo campo per eliminarlo in Marketo.
* [Elimina persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) azione di flusso. Questa operazione elimina una persona in MKTO, ma è possibile scegliere di eliminarla in `Salesforce` anche.

* [Elimina da SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) azione di flusso: elimina un lead in SFDC, ma puoi scegliere di eliminare anche una persona in Marketo.
* Se un lead viene eliminato in Salesforce (ma una persona non viene eliminata in Marketo) e successivamente viene eseguito attraverso il [Sincronizza con Salesforce](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) azione di flusso, per poi creare un nuovo lead in Salesforce.
