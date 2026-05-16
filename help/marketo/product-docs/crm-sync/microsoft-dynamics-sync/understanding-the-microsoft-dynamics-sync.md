---
unique-page-id: 10098625
description: Scopri in che modo la sincronizzazione di Microsoft Dynamics mantiene sincronizzati i dati di Marketo e Dynamics. Scopri cosa è sincronizzato e come funziona la sincronizzazione bidirezionale per lead e contatti.
title: Informazioni sulla sincronizzazione con Microsoft Dynamics
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
feature: Microsoft Dynamics
TQID: https://experienceleague.adobe.com/-Fr-yRhPskeESDyxFULmD-GIXvY5uqVANkGiCX3PhTM
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: c5f60233-d5ea-4453-a799-0ad258b4d399
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 230
ht-degree: 20%

---

# Informazioni sulla sincronizzazione con [!DNL Microsoft Dynamics] {#understanding-the-microsoft-dynamics-sync}

Marketo e [!DNL Microsoft Dynamics] vanno insieme. Mantengono la sincronizzazione dei dati di vendita e di marketing.

>[!CAUTION]
>
>Al momento non è supportato l&#39;aggiornamento della sandbox per la sincronizzazione [!DNL Marketo Dynamics]. Se è necessario aggiornare la sandbox CRM di [!DNL Dynamics], sarà necessaria una nuova sandbox Marketo. Per ulteriori informazioni, contatta il tuo Customer Success Manager.

## Funzionamento della sincronizzazione {#how-sync-works}

Marketo sincronizza continuamente i dati con [!DNL Microsoft Dynamics] tutto il giorno, ogni giorno. Viene eseguita utilizzando la sincronizzazione in background, in batch, non in tempo reale.

>[!NOTE]
>
>La prima sincronizzazione della sottoscrizione richiede da minuti a ore, a seconda delle dimensioni del database. Marketo copia l&#39;intero database da [!DNL Dynamics]. In seguito, ciascuna sincronizzazione richiede in genere pochi secondi o minuti e vengono sincronizzati solo i dati modificati.

La sincronizzazione tra Marketo e [!DNL Dynamics] è bidirezionale per lead e contatti. Se si apportano modifiche in Marketo o [!DNL Dynamics], gli aggiornamenti verranno applicati a entrambi i sistemi. Tutti gli altri campi, ad esempio account e opportunità, vengono sincronizzati in un solo modo, da [!DNL Dynamics] a Marketo.

## Che cosa viene sincronizzato tra Marketo e [!DNL Microsoft Dynamics]? {#what-is-synced-between-marketo-and-microsoft-dynamics}

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
