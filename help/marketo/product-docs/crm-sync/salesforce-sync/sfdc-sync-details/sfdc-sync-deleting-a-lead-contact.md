---
unique-page-id: 7515131
description: Sincr. SFDC - Eliminazione di un lead/contatto - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Eliminazione di un lead/contatto
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---

# Sincr. SFDC: Eliminazione di un lead/contatto {#sfdc-sync-deleting-a-lead-contact}

Ecco alcuni dettagli:

* Marketo non elimina automaticamente le persone solo perché i lead sono stati cancellati in Salesforce. Il flag &quot;SFDC Is Deleted&quot; è invece impostato su true. Se lo desideri, puoi attivare questo campo per eliminarlo in Marketo.
* [Elimina persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) azione di flusso. Questo elimina una persona in MKTO ma puoi scegliere di eliminarla `Salesforce` anche.

* [Elimina da SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) azione di flusso: Questo elimina un lead in SFDC ma puoi scegliere di eliminare una persona anche in Marketo.
* Se un lead viene eliminato in Salesforce (ma una persona non viene eliminata in Marketo) ed esegue successivamente il [Sincronizzazione con Salesforce](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) azione di flusso, quindi creerebbe un nuovo lead in Salesforce.
