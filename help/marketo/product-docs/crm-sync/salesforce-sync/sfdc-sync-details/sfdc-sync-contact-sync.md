---
unique-page-id: 2953457
description: Sincr. SFDC - Sincronizzazione contatto - Documenti Marketo - Documentazione del prodotto
title: Sincr. SFDC - Sincronizzazione contatto
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---


# Sincr. SFDC: Sincronizzazione contatti {#sfdc-sync-contact-sync}

Sapevi che Marketo sincronizza l&#39;intero database con Salesforce? Si sincronizza, poi aspetta 5 minuti e poi si sincronizza di nuovo, tutto il giorno, ogni giorno. Di seguito sono riportati alcuni dettagli su come Marketo gestisce in modo specifico i contatti Salesforce.

## Direzione sincronizzazione {#sync-direction}

La sincronizzazione dei contatti è bidirezionale. Se apporti modifiche a un contatto in Salesforce o in Marketo, gli aggiornamenti si rifletteranno su entrambi i sistemi.

## E se le modifiche fossero apportate contemporaneamente in entrambi i sistemi? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Siamo gentili e lasciamo vincere Salesforce. È raro che si verifichino simili collisioni di dati.

## Posso convertire una persona in un contatto a Marketo? {#can-i-convert-a-person-into-a-contact-in-marketo}

Sì, utilizza l&#39;azione di flusso ** [Converti persona](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)**.

>[!CAUTION]
>
>La conversione di una persona in Marketo darà luogo a un nuovo account e a nuove opportunità in Salesforce. Se non vuoi duplicare gli account, usa Salesforce per convertire.

## È possibile forzare manualmente la sincronizzazione di un contatto? {#can-i-manually-force-a-sync-of-a-contact}

Sì, utilizza l&#39;azione di flusso ** [Sync Person to SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) **e si sincronizza in tempo reale.

## Ogni singolo campo standard viene sincronizzato con Marketo? {#does-every-single-standard-field-sync-to-marketo}

No, non tutti i campi standard sono utili. Tutti i campi personalizzati possono essere parte della sincronizzazione.

>[!NOTE]
>
>Marketo sincronizzerà solo i campi a cui ha accesso l’utente di sincronizzazione Marketo.

## Marketo rispetterà le regole di convalida di Salesforce? {#will-marketo-respect-the-salesforce-validation-rules}

Sì, in caso di conflitto il risultato verrà registrato nel registro attività lead.
