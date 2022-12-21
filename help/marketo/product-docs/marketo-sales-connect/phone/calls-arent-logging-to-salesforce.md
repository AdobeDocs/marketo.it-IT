---
unique-page-id: 14352435
description: Le chiamate non effettuano la registrazione a Salesforce - Documenti Marketo - Documentazione del prodotto
title: Le chiamate non vengono registrate in Salesforce
exl-id: 99528c1a-7398-442b-81d1-9b5908e35e2f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '136'
ht-degree: 0%

---

# Le chiamate non vengono registrate in Salesforce {#calls-arent-logging-to-salesforce}

Se desideri che le tue chiamate dal telefono di vendita siano automaticamente registrate a Salesforce, assicurati che sia presente quanto segue.

Sarà necessario che il tuo account di vendita Connect sia collegato al tuo [Conto Salesforce](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md) tramite la connessione API.

Se si chiama da [applicazione web](https://toutapp.com/login), sarà necessario salvare un ID Salesforce in quel contatto. [Fai clic qui](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/import-a-salesforce-id-into-sales-connect.md) per vedere come è possibile assicurarsi che tutti i contatti di vendita Connect siano associati a un ID Salesforce.

>[!NOTE]
>
>Assicurati di avere &quot;Call&quot; nella lista di selezione dei tipi di attività per ottenere rapporti precisi e semplici in Salesforce.

Una volta che questo è attivo, vedrai un&#39;attività creata nella sezione Cronologia attività di Salesforce.
