---
unique-page-id: 3571836
description: Microsoft Dynamics Sync - Sincronizzazione account - Documenti Marketo - Documentazione prodotto
title: Microsoft Dynamics Sync - Sincronizzazione account
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Sincronizzazione account {#microsoft-dynamics-sync-account-sync}

Sapevate che Marketo sincronizza l&#39;intero database con Dynamics? Si sincronizza, poi aspetta 5 minuti e poi si sincronizza di nuovo, tutto il giorno, ogni giorno. Di seguito sono riportati alcuni dettagli su come Marketo gestisce in modo specifico gli account di Dynamics.

## In che modo vengono sincronizzate le informazioni? {#which-way-does-the-information-sync}

Solo un modo: da Dynamics a Marketo.

## Come funzionano gli aggiornamenti? {#how-do-the-updates-work}

Se si aggiorna un campo Account per un contatto in Marketo, vengono modificati i valori di tutti i contatti appartenenti a tale account in Marketo. Non si sincronizza con Dynamics. Tuttavia, al successivo aggiornamento dell&#39;account in Dynamics, le modifiche sostituiranno tutte le informazioni sull&#39;account in Marketo.

## Posso creare un account con Marketo? {#can-i-create-an-account-using-marketo}

No. Impossibile creare account in Dynamics.

## Quali campi verranno sincronizzati con Marketo? {#which-fields-will-sync-to-marketo}

Potete [selezionare i campi da sincronizzare](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) durante l&#39;impostazione. Tuttavia, Marketo sincronizzerà solo i campi a cui l&#39;utente della sincronizzazione Dynamics ha accesso.

## Se una modifica in un campo account di Dynamics restituisce un log attività di modifica del valore dei dati per ogni contatto?  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

Principalmente sì. Tuttavia, se un account ha più di 5.000 contatti e un campo su tale account cambia in Dynamics, sincronizzeremo la modifica ma non registreremo l&#39;attività per i 5.000 contatti.
