---
unique-page-id: 4719283
description: Informazioni sulla sincronizzazione di Salesforce - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni sulla sincronizzazione di Salesforce
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# Informazioni sulla sincronizzazione di Salesforce {#understanding-the-salesforce-sync}

Marketo e Salesforce si riuniscono come piselli e carote. Manteniamo sincronizzati i dati di vendita e marketing.

## Funzionamento della sincronizzazione {#how-sync-works}

Marketo sincronizza con Salesforce tutto il giorno, ogni giorno. Ogni sincronizzazione richiede un po&#39; di tempo e poi si mette in pausa per 5 minuti, quindi si riavvia.

>[!NOTE]
>
>La prima sincronizzazione dell’abbonamento potrebbe richiedere ore o persino giorni perché Marketo sta copiando l’intero database da Salesforce. In seguito, ogni sincronizzazione richiede in genere secondi o minuti e sincronizza solo i dati che sono cambiati.

![](assets/sync-illustration.png)

La sincronizzazione tra Salesforce e Marketo è bidirezionale solo per lead, contatti e campagne Salesforce. In questi casi, ogni volta che apporti modifiche in Salesforce o Marketo, gli aggiornamenti verranno rispecchiati in entrambi i sistemi. Tutte le altre sincronizzazioni sono solo da Salesforce a Marketo. Fai clic sui link qui sotto per i dettagli su ciascuno.

## Cosa viene sincronizzato tra Marketo e Salesforce? {#what-is-synced-between-marketo-and-salesforce}

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
>Le [credenziali immesse in Marketo per Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) vengono utilizzate per sincronizzare i dati. Verranno inclusi solo i dati a cui tali credenziali hanno accesso.

La sincronizzazione Marketo con Salesforce è la più potente del suo genere al mondo. Sembra magia; viene apportata una modifica e l&#39;altro sistema è presto aggiornato.
