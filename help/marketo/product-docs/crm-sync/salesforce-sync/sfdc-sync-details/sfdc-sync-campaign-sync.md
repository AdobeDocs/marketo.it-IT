---
unique-page-id: 2953469
description: Sincronizzazione SFDC - Sincronizzazione campagne - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Sincronizzazione campagna
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Sincronizzazione SFDC: Sincronizzazione campagna {#sfdc-sync-campaign-sync}

I programmi di Marketo Engage possono essere sincronizzati con le campagne Salesforce. Ecco una panoramica di come funziona.

## Perché sincronizzare i programmi Marketo con le campagne Salesforce? {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* Utilizza le potenti funzioni di un programma Marketo.
* Mantieni sincronizzati i membri e il loro stato tra un programma Marketo e una campagna Salesforce.
* Accedi alle funzioni di reporting in Marketo e Salesforce.

## Come vengono sincronizzati un programma Marketo e una campagna Salesforce? {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

In Marketo puoi creare una mappatura uno-a-uno tra un programma e una campagna Salesforce.

![](assets/image2015-7-8-9-3a43-3a8.png)

Il costo di **[channel](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}** e **[period](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md){target="_blank"}** in Marketo è sincronizzato con Salesforce come **tipo di campagna** e **costo effettivo**. Questa sincronizzazione è **unidirezionale**, da Marketo a Salesforce.

I **membri del programma** Marketo e i relativi **[stati di progressione](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md){target="_blank"}** sono sincronizzati con i **membri della campagna Salesforce** e i **stati membri della campagna**. Si tratta di una **sincronizzazione bidirezionale**, pertanto tutte le modifiche apportate in Marketo o Salesforce vengono applicate in entrambi i sistemi.

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

Sì, utilizza l&#39;azione [Aggiungi a flusso campagna SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md){target="_blank"}. Se questa persona non esiste in Salesforce, Marketo la creerà in Salesforce e quindi la aggiungerà alla campagna.

## Posso rimuovere membri dalla mia campagna SFDC utilizzando Marketo? {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

Sì, utilizza [Rimuovi dall&#39;azione di flusso della campagna SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md){target="_blank"}.

## Posso cambiare lo stato di membro della campagna utilizzando Marketo? {#can-i-change-campaign-member-status-using-marketo}

Sì, utilizza [Modifica stato nell&#39;azione di flusso della campagna SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"}.

## Perché non riesco a vedere nessuna delle mie campagne Salesforce? {#why-cant-i-see-any-of-my-salesforce-campaigns}

Di seguito sono riportati alcuni elementi che è possibile verificare:

1. Assicurarsi che la sincronizzazione della [campagna sia abilitata](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}.
1. Conferma che il tuo [utente Marketo Sync](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} è un [utente Marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"} in Salesforce.

>[!NOTE]
>
>Se la campagna Salesforce e il programma Marketo mappato presentano stati di programma non compatibili, è possibile che venga visualizzato un messaggio di errore. Ti consigliamo di [far corrispondere gli stati del programma prima della sincronizzazione](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Sincronizza una campagna SFDC con un programma](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md){target="_blank"}
>* [Informazioni sull&#39;iscrizione al programma](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md){target="_blank"}
>* [Attiva/Disattiva sincronizzazione campagne](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}
>* [Imposta utente di Marketo Sync come utente di marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"}
