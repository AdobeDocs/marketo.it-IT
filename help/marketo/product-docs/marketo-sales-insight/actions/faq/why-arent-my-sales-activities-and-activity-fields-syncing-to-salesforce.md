---
description: Perché le attività di vendita e i campi attività non vengono sincronizzati con Salesforce? - Documentazione di Marketo - Documentazione del prodotto
title: Perché le attività di vendita e i campi attività non vengono sincronizzati con Salesforce?
exl-id: 0836876d-1b89-4464-a841-81320a6e45fd
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# Perché le attività di vendita e i campi attività non vengono sincronizzati con Salesforce? {#why-arent-my-sales-activities-and-activity-fields-syncing-to-salesforce}

**Non vedo attività di e-mail o chiamate sincronizzate con Salesforce.**

* Assicurati di essere connesso a Salesforce. Ogni utente dovrà disporre di una connessione per registrare la propria e-mail e le chiamate a Salesforce.
* Assicurati di aver configurato [Impostazioni di sincronizzazione Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}.
* Le e-mail eseguiranno una ricerca dei record in base all’ID Salesforce come ricerca principale e all’indirizzo e-mail come secondario. Puoi confermare che a un record di persona sono collegati un ID Salesforce e un indirizzo e-mail nella [App web Actions](https://toutapp.com/next#command_center){target="_blank"}.
* Le chiamate eseguiranno una ricerca record basata solo sull’ID Salesforce. Se nel record della persona in Actions non esiste alcun ID Salesforce, la chiamata di non si registra. Puoi confermare che a un record di persona è collegato un ID Salesforce in [App web Actions](https://toutapp.com/next#command_center){target="_blank"}.

**Non vedo i campi di attività nell’aggiornamento di Salesforce.**

Se non visualizzi l’e-mail [campi attributo attività](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} in Salesforce, potrebbe essere dovuto a restrizioni sull’accessibilità dei campi del tuo team. La sicurezza a livello di campo di Salesforce consente agli amministratori di Salesforce di limitare le informazioni visualizzabili e modificabili dagli utenti. Se gli utenti di Actions non hanno accesso alla visualizzazione e alla modifica di questi campi, la sincronizzazione delle attività di Actions non riuscirà ad aggiornare questi campi.

* Rivolgiti al tuo amministratore Salesforce per assicurarti che queste impostazioni di sicurezza non interferiscano con [Campi delle attività di Actions Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}.
* Se sei un amministratore di Salesforce, puoi visualizzare l’accessibilità dei campi nella scheda Controlli di sicurezza. Gli oggetti principali con cui interagiranno le azioni sono: lead, contatti, account, opportunità e attività.

>[!NOTE]
>
>I campi associati agli oggetti Lead, Contact, Account e Opportunity verranno installati con il pacchetto Sales Insight Salesforce. Campi associati al [È necessario creare il tipo di record Attività](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} da un amministratore Salesforce.
