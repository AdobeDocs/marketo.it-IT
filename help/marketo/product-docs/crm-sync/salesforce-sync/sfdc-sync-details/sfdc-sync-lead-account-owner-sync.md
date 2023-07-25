---
unique-page-id: 2953463
description: Sincronizzazione SFDC - Sincronizzazione lead/proprietario account - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Sincronizzazione lead/proprietario account
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Sincronizzazione SFDC: sincronizzazione lead/proprietario account {#sfdc-sync-lead-account-owner-sync}

Tecnicamente, queste stanno sincronizzando la tabella &quot;utente&quot; in Salesforce, ma questa viene definita come campi Proprietario lead/account.

## Quali campi verranno sincronizzati con Marketo? {#which-fields-will-sync-to-marketo}

Per ogni persona sincronizzata con Marketo, vengono sincronizzati anche i seguenti campi del proprietario:

* Nome proprietario vendite
* Cognome Proprietario vendita
* Titolo proprietario vendite
* Numero di telefono del proprietario della vendita
* Indirizzo e-mail del proprietario della vendita

Per ogni contatto, vengono sincronizzati i cinque campi del proprietario del lead e i seguenti campi del proprietario dell’account:

* Nome proprietario account
* Cognome del proprietario dell’account
* Indirizzo e-mail del proprietario dell’account

## Posso cambiare il proprietario del lead in Marketo? {#can-i-change-the-lead-owner-in-marketo}

Assolutamente, utilizza solo [Cambia proprietario](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md) azione di flusso.

>[!NOTE]
>
>Non è possibile modificare le informazioni relative al proprietario utilizzando [Utilizzo della pagina Dettagli persona](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

## Cosa posso fare con questi dati? {#what-can-i-do-with-this-data}

Esistono molti motivi per utilizzare questi dati, ad esempio

* Invia un’e-mail personalizzata con la firma del proprietario dell’attività di vendita
* Possibilità di filtrare in base a rappresentanti di vendita specifici per scopi di marketing o per analisi dell&#39;efficacia
* Regole di assegnazione (e riassegnazione) in Marketo
* Utilizzali in [Cambia proprietario](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md), [Sincronizza persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md), e [Crea attività](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) azioni di flusso

Marketo ha sicuramente una fantastica sincronizzazione Salesforce. Nessun altro lo fa così bene!
