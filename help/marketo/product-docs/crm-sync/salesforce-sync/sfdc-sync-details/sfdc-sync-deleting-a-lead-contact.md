---
unique-page-id: 7515131
description: Sincronizzazione SFDC - Eliminazione di un lead/contatto - Documentazione Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Eliminazione di un lead/contatto
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 4%

---

# Sincronizzazione SFDC: eliminazione di un lead/contatto {#sfdc-sync-deleting-a-lead-contact}

Ecco alcuni dettagli:

* Marketo non elimina automaticamente le persone solo perché i lead sono stati eliminati in [!DNL Salesforce]. Piuttosto, il flag &quot;SFDC Is Deleted&quot; del campo è impostato su true. Se necessario, puoi disattivare questo campo per eliminarlo in Marketo.
* [Elimina persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) azione di flusso. In questo modo verrà eliminata una persona in MKTO, ma è possibile scegliere di eliminare anche `Salesforce`.

* [Azione di flusso Elimina da SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md): elimina un lead in SFDC, ma è possibile eliminare una persona anche in Marketo.
* Se un lead viene eliminato in [!DNL Salesforce] (ma una persona non viene eliminata in Marketo) e successivamente viene eseguito tramite l&#39;azione di flusso [Sincronizza con [!DNL Salesforce]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md), verrà creato un nuovo lead in [!DNL Salesforce].
