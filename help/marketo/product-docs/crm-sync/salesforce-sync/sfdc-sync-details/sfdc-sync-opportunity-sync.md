---
unique-page-id: 2953467
description: Sincr. SFDC - Opportunità di sincronizzazione - Documenti Marketo - Documentazione del prodotto
title: Sincr. SFDC - Sincronizzazione opportunità
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---


# Sincr. SFDC: Sincronizzazione opportunità {#sfdc-sync-opportunity-sync}

## Come vengono mantenuti sincronizzati i dettagli delle opportunità tra i due sistemi? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

La sincronizzazione è unidirezionale: da Salesforce a Marketo. Gli aggiornamenti delle opportunità in Salesforce verranno sincronizzati su Marketo.

>[!NOTE]
>
>Le [credenziali immesse in Marketo per Salesforce](../../../../product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) vengono utilizzate per sincronizzare i dati. Saranno inclusi solo i dati a cui tali credenziali hanno accesso.

## Posso avviare una sincronizzazione delle opportunità? {#can-i-initiate-an-opportunity-sync}

No, non puoi. Le modifiche apportate a qualsiasi opportunità in Salesforce verranno automaticamente sincronizzate su Marketo.

## Marketo supporta più di una valuta nell&#39;importo opportunità? {#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

No, Marketo supporta una sola valuta. L&#39;importo dell&#39;opportunità verrà sincronizzato da Salesforce, ma la valuta sarà la valuta [](https://docs.marketo.com/display/DOCS/Set+Default+Location+Settings+for+a+Subscription#SetDefaultLocationSettingsforaSubscription-SettheDefaultCurrencySettingsforaSubscription) predefinita nell&#39;abbonamento a Marketo.

## In che modo Marketo associa opportunità e contatti? {#how-does-marketo-associate-opportunities-and-contacts}

Marketo associa opportunità e contatti tramite Ruoli [di contatto](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm)opportunità. Le opportunità senza i ruoli di contatto assegnati verranno sincronizzate su Marketo, ma non appartengono a nessuno. Ad esempio, la persona non sarà qualificata con il filtro Con opportunità.

## Come posso vedere tutte le opportunità di una persona? {#how-can-i-see-all-the-opportunities-of-a-person}

Potete visualizzare un elenco delle opportunità nella scheda Informazioni **** opportunità nella pagina Dettagli [](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) persona.

## Quali sono i trigger/filtri correlati alle opportunità? {#what-are-the-triggers-filters-related-to-opportunity}

Triggers:

* Aggiunto all&#39;opportunità
* Rimosso dall&#39;opportunità
* Opportunità aggiornata

Filtri:

* Con opportunità
* Opportunità aggiornata/Opportunità non aggiornata
* È stato aggiunto all&#39;opportunità/Non è stato aggiunto all&#39;opportunità
* È stato rimosso dall&#39;opportunità/Non è stato rimosso dall&#39;opportunità
* Importo totale delle opzioni
* Numero di oggetti
* Totale ricavi previsti dell&#39;opzione

>[!TIP]
>
>Controlla i vincoli relativi a filtri e attivatori. Ci sono tanti dettagli interessanti.
>
>Crea un nuovo campo nell&#39;oggetto opportunità in Salesforce e diventerà automaticamente un vincolo!

Marketo ha la migliore sincronizzazione Salesforce al mondo!