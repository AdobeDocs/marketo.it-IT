---
unique-page-id: 2953469
description: Sincronizzazione SFDC - Sincronizzazione Campagne - Documentazione Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Sincronizzazione campagna
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 1%

---

# Sincronizzazione SFDC: sincronizzazione campagna {#sfdc-sync-campaign-sync}

I programmi Marketo possono essere sincronizzati con [!DNL Salesforce] campagne. Ecco una panoramica di come funziona.

## Perché sincronizzare i programmi Marketo con [!DNL Salesforce] campagne? {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* Utilizza le potenti funzioni di un programma Marketo.
* Mantieni sincronizzati i membri e il loro stato tra un programma Marketo e una campagna [!DNL Salesforce].
* Accedi alle funzioni di reporting in Marketo e [!DNL Salesforce].

## Come vengono sincronizzati un programma Marketo e una campagna [!DNL Salesforce]? {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

In Marketo è possibile creare una mappatura uno-a-uno tra un programma e una campagna [!DNL Salesforce].

![](assets/image2015-7-8-9-3a43-3a8.png)

Il costo di **[channel](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)** e **[period](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)** in Marketo è sincronizzato con [!DNL Salesforce] come **tipo di campagna** e **costo effettivo**. Questa sincronizzazione è **unidirezionale**, da Marketo a [!DNL Salesforce].

I **membri del programma** Marketo e i relativi **[stati di progressione](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)** sono sincronizzati con i **[!DNL Salesforce]membri della campagna** e i **stati membri della campagna**. Si tratta di una **sincronizzazione bidirezionale**, pertanto tutte le modifiche apportate in Marketo o [!DNL Salesforce] vengono applicate in entrambi i sistemi.

>[!NOTE]
>
>Se nel programma Marketo sono presenti membri che non esistono in [!DNL Salesforce], Marketo crea tali persone come lead in [!DNL Salesforce].

## Quali sono i trigger/filtri relativi alle campagne? {#what-are-the-triggers-filters-related-to-campaigns}

Trigger:

* Aggiunto a SFDC Campaign
* Rimosso da SFDC Campaign
* Lo stato viene modificato in SFDC Campaign

Filtri:

* Membro di SFDC Campaign

## Posso aggiungere persone Marketo alla mia campagna SFDC? {#can-i-add-marketo-people-to-my-sfdc-campaign}

Sì, utilizza l&#39;[azione Aggiungi a flusso campagna SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md). Se questa persona non esiste in [!DNL Salesforce], Marketo la creerà in [!DNL Salesforce] e quindi la aggiungerà alla campagna.

## È possibile rimuovere membri dalla campagna SFDC utilizzando Marketo? {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

Sì, utilizza l&#39;[azione di flusso Rimuovi da SFDC Campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md){target="_blank"}.

## Posso cambiare lo stato di membro della campagna utilizzando Marketo? {#can-i-change-campaign-member-status-using-marketo}

Sì, utilizza l&#39;[azione di flusso Modifica stato in SFDC Campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"}.

## Perché non è possibile visualizzare le campagne [!DNL Salesforce]? {#why-cant-i-see-any-of-my-salesforce-campaigns}

Di seguito sono riportati alcuni elementi che è possibile verificare:

1. Assicurarsi che la sincronizzazione della [campagna sia abilitata](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
1. Conferma che il tuo [utente Marketo Sync](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) è un [utente Marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) in [!DNL Salesforce].

>[!NOTE]
>
>Se la campagna [!DNL Salesforce] e il programma Marketo mappato presentano stati di programma non compatibili, è possibile che venga visualizzato un messaggio di errore. Ti consigliamo di [far corrispondere gli stati del programma prima della sincronizzazione](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

>[!MORELIKETHIS]
>
>* [Sincronizzare una campagna SFDC con un programma](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md){target="_blank"}
>* [Informazioni sull&#39;iscrizione al programma](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md){target="_blank"}
>* [Attiva/Disattiva sincronizzazione campagne](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}
>* [Imposta utente di Marketo Sync come utente di marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"}
