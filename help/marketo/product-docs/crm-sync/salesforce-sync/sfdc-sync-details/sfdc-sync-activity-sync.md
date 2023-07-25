---
unique-page-id: 2953473
description: Sincronizzazione SFDC - Sincronizzazione attività - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Sincronizzazione attività
exl-id: 780e9cb7-b8b2-4a79-a0b8-d9d34a655330
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---

# Sincronizzazione SFDC: sincronizzazione attività {#sfdc-sync-activity-sync}

Marketo esegue anche la sincronizzazione sui dati delle attività Salesforce. Ecco alcune domande e risposte.

## Su quali tipi di dati attività viene eseguita la sincronizzazione con Marketo? {#what-types-of-activity-data-does-marketo-sync-over}

Marketo esegue la sincronizzazione di eventi e attività associati a un lead o a un contatto.

## In che modo i dettagli dell’attività vengono mantenuti sincronizzati tra i due sistemi? {#how-are-activity-details-kept-in-sync-between-the-two-systems}

La sincronizzazione è unidirezionale, da Salesforce a Marketo. Ma puoi creare un’attività in Salesforce utilizzando [Crea attività](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) passaggio di flusso o [Personalizza sincronizzazione attività](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md) a Salesforce.

## Posso creare un&#39;attività con Marketo? {#can-i-create-a-task-using-marketo}

Sì, è possibile utilizzare [Azione Crea flusso di attività](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md).

## Quali sono i trigger/filtri relativi all’attività? {#what-are-the-triggers-filters-related-to-activity}

Triggers

* Attività registrata
* L&#39;attività è aggiornata

Filtri

* Attività registrata/non registrata
* L&#39;attività è stata aggiornata/l&#39;attività non è stata aggiornata

>[!TIP]
>
>Non sei sicuro della dicitura &quot;Non attività&quot;? Il termine &quot;non&quot; si riferisce a un filtro di inattività. Ulteriori informazioni su di essi qui: [Utilizzare i filtri di inattività in un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)
