---
unique-page-id: 3571840
description: Microsoft Dynamics Sync - Sincronizzazione utente - Documenti Marketo - Documentazione prodotto
title: Microsoft Dynamics Sync - Sincronizzazione utente
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Sincronizzazione utente {#microsoft-dynamics-sync-user-sync}

Sapevate che Marketo sincronizza l&#39;intero database con Dynamics? Si sincronizza, poi aspetta 5 minuti e poi si sincronizza di nuovo, tutto il giorno, ogni giorno. Di seguito sono riportati alcuni dettagli su come Marketo gestisce in modo specifico gli account di Dynamics.

Sarà necessario un utente Microsoft Dynamics CRM dedicato ai fini dell&#39;integrazione. Questo utente viene chiamato Utente sincronizzazione.

## Come vengono mantenuti sincronizzati i dettagli utente tra i due sistemi? {#how-are-user-details-kept-in-sync-between-the-two-systems}

La sincronizzazione degli utenti è unidirezionale: da Dynamics a Marketo. Se apporti modifiche a un utente in Dynamics, le modifiche verranno riportate in Marketo.

## Posso creare un utente con Marketo? {#can-i-create-an-user-using-marketo}

No. Marketo non è in grado di creare utenti in Dynamics.

## Quali campi verranno sincronizzati con Marketo? {#which-fields-will-sync-to-marketo}

È possibile [selezionare i campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) durante la configurazione. Tuttavia, Marketo sincronizzerà solo i campi a cui l&#39;utente della sincronizzazione Dynamics ha accesso.
