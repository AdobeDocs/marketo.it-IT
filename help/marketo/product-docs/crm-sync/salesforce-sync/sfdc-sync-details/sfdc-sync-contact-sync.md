---
unique-page-id: 2953457
description: Sincr. SFDC - Contatta Sync - Marketo Docs - Documentazione del prodotto
title: Sincr. SFDC - Contatto Sincronizzazione
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# Sincr. SFDC: Sincronizzazione contatti {#sfdc-sync-contact-sync}

Lo sapevi che Marketo sincronizza l&#39;intero database con Salesforce? Si sincronizza, poi aspetta 5 minuti e poi sincronizza di nuovo, tutto il giorno, ogni giorno. Di seguito sono riportati alcuni dettagli su come Marketo tratta in modo specifico i contatti Salesforce.

## Direzione sincronizzazione {#sync-direction}

La sincronizzazione dei contatti è bidirezionale. Se apporti modifiche a un contatto in Salesforce o Marketo, gli aggiornamenti verranno rispecchiati in entrambi i sistemi.

## E se le modifiche vengono apportate contemporaneamente in entrambi i sistemi? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Siamo gentili e lasciamo vincere Salesforce. È raro che si verifichi questo tipo di collisione di dati.

## Posso convertire una persona in un contatto in Marketo? {#can-i-convert-a-person-into-a-contact-in-marketo}

Sì, utilizza **[Converti persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)** azione di flusso.

>[!CAUTION]
>
>La conversione di una persona in Marketo comporterà un nuovo account e nuove opportunità in Salesforce. Se non desideri account duplicati, utilizza Salesforce per convertire.

## È possibile forzare manualmente la sincronizzazione di un contatto? {#can-i-manually-force-a-sync-of-a-contact}

Sì, utilizza **[Sincronizza persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** azione di flusso e si sincronizza in tempo reale.

## Ogni singolo campo standard si sincronizza con Marketo? {#does-every-single-standard-field-sync-to-marketo}

No, non tutti i campi standard sono utili. Tutti i campi personalizzati possono far parte della sincronizzazione.

>[!NOTE]
>
>Marketo sincronizzerà solo i campi a cui l’utente di Marketo Sync ha accesso.

## Marketo rispetterà le regole di convalida di Salesforce? {#will-marketo-respect-the-salesforce-validation-rules}

Sì, in caso di conflitto, registra il risultato nel registro attività lead.
