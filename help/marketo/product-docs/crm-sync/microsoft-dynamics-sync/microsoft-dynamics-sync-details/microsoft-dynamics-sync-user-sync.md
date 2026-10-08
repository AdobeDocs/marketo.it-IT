---
unique-page-id: 3571840
description: Scopri come i dati utente vengono sincronizzati da Microsoft Dynamics a Marketo. Scopri quali campi proprietari vengono sincronizzati e come utilizzarli negli elenchi avanzati e nelle azioni di flusso.
title: Sincronizzazione Microsoft [!DNL Dynamics] - Utente
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
feature: Microsoft Dynamics
TQID: 'https://experienceleague.adobe.com/8H1bMdkhxcvyTuYtHHk00GUy4uycuQ1unsGbZ19AjCM'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: d5c7388a-594e-4d15-9b39-98d6ce479e8b
    internal-label: Microsoft Dynamics
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 0%
---
# Sincronizzazione di Microsoft [!DNL Dynamics]: sincronizzazione utenti {#microsoft-dynamics-sync-user-sync}

Marketo sincronizza l&#39;intero database con [!DNL Dynamics]. Si sincronizza, poi aspetta 5 minuti e poi si sincronizza di nuovo, tutto il giorno, ogni giorno. Ecco alcuni dettagli su come Marketo tratta gli account [!DNL Dynamics] in modo specifico.

Sarà necessario un utente CRM Microsoft [!DNL Dynamics] dedicato ai fini dell&#39;integrazione. Questo utente viene chiamato utente di sincronizzazione.

## In che modo i dettagli utente vengono mantenuti sincronizzati tra i due sistemi? {#how-are-user-details-kept-in-sync-between-the-two-systems}

La sincronizzazione utente è unidirezionale: [!DNL Dynamics] a Marketo. Se si apportano modifiche a un utente in [!DNL Dynamics], le modifiche verranno applicate in Marketo.

## Posso creare un utente con Marketo? {#can-i-create-an-user-using-marketo}

No. Marketo: impossibile creare utenti in [!DNL Dynamics].

## Quali campi verranno sincronizzati con Marketo? {#which-fields-will-sync-to-marketo}

È possibile [selezionare i campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) durante l&#39;installazione. Ma Marketo sincronizzerà solo i campi a cui l&#39;utente di sincronizzazione [!DNL Dynamics] ha accesso.
