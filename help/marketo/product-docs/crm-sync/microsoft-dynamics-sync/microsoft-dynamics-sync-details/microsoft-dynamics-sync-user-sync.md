---
unique-page-id: 3571840
description: Sincronizzazione Microsoft Dynamics - Sincronizzazione utenti - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione Microsoft Dynamics - Sincronizzazione utenti
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---

# Sincronizzazione Microsoft Dynamics: Sincronizzazione utenti {#microsoft-dynamics-sync-user-sync}

Lo sapevi che Marketo sincronizza l’intero database con Dynamics? Si sincronizza, poi aspetta 5 minuti e poi si sincronizza di nuovo, tutto il giorno, ogni giorno. Di seguito sono riportati alcuni dettagli su come Marketo tratta gli account Dynamics in modo specifico.

Ai fini dell’integrazione, sarà necessario un utente Microsoft Dynamics CRM dedicato. Questo utente viene chiamato utente di sincronizzazione.

## In che modo i dettagli utente vengono mantenuti sincronizzati tra i due sistemi? {#how-are-user-details-kept-in-sync-between-the-two-systems}

La sincronizzazione utente è unidirezionale: da Dynamics a Marketo. Se apporti modifiche a un utente in Dynamics, tali modifiche verranno applicate in Marketo.

## Posso creare un utente con Marketo? {#can-i-create-an-user-using-marketo}

No. Marketo non può creare utenti in Dynamics.

## Quali campi verranno sincronizzati con Marketo? {#which-fields-will-sync-to-marketo}

È possibile [seleziona i campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) durante l&#39;installazione. Marketo sincronizzerà solo i campi a cui l’utente di Dynamics Sync ha accesso.
