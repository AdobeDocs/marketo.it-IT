---
unique-page-id: 7516241
description: Sincr. SFDC - Coda lead - Documenti Marketo - Documentazione prodotto
title: Sincr. SFDC - Coda lead
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# Sincr. SFDC: Coda lead {#sfdc-sync-lead-queue}

Marketo consente di aggiungere persone alle code [lead di](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) Salesforce per facilitare la distribuzione dei lead. Ecco i dettagli.

>[!NOTE]
>
>**FYI**
>
>Marketo sta standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che nell&#39;abbonamento siano presenti lead/lead e persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

## Come assegnare una persona a una coda in Marketo? {#how-to-assign-a-person-to-a-queue-in-marketo}

Puoi assegnare una persona a una coda di lead Salesforce tramite una delle seguenti azioni di flusso:

* [Sincronizza persona con SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)
* [Cambia proprietario](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)

>[!NOTE]
>
>Non puoi creare o modificare le code in Marketo.

## Come vengono memorizzate le informazioni relative al proprietario del lead se la persona appartiene a una coda? {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

Se un lead è di proprietà di una coda in Salesforce, questi campi del proprietario delle vendite rimangono vuoti finché il lead non viene assegnato a un proprietario.

* Nome proprietario vendita
* Cognome proprietario vendita
* Titolo proprietario vendita
* Numero di telefono proprietario vendita
* Indirizzo e-mail proprietario vendita

