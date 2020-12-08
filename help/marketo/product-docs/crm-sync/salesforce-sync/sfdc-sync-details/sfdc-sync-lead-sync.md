---
unique-page-id: 2953455
description: Sincr. SFDC - Sincr. lead - Documenti Marketo - Documentazione del prodotto
title: Sincr. SFDC - Sincronizzazione lead
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---


# Sincr. SFDC: Sincronizzazione lead {#sfdc-sync-lead-sync}

>[!NOTE]
>
>**FYI**
>
>Marketo sta standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che nell&#39;abbonamento siano presenti lead/lead e persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

Conoscevi le sincronizzazioni di Marketo dal tuo database Salesforce? Si sincronizza, aspetta 5 minuti, poi si sincronizza di nuovo. Tutto il giorno, ogni giorno. Di seguito sono riportati alcuni dettagli su come Marketo gestisce in modo specifico i lead Salesforce.

## Direzione sincronizzazione {#sync-direction}

Il lead (persona) e la sincronizzazione dei contatti sono bidirezionali. Se apporti modifiche a un record in Salesforce o in Marketo, gli aggiornamenti si rifletteranno su entrambi i sistemi.

## E se le modifiche fossero apportate contemporaneamente in entrambi i sistemi? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo vince. È raro che si verifichino simili collisioni di dati.

## Posso creare un lead in Salesforce utilizzando Marketo? {#can-i-create-a-lead-in-salesforce-using-marketo}

Sì, utilizza l’azione di flusso [Sincronizza persona con SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) . Questo creerà un lead in Salesforce se il lead non esiste.

## È possibile forzare manualmente la sincronizzazione di una persona in Marketo con un lead in Salesforce? {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

Sì, utilizza l’azione di flusso [Sincronizza persona con SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) e si sincronizza in tempo reale.

## Ogni singolo campo standard viene sincronizzato con Marketo? {#does-every-single-standard-field-sync-to-marketo}

No, non tutti i campi standard sono utili. Tutti i campi personalizzati possono essere parte della sincronizzazione.

>[!NOTE]
>
>Marketo sincronizzerà solo i campi a cui ha accesso l’utente della sincronizzazione Salesforce.

## Marketo rispetterà le regole di convalida di Salesforce? {#will-marketo-respect-the-salesforce-validation-rules}

Sì. La sincronizzazione non riesce se il formato dei dati è errato o mancano le informazioni sul campo necessarie. Marketo registrerà il risultato nel registro attività lead, se questo accade.
