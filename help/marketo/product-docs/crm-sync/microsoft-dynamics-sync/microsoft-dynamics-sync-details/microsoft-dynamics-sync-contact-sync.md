---
unique-page-id: 3571833
description: Sincronizzazione Microsoft Dynamics - Sincronizzazione Contatti - Documenti Marketo - Documentazione Del Prodotto
title: Sincronizzazione Microsoft Dynamics - Sincronizzazione contatti
exl-id: d4583ea0-2b52-415e-b28c-a8eafebeff64
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# Sincronizzazione Microsoft Dynamics: Sincronizzazione contatti {#microsoft-dynamics-sync-contact-sync}

Lo sapevi che Marketo sincronizza l’intero database con Dynamics? Si sincronizza, poi aspetta 5 minuti e poi si sincronizza di nuovo, tutto il giorno, ogni giorno. Di seguito sono riportati alcuni dettagli su come Marketo tratta in modo specifico i contatti Dynamics.

## Come vengono mantenuti sincroni i dettagli tra i due sistemi? {#how-are-details-kept-in-sync-between-the-two-systems}

La sincronizzazione dei contatti è bidirezionale. Se apporti modifiche a un contatto in Dynamics o a una persona in Marketo, gli aggiornamenti verranno applicati a entrambi i sistemi.

## Cosa succede se vengono apportate modifiche allo stesso campo in entrambi i sistemi contemporaneamente? (Conflitto di dati) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Anche se questo è raro, Marketo vincerà per le persone e Dynamics vincerà per i contatti. Questo perché consideriamo il reparto marketing come autorevole per le persone, mentre il sistema ufficiale di registrazione per i contatti è nel reparto vendite (CRM).

## Posso creare un contatto con Marketo? {#can-i-create-a-contact-using-marketo}

Sì. [Ecco come](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md).

>[!NOTE]
>
>Quando si utilizza l’azione di flusso &quot;Sincronizza persona con Microsoft&quot; (solo in una campagna di attivazione), il lead/contatto verrà creato in tempo reale in Dynamics.

## È possibile forzare manualmente la sincronizzazione di una persona o di un contatto? {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

No, la sincronizzazione in background automatizzata è l’unico modo per sincronizzare gli aggiornamenti tra Marketo e Dynamics. Il [Sincronizza persona con Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) non forzerà la sincronizzazione del lead.

## Quali campi verranno sincronizzati con Marketo? {#what-fields-will-sync-to-marketo}

È possibile [seleziona i campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) durante l&#39;installazione. Marketo sincronizzerà solo i campi a cui l’utente di Dynamics Sync ha accesso.

## Marketo rispetterà le regole di convalida Dynamics? {#will-marketo-respect-the-dynamics-validation-rules}

Sì, se si verifica un conflitto, il risultato verrà registrato nel registro attività lead.
