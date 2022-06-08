---
unique-page-id: 2953467
description: Sincr. SFDC - Sincronizzazione opportunità - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Sincronizzazione opportunità
exl-id: f8acc528-c631-43f0-8899-2f3c6fdabe9e
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# Sincr. SFDC: Sincronizzazione opportunità {#sfdc-sync-opportunity-sync}

## Come vengono mantenuti sincronizzati i dettagli delle opportunità tra i due sistemi? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

La sincronizzazione è un modo: da Salesforce a Marketo. Gli aggiornamenti alle opportunità in Salesforce verranno sincronizzati con Marketo.

>[!NOTE]
>
>La [credenziali inserite in Marketo per Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) vengono utilizzati per sincronizzare i dati. Verranno inclusi solo i dati a cui tali credenziali hanno accesso.

## Posso avviare una sincronizzazione opportunità? {#can-i-initiate-an-opportunity-sync}

No, non puoi. Le modifiche apportate a qualsiasi opportunità in Salesforce verranno automaticamente sincronizzate in Marketo.

## Marketo supporta più di una valuta nell&#39;importo opportunità? {#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

No, Marketo supporta una sola valuta. L&#39;importo dell&#39;opportunità verrà sincronizzato da Salesforce ma la valuta sarà [valuta predefinita](/help/marketo/product-docs/administration/settings/set-default-location-settings-for-a-subscription.md#set-the-default-currency-settings-for-a-subscription) nel tuo abbonamento Marketo.

## In che modo Marketo associa opportunità e contatti? {#how-does-marketo-associate-opportunities-and-contacts}

Marketo associa opportunità e contatti utilizzando [Ruoli contatto opportunità](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm). Le opportunità senza l’assegnazione di ruoli di contatto verranno sincronizzate con Marketo, ma non saranno di proprietà di nessuno. Ad esempio, la persona non qualificherà il filtro Con opportunità.

## Come posso vedere tutte le opportunità di una persona? {#how-can-i-see-all-the-opportunities-of-a-person}

È possibile visualizzare un elenco di opportunità nella **Informazioni opportunità** nella scheda [Dettagli persona](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) pagina.

## Quali sono i trigger/filtri correlati alle opportunità? {#what-are-the-triggers-filters-related-to-opportunity}

Triggers:

* Aggiunto all’opportunità
* Rimosso dall’opportunità
* Opportunità aggiornata

Filtri:

* Ha opportunità
* Opportunità aggiornata/Opportunità non aggiornata
* È stato aggiunto a Opportunità/Non è stato aggiunto all&#39;opportunità
* È stato rimosso dall&#39;opportunità o non è stato rimosso dall&#39;opportunità
* Importo totale dell&#39;opzione
* Numero di oggetti
* Ricavi previsti per l&#39;Opty totale

>[!TIP]
>
>Controlla i vincoli relativi a filtri e attivatori. Ci sono un sacco di bei dettagli.
>
>Crea un nuovo campo nell&#39;oggetto opportunità in Salesforce e diventerà automaticamente un vincolo!
