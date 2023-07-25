---
unique-page-id: 2953459
description: Sincronizzazione SFDC - Sincronizzazione account - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Sincronizzazione account
exl-id: 94f7a9e5-86ea-4bb4-9d78-96a09c61321d
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---

# Sincronizzazione SFDC: sincronizzazione account {#sfdc-sync-account-sync}

Marketo sincronizza inoltre le informazioni sul tuo account con Salesforce. Ecco alcune cose specifiche che dovresti sapere!

## In che modo vengono sincronizzate le informazioni? {#which-way-does-the-information-sync}

Solo un modo: da SFDC a Marketo.

## Come funzionano gli aggiornamenti? {#how-do-the-updates-work}

Se si aggiorna un campo Account per un contatto in Marketo, vengono modificati i valori di tutti i contatti appartenenti a tale account in Marketo. Non viene sincronizzato con SFDC. Tuttavia, al prossimo aggiornamento dell&#39;account in SFDC, le modifiche sostituiranno tutte le informazioni dell&#39;account in Marketo.

## Un contatto può appartenere a più account?  {#can-a-contact-belong-to-multiple-accounts}

No. Un account può avere molti contatti, un contatto può avere un solo account.

## Posso creare account da Marketo? {#can-i-create-accounts-from-marketo}

Per lo più, no. Tuttavia, se utilizzi il [Converti persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) per una persona, creerà un nuovo contatto, un nuovo account e una nuova opportunità.

>[!CAUTION]
>
>Questo passaggio di flusso presenta un caso d’uso molto limitato. Se non sei sicuro, probabilmente non dovresti utilizzarlo.

## Una modifica in un campo account in Salesforce determina un registro attività Change Data Value per ogni contatto?  {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

Per lo più, sì. Tuttavia, se un account ha più di 5.000 contatti e un campo su tale account cambia in SFDC, la modifica verrà sincronizzata ma non verrà registrata l&#39;attività per gli oltre 5.000 contatti.
