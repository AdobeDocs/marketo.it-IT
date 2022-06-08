---
unique-page-id: 2953463
description: Sincr. SFDC - Sincronizzazione lead/proprietario account - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Sincronizzazione lead/account proprietario
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Sincr. SFDC: Sincronizzazione proprietario lead/account {#sfdc-sync-lead-account-owner-sync}

Questi stanno tecnicamente sincronizzando la tabella &quot;utente&quot; in Salesforce, ma vi faremo riferimento come campi Lead/Proprietario account.

## Quali campi verranno sincronizzati con Marketo? {#which-fields-will-sync-to-marketo}

Per ogni persona sincronizzata con Marketo, sincronizziamo anche i seguenti campi del proprietario:

* Nome proprietario vendite
* Cognome proprietario vendite
* Titolo proprietario vendite
* Numero di telefono del proprietario vendite
* Indirizzo e-mail proprietario vendite

Per ogni contatto, sincronizziamo i cinque campi del proprietario del lead indicati sopra e i seguenti campi del proprietario dell’account:

* Nome proprietario account
* Cognome proprietario account
* Indirizzo e-mail proprietario account

## Posso cambiare il proprietario del lead in Marketo? {#can-i-change-the-lead-owner-in-marketo}

Assolutamente, utilizza semplicemente il [Cambia proprietario](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md) azione di flusso.

>[!NOTE]
>
>Non è possibile modificare le informazioni sul proprietario utilizzando [Utilizzo della pagina Dettagli persona](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

## Cosa posso fare con questi dati? {#what-can-i-do-with-this-data}

Ci sono molti motivi per utilizzare questi dati, come

* Invia un’e-mail personalizzata con firma dal proprietario del venditore
* Filtrare su agenti di vendita specifici per il marketing o anche per analizzare l&#39;efficacia
* Regole di assegnazione (e riassegnazione) in Marketo
* Utilizzali nel [Cambia proprietario](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md), [Sincronizza persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)e [Crea attività](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) azioni di flusso

Marketo ha sicuramente una fantastica sincronizzazione Salesforce. Nessun altro lo fa così bene!
