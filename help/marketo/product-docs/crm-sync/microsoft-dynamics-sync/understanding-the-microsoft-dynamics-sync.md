---
unique-page-id: 10098625
description: Informazioni su Microsoft Dynamics Sync - Marketo Docs - Documentazione prodotto
title: Informazioni sulla sincronizzazione di Microsoft Dynamics
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---


# Informazioni sulla sincronizzazione di Microsoft Dynamics {#understanding-the-microsoft-dynamics-sync}

Marketo e Microsoft Dynamics insieme. Manteniamo sincronizzati i dati di vendita e marketing.

>[!NOTE]
>
>Marketo supporta solo certificati SSL compatibili con Java 7.

## Come funziona la sincronizzazione {#how-sync-works}

Marketo sincronizza continuamente i dati con Microsoft Dynamics tutto il giorno, ogni giorno. Viene eseguito usando la sincronizzazione in background, in batch, non in tempo reale.

>[!NOTE]
>
>La prima sincronizzazione dell&#39;abbonamento richiede minuti di ore, a seconda delle dimensioni del database. Marketo copia l&#39;intero database da Dynamics. In seguito, ogni sincronizzazione richiede in genere secondi o minuti e sincronizza solo i dati modificati.

La sincronizzazione tra Marketo e Dynamics è bidirezionale per lead e contatti. Se apporti modifiche in Marketing Cloud o Dynamics, gli aggiornamenti si rifletteranno su entrambi i sistemi. Tutti gli altri campi, come account e opportunità, sono sincronizzati solo in un modo, da Dynamics a Marketo.

## Cosa è sincronizzato tra Marketo e Microsoft Dynamics? {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [Lead](microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [Contatti](microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [Account](microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [Utenti](microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* Team (gruppi di SystemUsers)
* [Opportunità](microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [Entità personalizzate](microsoft-dynamics-sync-details/microsoft-dynamics-sync-custom-entity-sync.md)

>[!NOTE]
>
>Le [credenziali immesse in Marketo per Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md) vengono utilizzate per sincronizzare i dati.

Esistono molte sfumature e funzionalità sulla sincronizzazione Dynamics. Consultate i dettagli nella sezione [Dettagli sincronizzazione di](http://docs.marketo.com/display/docs/microsoft+dynamics+sync+details)Microsoft Dynamics.

>[!CAUTION]
>
>Al momento non è supportato l&#39;aggiornamento sandbox per Marketo Dynamics Sync. Se devi aggiornare la sandbox di Dynamics CRM, sarà necessaria una nuova sandbox di Marketo. Contatta il tuo Customer Success Manager per ulteriori informazioni.

>[!NOTE]
>
>**Articoli correlati**
>
>* [Configurazione sincronizzazione](http://docs.marketo.com/display/docs/sync+setup)
   >
   >
* [Dettagli sincronizzazione di Microsoft Dynamics](http://docs.marketo.com/display/docs/microsoft+dynamics+sync+details)

