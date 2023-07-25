---
unique-page-id: 4719283
description: Informazioni su Salesforce Sync - Marketo Docs - Documentazione del prodotto
title: Informazioni su Salesforce Sync
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 1%

---

# Informazioni su Salesforce Sync {#understanding-the-salesforce-sync}

Marketo e Salesforce vanno insieme come piselli e carote. Manteniamo sincronizzati i dati di vendita e marketing.

## Funzionamento di Sync {#how-sync-works}

Marketo si sincronizza con Salesforce tutto il giorno, ogni giorno. Ogni sincronizzazione richiede un po’ di tempo, quindi si mette in pausa per 5 minuti e si riavvia.

>[!NOTE]
>
>La prima sincronizzazione nell’abbonamento potrebbe richiedere ore o anche giorni, perché Marketo sta copiando l’intero database da Salesforce. Successivamente, ogni sincronizzazione richiede in genere secondi o minuti e sincronizza solo i dati modificati.

![](assets/sync-illustration.png)

La sincronizzazione tra Salesforce e Marketo è bidirezionale solo per lead, contatti e campagne Salesforce. In questi casi, ogni volta che apporti modifiche in Salesforce o Marketo, gli aggiornamenti si rifletteranno in entrambi i sistemi. Tutte le altre sincronizzazioni vengono effettuate solo da Salesforce a Marketo. Fai clic sui collegamenti riportati di seguito per ottenere informazioni dettagliate su ciascuno di essi.

## Cos’è sincronizzato tra Marketo e Salesforce? {#what-is-synced-between-marketo-and-salesforce}

* [Lead](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md)
* [Contatti](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)
* [Account](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md)
* [Utenti](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md)
* [Opportunità](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md)
* [Campagne Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md)
* [Oggetti personalizzati](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md)
* [Attività](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md)

>[!NOTE]
>
>Il [credenziali immesse in Marketo per Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) vengono utilizzati per sincronizzare i dati. Verranno inclusi solo i dati a cui le credenziali hanno accesso.

La sincronizzazione di Marketo con Salesforce è la più potente del suo genere al mondo. Sembra una magia; viene fatto un cambiamento e l&#39;altro sistema è presto aggiornato.
