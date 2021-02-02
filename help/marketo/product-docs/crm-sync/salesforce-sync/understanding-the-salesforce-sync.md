---
unique-page-id: 4719283
description: Informazioni sulla sincronizzazione di Salesforce - Marketo Docs - Documentazione del prodotto
title: Informazioni sulla sincronizzazione di Salesforce
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# Informazioni sulla sincronizzazione di Salesforce {#understanding-the-salesforce-sync}

Marketo e Salesforce si riuniscono come piselli e carote. Manteniamo sincronizzati i dati di vendita e marketing.

## Come funziona la sincronizzazione {#how-sync-works}

Marketo si sincronizza con Salesforce tutto il giorno, ogni giorno. Ogni sincronizzazione richiede un po&#39; di tempo, quindi viene messa in pausa per 5 minuti, quindi riavvia.

>[!NOTE]
>
>La prima sincronizzazione dell&#39;abbonamento potrebbe richiedere ore o anche giorni perché Marketo sta copiando l&#39;intero database da Salesforce. In seguito, ogni sincronizzazione richiede in genere secondi o minuti e sincronizza solo i dati modificati.

![](assets/sync-illustration.png)

La sincronizzazione tra Salesforce e Marketo è bidirezionale solo per lead, contatti e campagne Salesforce. In questi casi, ogni volta che si apportano modifiche in Salesforce o in Marketo, gli aggiornamenti si rifletteranno su entrambi i sistemi. Tutte le altre sincronizzazioni vanno da Salesforce a Marketo. Fate clic sui collegamenti di seguito per i dettagli relativi a ciascuno.

## Che cosa è sincronizzato tra Marketo e Salesforce? {#what-is-synced-between-marketo-and-salesforce}

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
>Le [credenziali immesse in Marketo per Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) vengono utilizzate per la sincronizzazione dei dati. Saranno inclusi solo i dati a cui tali credenziali hanno accesso.

La sincronizzazione di Marketo con Salesforce è la più potente del suo genere al mondo. Sembra magia. viene apportata una modifica e l&#39;altro sistema sarà presto aggiornato.
