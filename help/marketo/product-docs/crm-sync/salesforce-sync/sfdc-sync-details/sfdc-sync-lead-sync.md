---
unique-page-id: 2953455
description: Sincronizzazione SFDC - Sincronizzazione lead - Documentazione Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Sincronizzazione lead
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 2%

---

# Sincronizzazione SFDC: sincronizzazione lead {#sfdc-sync-lead-sync}

Conoscevi le sincronizzazioni di Marketo dal tuo database [!DNL Salesforce]? Viene sincronizzato, attende 5 minuti, quindi viene sincronizzato di nuovo. Tutto il giorno, tutti i giorni. Ecco alcuni dettagli su come Marketo tratta in modo specifico i lead [!DNL Salesforce].

## Direzione di sincronizzazione {#sync-direction}

La sincronizzazione di lead (persona) e contatti è bidirezionale. Se si apportano modifiche a un record in [!DNL Salesforce] o Marketo, gli aggiornamenti verranno applicati a entrambi i sistemi.

## Cosa succede se vengono apportate modifiche contemporaneamente in entrambi i sistemi? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo vince. È raro che si verifichi questo tipo di conflitto di dati.

## Posso creare un lead in [!DNL Salesforce] utilizzando Marketo? {#can-i-create-a-lead-in-salesforce-using-marketo}

Sì, utilizza l&#39;azione di flusso [Sincronizza persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md). Questo creerà un lead in [!DNL Salesforce] se il lead non esiste.

## È possibile forzare manualmente la sincronizzazione di una persona in Marketo con un lead in [!DNL Salesforce]? {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

Sì, utilizza l&#39;azione di flusso [Sincronizza persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} che verrà sincronizzata in tempo reale.

## Ogni singolo campo standard è sincronizzato con Marketo? {#does-every-single-standard-field-sync-to-marketo}

No, non tutti i campi standard sono utili. Tutti i campi personalizzati possono far parte della sincronizzazione.

>[!NOTE]
>
>Marketo sincronizzerà solo i campi a cui ha accesso l&#39;utente di sincronizzazione [!DNL Salesforce].

## Marketo rispetterà le regole di convalida [!DNL Salesforce]? {#will-marketo-respect-the-salesforce-validation-rules}

Sì.  La sincronizzazione non riuscirà se il formato dei dati non è corretto o se mancano le informazioni richieste sul campo. In questo caso, Marketo registrerà il risultato nel registro attività dei lead.
