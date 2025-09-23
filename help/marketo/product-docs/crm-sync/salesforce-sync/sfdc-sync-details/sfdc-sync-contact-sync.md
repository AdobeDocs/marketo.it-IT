---
unique-page-id: 2953457
description: Sincronizzazione SFDC - Sincronizzazione contatti - Documentazione Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Sincronizzazione contatti
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 1%

---

# Sincronizzazione SFDC: sincronizzazione contatti {#sfdc-sync-contact-sync}

Lo sapevi che Marketo sincronizza l&#39;intero database con [!DNL Salesforce]? Si sincronizza, poi aspetta 5 minuti e poi si sincronizza di nuovo, tutto il giorno, ogni giorno. Ecco alcuni dettagli su come Marketo tratta in modo specifico i contatti di [!DNL Salesforce].

## Direzione di sincronizzazione {#sync-direction}

La sincronizzazione dei contatti è bidirezionale. Se si apportano modifiche a un contatto in [!DNL Salesforce] o Marketo, gli aggiornamenti verranno applicati a entrambi i sistemi.

## Cosa succede se vengono apportate modifiche contemporaneamente in entrambi i sistemi? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Siamo gentili e lasciamo vincere [!DNL Salesforce]. È raro che si verifichi questo tipo di conflitto di dati.

## È possibile convertire una persona in un contatto in Marketo? {#can-i-convert-a-person-into-a-contact-in-marketo}

Sì, utilizza l&#39;azione di flusso **[Converti persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"}**.

>[!CAUTION]
>
>La conversione di una persona in Marketo determinerà un nuovo account e una nuova opportunità in [!DNL Salesforce]. Se non si desidera duplicare gli account, utilizzare [!DNL Salesforce] per la conversione.

## È possibile forzare manualmente la sincronizzazione di un contatto? {#can-i-manually-force-a-sync-of-a-contact}

Sì, utilizza l&#39;azione di flusso **[Sincronizza persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}** che verrà sincronizzata in tempo reale.

## Ogni singolo campo standard è sincronizzato con Marketo? {#does-every-single-standard-field-sync-to-marketo}

No, non tutti i campi standard sono utili. Tutti i campi personalizzati possono far parte della sincronizzazione.

>[!NOTE]
>
>Marketo sincronizzerà solo i campi a cui l’utente di Marketo Sync ha accesso.

## Marketo rispetterà le regole di convalida [!DNL Salesforce]? {#will-marketo-respect-the-salesforce-validation-rules}

Sì, se si verifica un conflitto, il risultato verrà registrato nel registro attività lead.
