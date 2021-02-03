---
unique-page-id: 2953459
description: Sincr. SFDC - Sincronizzazione account - Documenti Marketo - Documentazione prodotto
title: Sincr. SFDC - Sincronizzazione account
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---


# Sincr. SFDC: Sincronizzazione account {#sfdc-sync-account-sync}

Marketo sincronizza anche le informazioni sull’account con Salesforce. Ecco alcune cose specifiche che dovreste sapere!

## In che modo vengono sincronizzate le informazioni? {#which-way-does-the-information-sync}

Solo un modo: dalla DSC a Marketo.

## Come funzionano gli aggiornamenti? {#how-do-the-updates-work}

Se si aggiorna un campo Account per un contatto in Marketo, vengono modificati i valori di tutti i contatti appartenenti a tale account in Marketo. Non viene sincronizzata con SFDC. Tuttavia, al successivo aggiornamento dell&#39;account in SFDC, le modifiche apportate sostituiranno tutte le informazioni sull&#39;account in Marketo.

## Un contatto può appartenere a più account?  {#can-a-contact-belong-to-multiple-accounts}

No. Un account può avere molti contatti, un contatto può avere un solo account.

## Posso creare account da Marketo? {#can-i-create-accounts-from-marketo}

Principalmente no. Tuttavia, se si utilizza il passaggio di flusso [Converti persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) su una persona, verrà creato un nuovo contatto, un nuovo account e una nuova opportunità.

>[!CAUTION]
>
>Questo passaggio di flusso ha un caso di utilizzo molto limitato. Se non sei sicuro, probabilmente non dovresti usarlo.

## Se una modifica in un campo account in Salesforce comporta la modifica del registro attività valore dati per ogni contatto?  {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

Principalmente sì. Tuttavia, se un account ha più di 5.000 contatti e un campo su tale account cambia in SFDC, sincronizzeremo la modifica ma non registreremo l&#39;attività per più di 5.000 contatti.
