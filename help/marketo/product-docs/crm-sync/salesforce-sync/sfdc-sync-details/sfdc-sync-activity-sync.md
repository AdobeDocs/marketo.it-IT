---
unique-page-id: 2953473
description: Sincr. SFDC -Sincronizzazione attività - Documenti Marketo - Documentazione del prodotto
title: Sincr. SFDC -Sincronizzazione attività
exl-id: 780e9cb7-b8b2-4a79-a0b8-d9d34a655330
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---

# Sincr. SFDC: Sincronizzazione attività {#sfdc-sync-activity-sync}

Marketo sincronizza anche i dati delle attività Salesforce. Ecco alcune domande e risposte.

## Su quali tipi di dati di attività si sincronizza Marketo? {#what-types-of-activity-data-does-marketo-sync-over}

Marketo sincronizza sia gli eventi che le attività associati a un lead o a un contatto.

## Come vengono mantenuti sincronizzati i dettagli dell’attività tra i due sistemi? {#how-are-activity-details-kept-in-sync-between-the-two-systems}

La sincronizzazione è un modo, da Salesforce a Marketo. Ma puoi creare un&#39;attività in Salesforce utilizzando il passaggio di flusso [Crea attività](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) o [Personalizza attività Sincronizza](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md) in Salesforce.

## Posso creare un&#39;attività utilizzando Marketo? {#can-i-create-a-task-using-marketo}

Sì, puoi utilizzare l&#39;azione [Crea flusso di attività](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md).

## Quali sono i trigger/filtri correlati all’attività? {#what-are-the-triggers-filters-related-to-activity}

Triggers

* L’attività viene registrata
* L’attività è stata aggiornata

Filtri

* L&#39;attività è stata registrata/Non è stata registrata
* L&#39;attività è stata aggiornata/L&#39;attività non è stata aggiornata

>[!TIP]
>
>Non sei sicuro della formulazione &quot;Not Activity&quot;? Il termine &quot;non&quot; si riferisce a un filtro di inattività. Ulteriori informazioni qui: [Utilizzare i filtri di inattività in un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)
