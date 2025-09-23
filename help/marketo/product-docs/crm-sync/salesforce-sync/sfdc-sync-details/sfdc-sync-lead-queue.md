---
unique-page-id: 7516241
description: Sincronizzazione SFDC - Coda lead - Documentazione Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Coda lead
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '130'
ht-degree: 3%

---

# Sincronizzazione SFDC: coda lead {#sfdc-sync-lead-queue}

Marketo consente di aggiungere persone alle [[!DNL Salesforce] code lead](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) per facilitare la distribuzione dei lead. Ecco i dettagli.

## Come assegnare una persona a una coda in Marketo? {#how-to-assign-a-person-to-a-queue-in-marketo}

È possibile assegnare una persona a una coda di lead [!DNL Salesforce] utilizzando una delle azioni di flusso seguenti:

* [Sincronizza persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}
* [Cambia proprietario](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}

>[!NOTE]
>
>Non è possibile creare o modificare code in Marketo.

## Come vengono memorizzate le informazioni sul proprietario del lead se la persona appartiene a una coda? {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

Se un lead appartiene a una coda in [!DNL Salesforce], questi campi del proprietario delle vendite rimangono vuoti fino a quando il lead non viene assegnato a un proprietario.

* Nome proprietario vendite
* Cognome Proprietario vendita
* Titolo proprietario vendite
* Numero di telefono del proprietario della vendita
* Indirizzo e-mail del proprietario della vendita
