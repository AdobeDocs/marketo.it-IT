---
unique-page-id: 3571836
description: Scopri come le informazioni dell’account vengono sincronizzate da Microsoft Dynamics a Marketo. Comprendere la sincronizzazione unidirezionale e la relazione contatto-account.
title: Sincronizzazione Microsoft Dynamics - Sincronizzazione account
exl-id: 86249d33-60dd-47e1-a7c8-3996c9444084
feature: Microsoft Dynamics
TQID: 'https://experienceleague.adobe.com/O4tO6DCM-BhwZriMmPGiQqzuhpIc-rWAKojWCn5-Ab8'
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
source-wordcount: '217'
ht-degree: 0%
---
# Sincronizzazione [!DNL Microsoft Dynamics]: sincronizzazione account {#microsoft-dynamics-sync-account-sync}

Marketo sincronizza l&#39;intero database con [!DNL Dynamics]. Si sincronizza, poi aspetta 5 minuti e poi si sincronizza di nuovo, tutto il giorno, ogni giorno. Ecco alcuni dettagli su come Marketo tratta gli account [!DNL Dynamics] in modo specifico.

## In che modo vengono sincronizzate le informazioni? {#which-way-does-the-information-sync}

Solo un modo: da [!DNL Dynamics] a Marketo.

## Come funzionano gli aggiornamenti? {#how-do-the-updates-work}

Se si aggiorna un campo Account per un contatto in Marketo, vengono modificati i valori di tutti i contatti appartenenti a tale account in Marketo. Non è sincronizzato con [!DNL Dynamics]. Tuttavia, al prossimo aggiornamento dell&#39;account in [!DNL Dynamics], le modifiche sostituiranno tutte le informazioni dell&#39;account in Marketo.

## Posso creare un account con Marketo? {#can-i-create-an-account-using-marketo}

No. Marketo: impossibile creare account in [!DNL Dynamics].

## Quali campi verranno sincronizzati con Marketo? {#which-fields-will-sync-to-marketo}

È possibile [selezionare i campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) durante l&#39;installazione. Ma Marketo sincronizzerà solo i campi a cui l&#39;utente di sincronizzazione [!DNL Dynamics] ha accesso.

## Una modifica in un campo account in [!DNL Dynamics] determina un registro attività Modifica valore dati per ogni contatto?  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

Per lo più, sì. Tuttavia, se un account ha più di 5.000 contatti e un campo su tale account cambia in [!DNL Dynamics], la modifica verrà sincronizzata ma non verrà registrata l&#39;attività per gli oltre 5.000 contatti.
