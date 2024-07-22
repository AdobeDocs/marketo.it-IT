---
unique-page-id: 3571836
description: Sincronizzazione Microsoft Dynamics - Sincronizzazione account - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione Microsoft Dynamics - Sincronizzazione account
exl-id: 86249d33-60dd-47e1-a7c8-3996c9444084
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Sincronizzazione Microsoft Dynamics: sincronizzazione account {#microsoft-dynamics-sync-account-sync}

Lo sapevi che il Marketo Engage sincronizza l’intero database con Dynamics? Si sincronizza, poi aspetta 5 minuti e poi si sincronizza di nuovo, tutto il giorno, ogni giorno. Di seguito sono riportati alcuni dettagli su come Marketo tratta gli account Dynamics in modo specifico.

## In che modo vengono sincronizzate le informazioni? {#which-way-does-the-information-sync}

Solo un modo: da Dynamics a Marketo.

## Come funzionano gli aggiornamenti? {#how-do-the-updates-work}

Se si aggiorna un campo Account per un contatto in Marketo, vengono modificati i valori di tutti i contatti appartenenti a tale account in Marketo. Non viene sincronizzato con Dynamics. Tuttavia, al successivo aggiornamento dell’account in Dynamics, le modifiche sostituiranno tutte le informazioni dell’account in Marketo.

## Posso creare un account con Marketo? {#can-i-create-an-account-using-marketo}

No. Marketo non può creare account in Dynamics.

## Quali campi verranno sincronizzati con Marketo? {#which-fields-will-sync-to-marketo}

È possibile [selezionare i campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} durante l&#39;installazione. Marketo sincronizzerà solo i campi a cui l’utente di Dynamics Sync ha accesso.

## Una modifica in un campo account in Dynamics determina un registro attività Modifica valore dati per ogni contatto?  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

Per lo più, sì. Tuttavia, se un account ha più di 5.000 contatti e un campo su tale account cambia in Dynamics, la modifica verrà sincronizzata ma non verrà registrata l’attività per gli oltre 5.000 contatti.
