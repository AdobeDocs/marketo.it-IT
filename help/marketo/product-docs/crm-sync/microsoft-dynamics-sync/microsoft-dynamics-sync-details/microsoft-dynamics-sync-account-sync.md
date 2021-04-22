---
unique-page-id: 3571836
description: Microsoft Dynamics Sync - Sincronizzazione account - Documenti Marketo - Documentazione del prodotto
title: Microsoft Dynamics Sync - Sincronizzazione account
exl-id: 86249d33-60dd-47e1-a7c8-3996c9444084
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Sincronizzazione Microsoft Dynamics: Sincronizzazione account {#microsoft-dynamics-sync-account-sync}

Lo sapevi che Marketo sincronizza l’intero database con Dynamics? Si sincronizza, poi aspetta 5 minuti e poi sincronizza di nuovo, tutto il giorno, ogni giorno. Di seguito sono riportati alcuni dettagli su come Marketo tratta gli account Dynamics in modo specifico.

## In che modo le informazioni vengono sincronizzate? {#which-way-does-the-information-sync}

Solo un modo: da Dynamics a Marketo.

## Come funzionano gli aggiornamenti? {#how-do-the-updates-work}

Se si aggiorna un campo Account per un contatto in Marketo, vengono modificati i valori di tutti i contatti appartenenti a tale account in Marketo. Non si sincronizza con Dynamics. Tuttavia, al successivo aggiornamento dell’account in Dynamics, le modifiche sovrascriveranno tutte le informazioni sull’account in Marketo.

## Posso creare un account utilizzando Marketo? {#can-i-create-an-account-using-marketo}

No. Marketo non è in grado di creare account in Dynamics.

## Quali campi verranno sincronizzati con Marketo? {#which-fields-will-sync-to-marketo}

È possibile [selezionare i campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) durante la configurazione. Tuttavia, Marketo sincronizzerà solo i campi a cui l’utente di sincronizzazione Dynamics ha accesso.

## Se una modifica in un campo account in Dynamics si traduce in un registro attività Modifica valore dati per ogni contatto?  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

Principalmente sì. Tuttavia, se un account ha più di 5.000 contatti e un campo su tale account cambia in Dynamics, sincronizzeremo la modifica ma non registreremo l&#39;attività per più di 5.000 contatti.
