---
unique-page-id: 2953463
description: Sincronizzazione SFDC - Sincronizzazione lead/proprietario account - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Sincronizzazione lead/proprietario account
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# Sincronizzazione SFDC: sincronizzazione lead/proprietario account {#sfdc-sync-lead-account-owner-sync}

Tecnicamente, la tabella &quot;utente&quot; verrà sincronizzata in [!DNL Salesforce], ma verrà indicata come campo Proprietario lead/account.

## Quali campi verranno sincronizzati con Marketo Engage? {#which-fields-will-sync-to-marketo-engage}

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

Utilizzare l&#39;azione di flusso [Modifica proprietario](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}.

>[!NOTE]
>
>Impossibile modificare le informazioni sul proprietario utilizzando [la pagina Dettagli persona](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"}.

## Cosa posso fare con questi dati? {#what-can-i-do-with-this-data}

Esistono molti motivi per utilizzare questi dati, ad esempio

* Invia un’e-mail personalizzata con la firma del proprietario dell’attività di vendita
* Possibilità di filtrare in base a rappresentanti di vendita specifici per scopi di marketing o per analisi dell&#39;efficacia
* Regole di assegnazione (e riassegnazione) in Marketo
* Utilizzali nelle azioni di flusso [Cambia proprietario](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}, [Sincronizza persona in SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} e [Crea attività](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}

Marketo ha sicuramente una fantastica sincronizzazione di [!DNL Salesforce]. Nessun altro lo fa così bene!
