---
unique-page-id: 2953469
description: Sincronizzazione SFDC - Sincronizzazione campagne - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Sincronizzazione campagna
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Sincronizzazione SFDC: Sincronizzazione campagna {#sfdc-sync-campaign-sync}

I programmi Marketo possono essere sincronizzati con le campagne Salesforce. Ecco una panoramica di come funziona.

## Perché sincronizzare i programmi Marketo con le campagne Salesforce? {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* Utilizza le potenti funzioni di un programma Marketo.
* Mantieni sincronizzati i membri e il loro stato tra un programma Marketo e una campagna Salesforce.
* Accedi alle funzioni di reporting in Marketo e Salesforce.

## Come vengono sincronizzati un programma Marketo e una campagna Salesforce? {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

In Marketo puoi creare una mappatura uno-a-uno tra un programma e una campagna Salesforce.

![](assets/image2015-7-8-9-3a43-3a8.png)

Il **[channel](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)** e **[costo periodo](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)** in Marketo sincronizza con Salesforce come **tipo di campagna** e **costo effettivo**. Questa sincronizzazione è **unidirezionale**, da Marketo a Salesforce.

Marketo **membri del programma** e i loro **[stati di progressione](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)** sono sincronizzati con **Membri della campagna Salesforce** e **statuti dei membri della campagna**. Questo è un **sincronizzazione bidirezionale** Pertanto, qualsiasi modifica apportata in Marketo o Salesforce viene riportata in entrambi i sistemi.

>[!NOTE]
>
>Se nel programma Marketo sono presenti membri che non esistono in Salesforce, Marketo crea tali persone come lead in Salesforce.

## Quali sono i trigger/filtri relativi alle campagne? {#what-are-the-triggers-filters-related-to-campaigns}

Trigger:

* Aggiunta a Campagna SFDC
* Rimosso da Campagna SFDC
* Stato modificato nella campagna SFDC

Filtri:

* Membro della campagna SFDC

## Posso aggiungere persone Marketo alla mia campagna SFDC? {#can-i-add-marketo-people-to-my-sfdc-campaign}

Sì, utilizza [Azione di flusso Aggiungi a campagna SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md). Se questa persona non esiste in Salesforce, Marketo la creerà in Salesforce e quindi la aggiungerà alla campagna.

## Posso rimuovere membri dalla mia campagna SFDC utilizzando Marketo? {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

Sì, utilizza [Rimuovi dall’azione di flusso della campagna SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md).

## Posso cambiare lo stato di membro della campagna utilizzando Marketo? {#can-i-change-campaign-member-status-using-marketo}

Sì, utilizza [Modifica stato nell’azione di flusso della campagna SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md).

## Perché non riesco a vedere nessuna delle mie campagne Salesforce? {#why-cant-i-see-any-of-my-salesforce-campaigns}

Di seguito sono riportati alcuni elementi che è possibile verificare:

1. Assicurati che le [la sincronizzazione della campagna è abilitata](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
1. Conferma che il tuo [Utente Marketo Sync](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) è un [Utente marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) in Salesforce.

>[!NOTE]
>
>Se la campagna Salesforce e il programma Marketo mappato presentano stati di programma non compatibili, è possibile che venga visualizzato un messaggio di errore. Ti consigliamo di [corrisponde agli stati del programma prima della sincronizzazione](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

>[!MORELIKETHIS]
>
>* [Sincronizzare una campagna SFDC con un programma](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md)
>* [Informazioni sull’iscrizione al programma](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)
>* [Abilita/Disabilita sincronizzazione campagne](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)
>* [Rendi utente di Marketo Sync utente di marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)
