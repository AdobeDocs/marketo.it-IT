---
unique-page-id: 7515131
description: Sincr. SFDC -Eliminazione di un lead/contatto - Documenti Marketo - Documentazione del prodotto
title: Sincr. SFDC - Eliminazione di un lead/contatto
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---


# Sincr. SFDC: Eliminazione di un lead/contatto {#sfdc-sync-deleting-a-lead-contact}

Di seguito sono riportati alcuni dettagli:

* Marketo non elimina automaticamente le persone solo perché i lead sono stati eliminati in Salesforce. Piuttosto, il flag &quot;SFDC Is Deleted&quot; del campo è impostato su true. Se lo desideri, puoi disattivare questo campo per eliminarlo in Marketo.
* [Elimina azione ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) flusso di lavoro. In questo modo viene eliminata una persona in MKTO, ma è possibile scegliere di eliminarla anche in `Salesforce`.

* [Elimina da azione ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) SFDCflow: In questo modo si elimina un lead in SFDC, ma si può anche scegliere di eliminarlo in Marketo.
* Se un lead viene eliminato in Salesforce (ma una persona non viene eliminata in Marketo) ed eseguito successivamente tramite l&#39;azione di flusso [Sincronizza con Salesforce](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md), creerà un nuovo lead in Salesforce.
