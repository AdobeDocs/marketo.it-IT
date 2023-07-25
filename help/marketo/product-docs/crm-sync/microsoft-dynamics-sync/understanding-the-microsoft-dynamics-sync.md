---
unique-page-id: 10098625
description: Informazioni su Microsoft Dynamics Sync - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni su Microsoft Dynamics Sync
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Informazioni su Microsoft Dynamics Sync {#understanding-the-microsoft-dynamics-sync}

Marketo e Microsoft Dynamics funzionano insieme. Manteniamo sincronizzati i dati di vendita e marketing.

>[!NOTE]
>
>Al momento, Marketo supporta solo i certificati SSL compatibili con Java 7.

>[!CAUTION]
>
>Al momento non è supportato l’aggiornamento della sandbox per Marketo Dynamics Sync. Se devi aggiornare la sandbox di Dynamics CRM, sarà necessaria una nuova sandbox di Marketo. Per ulteriori informazioni, contatta l’Adobe Account Team (il tuo Account Manager).

## Funzionamento di Sync {#how-sync-works}

Marketo sincronizza continuamente i dati con Microsoft Dynamics tutto il giorno, ogni giorno. Viene eseguita utilizzando la sincronizzazione in background, in batch, non in tempo reale.

>[!NOTE]
>
>La prima sincronizzazione della sottoscrizione richiede da minuti a ore, a seconda delle dimensioni del database. Marketo copia l’intero database da Dynamics. Successivamente, ogni sincronizzazione richiede in genere secondi o minuti e sincronizza solo i dati modificati.

La sincronizzazione tra Marketo e Dynamics è bidirezionale per lead e contatti. Se apporti modifiche in Marketo o Dynamics, i tuoi aggiornamenti si rifletteranno in entrambi i sistemi. Tutti gli altri campi, ad esempio account e opportunità, vengono sincronizzati in un solo modo, da Dynamics a Marketo.

## Cos’è sincronizzato tra Marketo e Microsoft Dynamics? {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [Lead](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [Contatti](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [Account](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [Utenti](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* Team (gruppi di UtentiSistema)
* [Opportunità](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [Entità personalizzate](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/enable-sync-for-a-custom-entity.md)

Il [credenziali immesse in Marketo for Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md) vengono utilizzati per sincronizzare i dati.

>[!NOTE]
>
>La copia dell’istanza non è supportata se l’istanza di origine è integrata con Microsoft Dynamics.
