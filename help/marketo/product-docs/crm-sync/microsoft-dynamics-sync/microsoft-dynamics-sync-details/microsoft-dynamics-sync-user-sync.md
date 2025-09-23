---
unique-page-id: 3571840
description: Microsoft [!DNL Dynamics] Sincronizza - Sincronizzazione utenti - Documenti Marketo - Documentazione del prodotto
title: Microsoft [!DNL Dynamics] Sincronizza - Sincronizzazione utente
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 0%

---

# Sincronizzazione di Microsoft [!DNL Dynamics]: sincronizzazione utenti {#microsoft-dynamics-sync-user-sync}

Lo sapevi che Marketo sincronizza l&#39;intero database con [!DNL Dynamics]? Si sincronizza, poi aspetta 5 minuti e poi si sincronizza di nuovo, tutto il giorno, ogni giorno. Ecco alcuni dettagli su come Marketo tratta gli account [!DNL Dynamics] in modo specifico.

Sarà necessario un utente CRM Microsoft [!DNL Dynamics] dedicato ai fini dell&#39;integrazione. Questo utente viene chiamato utente di sincronizzazione.

## In che modo i dettagli utente vengono mantenuti sincronizzati tra i due sistemi? {#how-are-user-details-kept-in-sync-between-the-two-systems}

La sincronizzazione utente è unidirezionale: [!DNL Dynamics] a Marketo. Se si apportano modifiche a un utente in [!DNL Dynamics], le modifiche verranno applicate in Marketo.

## Posso creare un utente con Marketo? {#can-i-create-an-user-using-marketo}

No. Marketo: impossibile creare utenti in [!DNL Dynamics].

## Quali campi verranno sincronizzati con Marketo? {#which-fields-will-sync-to-marketo}

È possibile [selezionare i campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) durante l&#39;installazione. Ma Marketo sincronizzerà solo i campi a cui l&#39;utente di sincronizzazione [!DNL Dynamics] ha accesso.
