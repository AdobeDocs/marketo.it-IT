---
unique-page-id: 2953469
description: Sincr. SFDC -Campaign Sync - Marketo Docs - Documentazione prodotto
title: Sincr. SFDC - Sincronizzazione campagna
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---


# Sincr. SFDC: Sincronizzazione campagna {#sfdc-sync-campaign-sync}

I programmi Marketo possono essere sincronizzati con le campagne Salesforce. Di seguito viene fornita una panoramica di come funziona.

## Perché dovrei sincronizzare i programmi Marketo con le campagne Salesforce? {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* Utilizza le potenti funzionalità di un programma Marketo.
* Mantieni i membri e il loro stato sincronizzati tra un programma Marketo e una campagna Salesforce.
* Toccate le funzioni di reporting in Marketo e Salesforce.

## Come vengono sincronizzati un programma Marketo e una campagna Salesforce? {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

In Marketo, puoi creare una mappatura uno-a-uno tra un programma e una campagna Salesforce.

![](assets/image2015-7-8-9-3a43-3a8.png)

Il costo [di](../../../../product-docs/administration/tags/create-a-program-channel.md) periodo ** **canale [](../../../../product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)** e ** in Marketo sincronizza con Salesforce come tipo **di** campagna e costo **** effettivo. Questa sincronizzazione è **unidirezionale**, da Marketo a Salesforce.

I membri **del** programma Marketo e i relativi stati di [avanzamento **** sono sincronizzati con i membri](../../../../product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)della campagna **Salesforce** e gli stati **membri della** campagna. Si tratta di una **** sincronizzazione **bidirezionale**, pertanto qualsiasi modifica apportata in Marketo o Salesforce si riflette in entrambi i sistemi.

>[!NOTE]
>
>Se nel programma Marketo sono presenti membri che non esistono in Salesforce, Marketo li crea come lead in Salesforce.

## Quali sono i trigger/filtri correlati alle campagne? {#what-are-the-triggers-filters-related-to-campaigns}

Triggers:

* Aggiunta alla campagna SFDC
* Rimosso dalla campagna SFDC
* Lo stato viene modificato nella campagna SFDC

Filtri:

* Membro della campagna SFDC

## Posso aggiungere Marketo People alla mia campagna SFDC? {#can-i-add-marketo-people-to-my-sfdc-campaign}

Sì, utilizza l’azione [di flusso della campagna](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md)Aggiungi a SFDC. Se questa persona non esiste in Salesforce, Marketo la creerà in Salesforce e quindi lo aggiungerà alla campagna.

## È possibile rimuovere i membri dalla campagna SFDC utilizzando Marketo? {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

Sì, utilizza l&#39;azione [](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md)Rimuovi da campagna SFDC.

## Posso cambiare lo stato dei membri della campagna utilizzando Marketo? {#can-i-change-campaign-member-status-using-marketo}

Sì, utilizza [Modifica stato nell&#39;azione](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md)di flusso della campagna SFDC.

## Perché non riesco a vedere nessuna delle mie campagne Salesforce? {#why-cant-i-see-any-of-my-salesforce-campaigns}

Di seguito sono riportati alcuni elementi che è possibile controllare:

1. Accertatevi che la sincronizzazione della [campagna sia abilitata](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
1. Verifica che [Marketo Sync User](../../../../product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) sia un utente [](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) Marketing in Salesforce.

>[!NOTE]
>
>Se la tua campagna Salesforce e il programma Marketo mappato hanno stati di programma incompatibili, potresti ricevere un messaggio di errore. Prima della sincronizzazione [è consigliabile](sfdc-errors/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md)corrispondere agli stati del programma.

>[!NOTE]
>
>**Articoli correlati**
>
>* [Sincronizzazione di una campagna SFDC con un programma](../../../../product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md)
>* [Informazioni sull&#39;iscrizione al programma](../../../../product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)
>* [Attiva/Disattiva sincronizzazione campagna](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)
>* [Come rendere Marketo Sync User un Marketing User](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)

>



