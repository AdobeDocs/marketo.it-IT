---
unique-page-id: 4719283
description: Informazioni su Salesforce Sync - Marketo Docs - Documentazione del prodotto
title: Informazioni sulla sincronizzazione Salesforce
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 2%

---

# Informazioni sulla sincronizzazione di [!DNL Salesforce] {#understanding-the-salesforce-sync}

Marketo Engage e Salesforce vanno insieme come piselli e carote. Manteniamo sincronizzati i dati di vendita e marketing.

## Funzionamento di Sync {#how-sync-works}

Marketo esegue la sincronizzazione con [!DNL Salesforce] tutto il giorno, ogni giorno. Ogni sincronizzazione richiede un po’ di tempo, quindi si mette in pausa per 5 minuti e si riavvia.

>[!NOTE]
>
>La prima sincronizzazione della sottoscrizione potrebbe richiedere ore o anche giorni perché Marketo sta copiando l&#39;intero database da [!DNL Salesforce]. Successivamente, ogni sincronizzazione richiede in genere secondi o minuti e sincronizza solo i dati modificati.

![](assets/sync-illustration.png)

La sincronizzazione tra [!DNL Salesforce] e Marketo è bidirezionale solo per lead, contatti e [!DNL Salesforce] campagne. In questi casi, ogni volta che si apportano modifiche in [!DNL Salesforce] o Marketo, gli aggiornamenti verranno applicati a entrambi i sistemi. Tutte le altre sincronizzazioni sono solo da [!DNL Salesforce] a Marketo. Fai clic sui collegamenti riportati di seguito per ottenere informazioni dettagliate su ciascuno di essi.

## Cos&#39;è sincronizzato tra Marketo e [!DNL Salesforce]? {#what-is-synced-between-marketo-and-salesforce}

* [Lead](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md){target="_blank"}
* [Contatti](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md){target="_blank"}
* [Account](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md){target="_blank"}
* [Utenti](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md){target="_blank"}
* [Opportunità](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md){target="_blank"}
* [Campagne Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}
* [Oggetti personalizzati](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md){target="_blank"}
* [Attività](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md){target="_blank"}

>[!NOTE]
>
>Le [credenziali immesse in Marketo per Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} vengono utilizzate per sincronizzare i dati. Verranno inclusi solo i dati a cui le credenziali hanno accesso.

La sincronizzazione di Marketo con [!DNL Salesforce] è la più potente del suo genere al mondo. Sembra una magia; viene fatto un cambiamento e l&#39;altro sistema è presto aggiornato.
