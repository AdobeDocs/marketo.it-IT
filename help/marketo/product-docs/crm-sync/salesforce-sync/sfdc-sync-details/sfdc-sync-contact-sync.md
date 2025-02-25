---
unique-page-id: 2953457
description: Sincronizzazione SFDC - Sincronizzazione contatti - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Sincronizzazione contatti
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Sincronizzazione SFDC: Sincronizzazione contatti {#sfdc-sync-contact-sync}

Lo sapevi che Marketo Engage sincronizza l&#39;intero database con Salesforce? Si sincronizza, poi aspetta 5 minuti e poi si sincronizza di nuovo, tutto il giorno, ogni giorno. Ecco alcuni dettagli su come Marketo tratta in modo specifico i contatti Salesforce.

## Direzione di sincronizzazione {#sync-direction}

La sincronizzazione dei contatti è bidirezionale. Se apporti modifiche a un contatto in Salesforce o Marketo, i tuoi aggiornamenti si rifletteranno in entrambi i sistemi.

## Cosa succede se vengono apportate modifiche contemporaneamente in entrambi i sistemi? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Siamo gentili e lasciamo vincere Salesforce. È raro che si verifichi questo tipo di conflitto di dati.

## È possibile convertire una persona in un contatto in Marketo? {#can-i-convert-a-person-into-a-contact-in-marketo}

Sì, utilizza l&#39;azione di flusso **[Converti persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"}**.

>[!CAUTION]
>
>La conversione di una persona in Marketo determinerà un nuovo account e una nuova opportunità in Salesforce. Se non desideri account duplicati, usa Salesforce per la conversione.

## È possibile forzare manualmente la sincronizzazione di un contatto? {#can-i-manually-force-a-sync-of-a-contact}

Sì, utilizza l&#39;azione di flusso **[Sincronizza persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}** che verrà sincronizzata in tempo reale.

## Ogni singolo campo standard è sincronizzato con Marketo? {#does-every-single-standard-field-sync-to-marketo}

No, non tutti i campi standard sono utili. Tutti i campi personalizzati possono far parte della sincronizzazione.

>[!NOTE]
>
>Marketo sincronizzerà solo i campi a cui l’utente di Marketo Sync ha accesso.

## Marketo rispetterà le regole di convalida Salesforce? {#will-marketo-respect-the-salesforce-validation-rules}

Sì, se si verifica un conflitto, il risultato verrà registrato nel registro attività lead.
