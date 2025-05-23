---
description: Perché le attività di vendita e i campi attività non vengono sincronizzati con Salesforce? - Documentazione di Marketo - Documentazione del prodotto
title: Perché le attività di vendita e i campi attività non vengono sincronizzati con Salesforce?
exl-id: 5da855f2-18c6-456a-9e5d-ef4499596b3c
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Perché le attività di vendita e i campi attività non vengono sincronizzati con Salesforce? {#why-arent-my-sales-activities-and-activity-fields-syncing-to-salesforce}

**Non vedo attività di e-mail o chiamate sincronizzate con Salesforce.**

* Assicurati di essere connesso a Salesforce. Ogni utente dovrà disporre di una connessione per registrare la propria e-mail e le chiamate a Salesforce.
* Assicurati di aver configurato [Impostazioni di sincronizzazione Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}.
* Le e-mail eseguiranno una ricerca dei record in base all’ID Salesforce come ricerca principale e all’indirizzo e-mail come secondario. Puoi verificare che un record persona abbia un ID Salesforce e un indirizzo e-mail collegati nell&#39;[app Web Actions](https://toutapp.com/next#command_center){target="_blank"}.
* Le chiamate eseguiranno una ricerca record basata solo sull’ID Salesforce. Se nel record della persona in Actions non esiste alcun ID Salesforce, la chiamata di non si registra. Puoi verificare che un record persona abbia un ID Salesforce collegato nell&#39;app Web [Actions](https://toutapp.com/next#command_center){target="_blank"}.

**Non vedo campi attività nell&#39;aggiornamento Salesforce.**

Se non vedi l&#39;aggiornamento dei [campi dell&#39;attributo dell&#39;attività](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} tramite e-mail in Salesforce, ciò potrebbe essere dovuto a restrizioni all&#39;accessibilità dei campi del tuo team. La sicurezza a livello di campo di Salesforce consente agli amministratori di Salesforce di limitare le informazioni visualizzabili e modificabili dagli utenti. Se gli utenti di Actions non hanno accesso alla visualizzazione e alla modifica di questi campi, la sincronizzazione delle attività di Actions non riuscirà ad aggiornare questi campi.

* Rivolgiti al tuo amministratore Salesforce per assicurarti che queste impostazioni di sicurezza non interferiscano con i campi dell&#39;[Attività Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} delle azioni.
* Se sei un amministratore di Salesforce, puoi visualizzare l’accessibilità dei campi nella scheda Controlli di sicurezza. Gli oggetti principali con cui interagiranno le azioni sono: lead, contatti, account, opportunità e attività.

>[!NOTE]
>
>I campi associati agli oggetti Lead, Contact, Account e Opportunity verranno installati con il pacchetto Sales Insight Salesforce. I campi associati al tipo di record [Attività/Attività dovranno essere creati](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} da un amministratore Salesforce.
