---
unique-page-id: 2953459
description: Sincr. SFDC - Sincronizzazione account - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Sincronizzazione account
exl-id: 94f7a9e5-86ea-4bb4-9d78-96a09c61321d
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---

# Sincr. SFDC: Sincronizzazione account {#sfdc-sync-account-sync}

Marketo sincronizza inoltre le informazioni sul tuo account con Salesforce. Ecco alcune cose specifiche che dovreste sapere!

## In che modo le informazioni vengono sincronizzate? {#which-way-does-the-information-sync}

Solo un modo: da SFDC a Marketo.

## Come funzionano gli aggiornamenti? {#how-do-the-updates-work}

Se si aggiorna un campo Account per un contatto in Marketo, vengono modificati i valori di tutti i contatti appartenenti a tale account in Marketo. Non si sincronizza con SFDC. Tuttavia, la prossima volta che l’account viene aggiornato in SFDC, le modifiche sovrascriveranno tutte le informazioni sull’account in Marketo.

## Un contatto può appartenere a più account?  {#can-a-contact-belong-to-multiple-accounts}

No. Un account può avere molti contatti, un contatto può avere un solo account.

## Posso creare account da Marketo? {#can-i-create-accounts-from-marketo}

Principalmente no. Tuttavia, se utilizzi il [Converti persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) passaggio di flusso su una persona, creerà un nuovo contatto, un nuovo account e una nuova opportunità.

>[!CAUTION]
>
>Questa fase del flusso ha un caso d’uso molto limitato. Se non sei sicuro, probabilmente non dovresti usarlo.

## Una modifica in un campo account in Salesforce determina un registro attività Modifica valore dati per ogni contatto?  {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

Principalmente sì. Tuttavia, se un account ha più di 5.000 contatti e un campo su tale account cambia in SFDC, sincronizziamo la modifica ma non registriamo l&#39;attività per più di 5.000 contatti.
