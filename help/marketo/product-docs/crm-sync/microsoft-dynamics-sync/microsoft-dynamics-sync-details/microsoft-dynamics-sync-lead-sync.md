---
unique-page-id: 3571848
description: Microsoft Dynamics Sync - Sincronizzazione lead - Documentazione di Marketo - Documentazione del prodotto
title: Microsoft Dynamics Sync - Sincronizzazione lead
exl-id: ea04a039-32f7-41f9-85fb-18df8e236390
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Sincronizzazione Microsoft Dynamics: Sincronizzazione lead {#microsoft-dynamics-sync-lead-sync}

La sincronizzazione tra Marketo e Dynamics è estremamente potente. Di seguito sono riportati i dettagli:

## Come vengono mantenuti sincronizzati i dettagli tra i due sistemi? {#how-are-details-kept-in-sync-between-the-two-systems}

La sincronizzazione è bidirezionale. Se apporti modifiche a un lead in Dynamics o a una persona in Marketo, l’aggiornamento verrà rispecchiato in entrambi i sistemi.

>[!NOTE]
>
>Le eliminazioni non sempre si sincronizzano automaticamente in entrambe le direzioni. Vedere [Eliminazione di un lead o di un contatto](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md).

## Cosa succede se contemporaneamente vengono apportate modifiche allo stesso campo in entrambi i sistemi? (Collisione dati) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Anche se questo è raro, Marketo vincerà le persone (lead) e Dynamics vincerà i contatti. Questo perché riteniamo che il reparto marketing sia autorevole per le persone, mentre il sistema ufficiale di registrazione dei contatti è nel reparto vendite (CRM).

## Posso creare un lead in Dynamics utilizzando Marketo? {#can-i-create-a-lead-in-dynamics-using-marketo}

Sì, utilizza l&#39;azione di flusso [Sincronizza persona con Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md). In questo modo verrà creato un lead in Dynamics se il lead non esiste. Se il lead esiste, il passaggio di flusso non esegue alcuna azione.

>[!NOTE]
>
>Quando utilizzi l’azione di flusso &quot;Sincronizza persona con Microsoft&quot; (solo in una campagna di trigger), il lead/contatto verrà creato in tempo reale in Dynamics.

## È possibile forzare manualmente la sincronizzazione di una persona da Marketo a un lead in Dynamics? {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

No, la sincronizzazione automatica in background è l’unico modo per sincronizzare gli aggiornamenti tra Marketo e Dynamics. L&#39;azione di flusso [Sincronizza persona con Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) non forzerà la sincronizzazione del lead.

## Quali campi verranno sincronizzati con Marketo? {#what-fields-will-sync-to-marketo}

È possibile [selezionare i campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) durante la configurazione.

## Marketo rispetterà le regole di convalida di Dynamics? {#will-marketo-respect-the-dynamics-validation-rules}

Sì. La sincronizzazione avrà esito negativo se il formato dei dati è errato o se mancano le informazioni sul campo richieste. In questo caso, Marketo registra il risultato nel registro attività della persona.
