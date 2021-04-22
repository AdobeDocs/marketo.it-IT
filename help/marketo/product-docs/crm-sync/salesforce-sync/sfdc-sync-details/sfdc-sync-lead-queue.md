---
unique-page-id: 7516241
description: Sincr. SFDC - Coda lead - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Coda lead
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# Sincr. SFDC: Coda lead {#sfdc-sync-lead-queue}

Marketo consente di aggiungere persone alle [code lead Salesforce](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) per facilitare la distribuzione dei lead. Ecco i dettagli.

## Come assegnare una persona a una coda in Marketo? {#how-to-assign-a-person-to-a-queue-in-marketo}

Puoi assegnare una persona a una coda lead Salesforce utilizzando una delle seguenti azioni di flusso:

* [Sincronizza persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)
* [Cambia proprietario](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)

>[!NOTE]
>
>Non è possibile creare o modificare le code in Marketo.

## Come vengono archiviate le informazioni sul proprietario del lead se la persona appartiene a una coda? {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

Se un lead è di proprietà di una coda in Salesforce, questi campi del proprietario delle vendite rimangono vuoti fino a quando il lead non viene assegnato a un proprietario.

* Nome proprietario vendite
* Cognome proprietario vendite
* Titolo proprietario vendite
* Numero di telefono del proprietario vendite
* Indirizzo e-mail proprietario vendite
