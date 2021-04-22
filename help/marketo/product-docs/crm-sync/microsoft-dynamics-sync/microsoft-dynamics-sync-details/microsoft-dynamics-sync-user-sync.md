---
unique-page-id: 3571840
description: Microsoft Dynamics Sync - Sincronizzazione utente - Documentazione di Marketo - Documentazione del prodotto
title: Microsoft Dynamics Sync - Sincronizzazione utente
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---

# Sincronizzazione Microsoft Dynamics: Sincronizzazione utente {#microsoft-dynamics-sync-user-sync}

Lo sapevi che Marketo sincronizza l’intero database con Dynamics? Si sincronizza, poi aspetta 5 minuti e poi sincronizza di nuovo, tutto il giorno, ogni giorno. Di seguito sono riportati alcuni dettagli su come Marketo tratta gli account Dynamics in modo specifico.

Sarà necessario un utente Microsoft Dynamics CRM dedicato allo scopo dell’integrazione. Questo utente viene chiamato Utente di sincronizzazione.

## Come vengono mantenuti sincronizzati i dettagli utente tra i due sistemi? {#how-are-user-details-kept-in-sync-between-the-two-systems}

La sincronizzazione utente è unidirezionale: da Dynamics a Marketo. Se apporti modifiche a un utente in Dynamics, queste verranno applicate in Marketo.

## Posso creare un utente utilizzando Marketo? {#can-i-create-an-user-using-marketo}

No. Marketo non è in grado di creare utenti in Dynamics.

## Quali campi verranno sincronizzati con Marketo? {#which-fields-will-sync-to-marketo}

È possibile [selezionare i campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) durante la configurazione. Tuttavia, Marketo sincronizzerà solo i campi a cui l’utente di sincronizzazione Dynamics ha accesso.
