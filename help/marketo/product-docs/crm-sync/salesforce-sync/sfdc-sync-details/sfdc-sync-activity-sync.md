---
unique-page-id: 2953473
description: Sincr. SFDC -Activity Sync - Marketo Docs - Documentazione del prodotto
title: Sincr. SFDC - Sincronizzazione attività
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---


# Sincr. SFDC: Sincronizzazione attività {#sfdc-sync-activity-sync}

Marketo sincronizza anche sui dati delle attività di Salesforce. Ecco alcune domande e risposte.

## Su quali tipi di dati di attività è sincronizzato Marketo? {#what-types-of-activity-data-does-marketo-sync-over}

Marketo si sincronizza sia sugli eventi che sulle attività associati a un lead o a un contatto.

## In che modo i dettagli dell&#39;attività vengono mantenuti sincronizzati tra i due sistemi? {#how-are-activity-details-kept-in-sync-between-the-two-systems}

La sincronizzazione è unidirezionale, da Salesforce a Marketo. Tuttavia, puoi creare un&#39;attività in Salesforce utilizzando il passaggio di flusso [Crea attività](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) o [Personalizza sincronizzazione attività](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md) in Salesforce.

## Posso creare un&#39;attività con Marketo? {#can-i-create-a-task-using-marketo}

Sì, è possibile utilizzare l&#39;azione [Crea flusso di attività](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md).

## Quali sono i trigger/filtri correlati all&#39;attività? {#what-are-the-triggers-filters-related-to-activity}

Triggers

* Attività registrata
* Attività aggiornata

Filtri

* Attività registrata/Attività non registrata
* Attività aggiornata/Attività non aggiornata

>[!TIP]
>
>Non sei sicuro della formulazione &quot;Not Activity&quot;? Il termine &quot;not&quot; si riferisce a un filtro di inattività. Per saperne di più, consulta: [Utilizzare i filtri per l&#39;inattività in un elenco avanzato](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)

