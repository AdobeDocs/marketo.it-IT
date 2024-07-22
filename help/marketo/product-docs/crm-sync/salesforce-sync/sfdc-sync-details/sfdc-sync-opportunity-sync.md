---
unique-page-id: 2953467
description: Sincronizzazione SFDC - Sincronizzazione opportunità - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Sincronizzazione opportunità
exl-id: f8acc528-c631-43f0-8899-2f3c6fdabe9e
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Sincronizzazione SFDC: sincronizzazione opportunità {#sfdc-sync-opportunity-sync}

## In che modo i dettagli delle opportunità vengono mantenuti sincronizzati tra i due sistemi? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

La sincronizzazione è unidirezionale: da Salesforce a Marketo Engage. Gli aggiornamenti alle opportunità in Salesforce verranno sincronizzati con Marketo.

>[!NOTE]
>
>Le [credenziali immesse in Marketo per Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} vengono utilizzate per sincronizzare i dati. Verranno inclusi solo i dati a cui le credenziali hanno accesso.

## È possibile avviare una sincronizzazione opportunità? {#can-i-initiate-an-opportunity-sync}

No, non puoi. Le modifiche apportate a qualsiasi opportunità in Salesforce verranno sincronizzate automaticamente in Marketo.

## Marketo supporta più di una valuta nell’importo dell’opportunità? {#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

No, Marketo supporta una sola valuta. L&#39;importo dell&#39;opportunità verrà sincronizzato da Salesforce ma la valuta sarà la [valuta predefinita](/help/marketo/product-docs/administration/settings/set-default-location-settings-for-a-subscription.md#set-the-default-currency-settings-for-a-subscription){target="_blank"} nella sottoscrizione a Marketo.

## In che modo Marketo associa opportunità e contatti? {#how-does-marketo-associate-opportunities-and-contacts}

Marketo associa opportunità e contatti utilizzando [Ruoli di contatto opportunità](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm){target="_blank"}. Le opportunità senza alcun ruolo di contatto assegnato verranno sincronizzate con Marketo, ma non apparterranno a nessuno. Ad esempio, la persona non si qualifica come idonea per il filtro Ha opportunità.

## Come posso vedere tutte le opportunità di una persona? {#how-can-i-see-all-the-opportunities-of-a-person}

È possibile visualizzare un elenco di opportunità nella scheda **Informazioni opportunità** della pagina [Dettagli persona](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"}.

## Quali sono i trigger/filtri relativi all’opportunità? {#what-are-the-triggers-filters-related-to-opportunity}

Trigger:

* Aggiunto all’opportunità
* Rimosso dall’opportunità
* L’opportunità è aggiornata

Filtri:

* Ha un’opportunità
* L’opportunità è stata aggiornata/l’opportunità non è stata aggiornata
* È stato aggiunto all’opportunità/Non è stato aggiunto all’opportunità
* È stato rimosso dall’opportunità/Non è stato rimosso dall’opportunità
* Importo opzione totale
* Numero di opzioni
* Ricavi previsti opzione totale

>[!TIP]
>
>Scopri i vincoli per filtri e attivatori. Ci sono un sacco di dettagli interessanti.
>
>È sufficiente creare un nuovo campo nell’oggetto opportunità in Salesforce per trasformarlo automaticamente in un vincolo.
