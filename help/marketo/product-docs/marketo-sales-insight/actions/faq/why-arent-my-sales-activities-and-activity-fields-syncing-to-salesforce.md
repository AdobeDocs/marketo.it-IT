---
description: Perché le attività di vendita e i campi attività non vengono sincronizzati con Salesforce? - Documenti Marketo - Documentazione del prodotto
title: Perché le attività di vendita e i campi attività non vengono sincronizzati con Salesforce?
exl-id: 5da855f2-18c6-456a-9e5d-ef4499596b3c
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 7%

---

# Perché le attività di vendita e i campi attività non vengono sincronizzati con Salesforce? {#why-arent-my-sales-activities-and-activity-fields-syncing-to-salesforce}

**Non vedo attività di e-mail o chiamate sincronizzate con Salesforce.**

* Assicurati di essere connesso a Salesforce. Ogni utente dovrà disporre di una connessione per registrare le proprie chiamate e-mail a Salesforce.
* Assicurarsi di aver configurato [Impostazioni di sincronizzazione Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}.
* Le e-mail eseguiranno una ricerca record basata su Salesforce ID come ricerca principale e l’indirizzo e-mail come secondario. Puoi verificare che un record persona abbia un ID Salesforce e un indirizzo e-mail collegati nell&#39;[app Web Actions](https://toutapp.com/next#command_center){target="_blank"}.
* Le chiamate eseguiranno una ricerca record basata solo su Salesforce ID. Se nel record della persona in Actions non esiste alcun ID Salesforce, la chiamata di non si registra. Puoi verificare che un record persona abbia un Salesforce ID collegato nell&#39;app Web [Actions](https://toutapp.com/next#command_center){target="_blank"}.

**Non vedo campi attività in Salesforce Update.**

Se non vedi l&#39;aggiornamento dei [campi dell&#39;attributo dell&#39;attività](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} tramite e-mail in Salesforce, ciò potrebbe essere dovuto a restrizioni all&#39;accessibilità dei campi del tuo team. La sicurezza a livello di campo di Salesforce consente agli amministratori di Salesforce di limitare le informazioni visualizzabili e modificabili dagli utenti. Se gli utenti di Actions non hanno accesso alla visualizzazione e alla modifica di questi campi, la sincronizzazione delle attività di Actions non riuscirà ad aggiornare questi campi.

* Rivolgiti al tuo amministratore di Salesforce per assicurarti che queste impostazioni di sicurezza non interferiscano con i campi [Attività Salesforce per azioni](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}.
* Se sei un amministratore di Salesforce, puoi visualizzare l’accessibilità dei campi nella scheda Controlli di sicurezza. Gli oggetti principali con cui interagiranno le azioni sono: lead, contatti, account, opportunità e attività.

>[!NOTE]
>
>I campi associati agli oggetti Lead, Contact, Account e Opportunity verranno installati con il pacchetto Sales Insight Salesforce. I campi associati al tipo di record [Attività/Attività dovranno essere creati](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} da un amministratore Salesforce.
