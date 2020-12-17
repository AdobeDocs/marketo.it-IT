---
unique-page-id: 2953463
description: Sincr. SFDC - Sincr. lead/proprietario account - Documenti Marketo - Documentazione prodotto
title: Sincr. SFDC - Sincronizzazione lead/proprietario account
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---


# Sincr. SFDC: Sincronizzazione proprietario lead/account {#sfdc-sync-lead-account-owner-sync}

tecnicamente sincronizzando la tabella &quot;utente&quot; in Salesforce, tuttavia vi faremo riferimento come campi Lead/Proprietario account.

## Quali campi verranno sincronizzati con Marketo? {#which-fields-will-sync-to-marketo}

Per ogni persona sincronizzata con Marketo, sincronizziamo anche i seguenti campi proprietari:

* Nome proprietario vendita
* Cognome proprietario vendita
* Titolo proprietario vendita
* Numero di telefono proprietario vendita
* Indirizzo e-mail proprietario vendita

Per ogni contatto, sincronizziamo i cinque campi del proprietario del lead indicati sopra e i seguenti campi del proprietario dell’account:

* Nome proprietario account
* Cognome proprietario account
* Indirizzo e-mail proprietario account

## Posso cambiare il proprietario del lead in Marketo? {#can-i-change-the-lead-owner-in-marketo}

Assolutamente, basta utilizzare l&#39;azione di flusso [Modifica proprietario](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md).

>[!NOTE]
>
>Non è possibile modificare le informazioni sul proprietario utilizzando la [Pagina di dettaglio persona](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

## Cosa posso fare con questi dati? {#what-can-i-do-with-this-data}

Ci sono molti motivi per utilizzare questi dati, come

* Inviare un&#39;e-mail personalizzata con firma dal proprietario della vendita
* Filtra su agenti di vendita specifici per il marketing o anche per l&#39;analisi dell&#39;efficacia
* Regole di assegnazione (e riassegnazione) in Marketo
* Utilizzateli nelle azioni di flusso [Cambia proprietario](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md), [Sincronizza persona con SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) e [Crea attività](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)

Marketo ha sicuramente un&#39;incredibile sincronizzazione Salesforce. Nessun altro lo fa così bene!
