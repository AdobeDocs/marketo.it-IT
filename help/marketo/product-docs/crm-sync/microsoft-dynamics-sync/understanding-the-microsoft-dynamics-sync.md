---
unique-page-id: 10098625
description: Informazioni su Microsoft Dynamics Sync - Marketo Docs - Documentazione del prodotto
title: Informazioni sulla sincronizzazione di Microsoft Dynamics
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 0%

---

# Informazioni sulla sincronizzazione di Microsoft Dynamics {#understanding-the-microsoft-dynamics-sync}

Marketo e Microsoft Dynamics sono compatibili. Manteniamo sincronizzati i dati di vendita e marketing.

>[!NOTE]
>
>Marketo supporta solo i certificati SSL compatibili con Java 7 al momento.

## Funzionamento della sincronizzazione {#how-sync-works}

Marketo sincronizza continuamente i dati con Microsoft Dynamics tutto il giorno e ogni giorno. Viene eseguito usando la sincronizzazione in background, in batch, non in tempo reale.

>[!NOTE]
>
>La prima sincronizzazione della sottoscrizione richiede minuti alle ore, a seconda delle dimensioni del database. Marketo copia l’intero database da Dynamics. In seguito, ogni sincronizzazione richiede in genere secondi o minuti e sincronizza solo i dati che sono cambiati.

La sincronizzazione tra Marketo e Dynamics è bidirezionale per lead e contatti. Se apporti modifiche in Marketo o Dynamics, gli aggiornamenti verranno rispecchiati in entrambi i sistemi. Tutti gli altri campi, come account e opportunità, vengono sincronizzati in un solo modo, da Dynamics a Marketo.

## Cosa viene sincronizzato tra Marketo e Microsoft Dynamics? {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [Lead](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [Contatti](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [Account](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [Utenti](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* Team (gruppi di SystemUsers)
* [Opportunità](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [Entità personalizzate](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-custom-entity-sync.md)

>[!NOTE]
>
>Le [credenziali immesse in Marketo per Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md) vengono utilizzate per sincronizzare i dati.

>[!CAUTION]
>
>Al momento non è supportato l’aggiornamento della sandbox per Marketo Dynamics Sync. Se devi aggiornare la sandbox di Dynamics CRM, sarà necessaria una nuova sandbox Marketo. Per ulteriori informazioni, contatta il tuo Customer Success Manager.
