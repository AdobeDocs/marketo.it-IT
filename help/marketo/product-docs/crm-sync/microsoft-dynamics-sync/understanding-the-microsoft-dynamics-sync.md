---
unique-page-id: 10098625
description: Informazioni su  [!DNL Microsoft Dynamics] Sync - Marketo Docs - Documentazione del prodotto
title: Informazioni sulla sincronizzazione con Microsoft Dynamics
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 3%

---

# Informazioni sulla sincronizzazione di [!DNL Microsoft Dynamics] {#understanding-the-microsoft-dynamics-sync}

Marketo e [!DNL Microsoft Dynamics] vanno insieme. Manteniamo sincronizzati i dati di vendita e marketing.

>[!CAUTION]
>
>Al momento non è supportato l&#39;aggiornamento della sandbox per la sincronizzazione [!DNL Marketo Dynamics]. Se è necessario aggiornare la sandbox CRM di [!DNL Dynamics], sarà necessaria una nuova sandbox Marketo. Per ulteriori informazioni, contatta il tuo Customer Success Manager.

## Funzionamento di Sync {#how-sync-works}

Marketo sincronizza continuamente i dati con [!DNL Microsoft Dynamics] tutto il giorno, ogni giorno. Viene eseguita utilizzando la sincronizzazione in background, in batch, non in tempo reale.

>[!NOTE]
>
>La prima sincronizzazione della sottoscrizione richiede da minuti a ore, a seconda delle dimensioni del database. Marketo copia l&#39;intero database da [!DNL Dynamics]. Successivamente, ogni sincronizzazione richiede in genere secondi o minuti e sincronizza solo i dati modificati.

La sincronizzazione tra Marketo e [!DNL Dynamics] è bidirezionale per lead e contatti. Se si apportano modifiche in Marketo o [!DNL Dynamics], gli aggiornamenti verranno applicati a entrambi i sistemi. Tutti gli altri campi, ad esempio account e opportunità, vengono sincronizzati in un solo modo, da [!DNL Dynamics] a Marketo.

## Cos&#39;è sincronizzato tra Marketo e [!DNL Microsoft Dynamics]? {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [Lead](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [Contatti](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [Account](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [Utenti](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* Team (gruppi di UtentiSistema)
* [Opportunità](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [Entità personalizzate](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/enable-sync-for-a-custom-entity.md)

Le [credenziali immesse in Marketo per  [!DNL Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md) vengono utilizzate per sincronizzare i dati.

>[!NOTE]
>
>Copia dell&#39;istanza non supportata se l&#39;istanza di origine è integrata con [!DNL Microsoft Dynamics].
