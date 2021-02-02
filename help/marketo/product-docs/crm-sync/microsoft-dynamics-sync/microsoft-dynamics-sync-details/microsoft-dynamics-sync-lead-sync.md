---
unique-page-id: 3571848
description: Microsoft Dynamics Sync - Lead Sync - Marketo Docs - Documentazione prodotto
title: Microsoft Dynamics Sync - Sincronizzazione lead
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Sincronizzazione lead {#microsoft-dynamics-sync-lead-sync}

La sincronizzazione tra Marketo e Dynamics è super potente. Di seguito sono riportati i dettagli:

## Come vengono mantenuti sincronizzati i dettagli tra i due sistemi? {#how-are-details-kept-in-sync-between-the-two-systems}

La sincronizzazione è bidirezionale. Se apporti modifiche a un lead in Dynamics o a una persona in Marketo, l’aggiornamento verrà riflesso in entrambi i sistemi.

>[!NOTE]
>
>Le eliminazioni non sempre si sincronizzano automaticamente in entrambe le direzioni. Vedere [Eliminazione di un lead o di un contatto](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md).

## Cosa succede se nello stesso campo vengono apportate modifiche contemporaneamente in entrambi i sistemi? (Collisione dati) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Anche se questo è raro, Marketo vincerà per le persone (lead) e Dynamics vincerà per i contatti. Questo perché riteniamo che il reparto marketing sia autorevole per le persone, mentre il sistema ufficiale di registrazione dei contatti è nel reparto vendite (CRM).

## Posso creare un lead in Dynamics utilizzando Marketo? {#can-i-create-a-lead-in-dynamics-using-marketo}

Sì, utilizza l&#39;azione di flusso [Sincronizza persona con Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md). Questo creerà un lead in Dynamics se il lead non esiste. Se il lead esiste, il passaggio di flusso non esegue alcuna azione.

>[!NOTE]
>
>Quando si utilizza l’azione di flusso &quot;Sincronizza persona con Microsoft&quot; (solo in una campagna di attivazione), il lead/contatto verrà creato in tempo reale in Dynamics.

## È possibile forzare manualmente la sincronizzazione di una persona da Marketo a un lead in Dynamics? {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

No, la sincronizzazione automatica in background è l&#39;unico modo per sincronizzare gli aggiornamenti tra Marketo e Dynamics. L&#39;azione di flusso [Sincronizza persona con Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) non forzerà la sincronizzazione del lead.

## Quali campi verranno sincronizzati con Marketo? {#what-fields-will-sync-to-marketo}

È possibile [selezionare i campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) durante la configurazione.

## Marketo rispetterà le regole di convalida di Dynamics? {#will-marketo-respect-the-dynamics-validation-rules}

Sì. La sincronizzazione non riesce se il formato dei dati è errato o mancano le informazioni sul campo necessarie. Marketo registrerà il risultato nel log delle attività della persona, se questo accade.
