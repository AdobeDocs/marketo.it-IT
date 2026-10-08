---
unique-page-id: 7516241
description: Scopri come assegnare persone alle code di lead di Salesforce da Marketo. Utilizzare le azioni di flusso Sincronizza persona in SFDC o Modifica proprietario per la distribuzione dei lead.
title: Sincronizzazione SFDC - Coda lead
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
feature: Salesforce Integration
TQID: 'https://experienceleague.adobe.com/aUrT7qSMy65t3K07O176nt-Bzjm9urgnXKAkZgs1-cs'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: edcca97f-2314-445f-9a79-3ac30a2a9c27
    internal-label: Salesforce integration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 6%
---
# Sincronizzazione SFDC: coda lead {#sfdc-sync-lead-queue}

Marketo consente di aggiungere persone alle [[!DNL Salesforce] code lead](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) per facilitare la distribuzione dei lead. Ecco i dettagli.

## Come assegnare una persona a una coda in Marketo? {#how-to-assign-a-person-to-a-queue-in-marketo}

È possibile assegnare una persona a una coda di lead [!DNL Salesforce] utilizzando una delle azioni di flusso seguenti:

* [Sincronizzare persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}
* [Modificare proprietario](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}

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
