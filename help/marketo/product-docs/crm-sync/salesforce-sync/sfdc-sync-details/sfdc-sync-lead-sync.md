---
unique-page-id: 2953455
description: Sincr. SFDC - Sincronizzazione lead - Documenti Marketo - Documentazione del prodotto
title: Sincr. SFDC - Sincronizzazione lead
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Sincr. SFDC: Sincronizzazione lead {#sfdc-sync-lead-sync}

Lei conosceva le sincronizzazioni Marketo dal suo database Salesforce? Si sincronizza, aspetta 5 minuti, poi si sincronizza di nuovo. Tutto il giorno, ogni giorno. Di seguito sono riportati alcuni dettagli su come Marketo tratta in modo specifico i lead Salesforce.

## Direzione sincronizzazione {#sync-direction}

La sincronizzazione del lead (persona) e del contatto è bidirezionale. Se apporti modifiche a un record in Salesforce o Marketo, gli aggiornamenti verranno rispecchiati in entrambi i sistemi.

## E se le modifiche vengono apportate contemporaneamente in entrambi i sistemi? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

vince Marketo. È raro che si verifichi questo tipo di collisione di dati.

## Posso creare un lead in Salesforce utilizzando Marketo? {#can-i-create-a-lead-in-salesforce-using-marketo}

Sì, utilizza l&#39;azione di flusso [Sincronizza persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md). Questo creerà un lead in Salesforce se il lead non esiste.

## È possibile forzare manualmente la sincronizzazione di una persona in Marketo con un lead in Salesforce? {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

Sì, utilizza l&#39;azione di flusso [Sincronizza persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) e si sincronizza in tempo reale.

## Ogni singolo campo standard si sincronizza con Marketo? {#does-every-single-standard-field-sync-to-marketo}

No, non tutti i campi standard sono utili. Tutti i campi personalizzati possono far parte della sincronizzazione.

>[!NOTE]
>
>Marketo sincronizzerà solo i campi a cui l’utente di sincronizzazione Salesforce ha accesso.

## Marketo rispetterà le regole di convalida di Salesforce? {#will-marketo-respect-the-salesforce-validation-rules}

Sì. La sincronizzazione avrà esito negativo se il formato dei dati è errato o se mancano le informazioni sul campo richieste. In questo caso, Marketo registra il risultato nel registro attività dei lead.
