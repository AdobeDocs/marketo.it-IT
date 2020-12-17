---
unique-page-id: 3571833
description: Microsoft Dynamics Sync - Contatta Sincronizzazione - Documenti Marketo - Documentazione prodotto
title: Microsoft Dynamics Sync - Contatto sincronizzazione
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Sincronizzazione contatto {#microsoft-dynamics-sync-contact-sync}

Sapevate che Marketo sincronizza l&#39;intero database con Dynamics? Si sincronizza, poi aspetta 5 minuti e poi si sincronizza di nuovo, tutto il giorno, ogni giorno. Di seguito sono riportati alcuni dettagli su come Marketo gestisce in modo specifico i contatti di Dynamics.

## Come vengono mantenuti sincronizzati i dettagli tra i due sistemi? {#how-are-details-kept-in-sync-between-the-two-systems}

La sincronizzazione dei contatti è bidirezionale. Se apporti modifiche a un contatto in Dynamics o a una persona in Marketo, i tuoi aggiornamenti si rifletteranno su entrambi i sistemi.

## Cosa succede se nello stesso campo vengono apportate modifiche contemporaneamente in entrambi i sistemi? (Collisione dati) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Anche se questo è raro, Marketo vincerà per le persone e Dynamics vincerà per i contatti. Questo perché riteniamo che il reparto marketing sia autorevole per le persone, mentre il sistema ufficiale di registrazione dei contatti è nel reparto vendite (CRM).

## Posso creare un contatto con Marketo? {#can-i-create-a-contact-using-marketo}

Sì. [Ecco come](microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md).

>[!NOTE]
>
>Quando si utilizza l’azione di flusso &quot;Sincronizza persona con Microsoft&quot; (solo in una campagna di attivazione), il lead/contatto verrà creato in tempo reale in Dynamics.

## È possibile forzare manualmente la sincronizzazione di una persona o di un contatto? {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

No, la sincronizzazione automatica in background è l&#39;unico modo per sincronizzare gli aggiornamenti tra Marketo e Dynamics. La [Sincronizza persona con Microsoft](../../../../product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) non forzerà la sincronizzazione del lead.

## Quali campi verranno sincronizzati con Marketo? {#what-fields-will-sync-to-marketo}

È possibile [selezionare i campi da sincronizzare](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) durante la configurazione. Tuttavia, Marketo sincronizzerà solo i campi a cui l&#39;utente della sincronizzazione Dynamics ha accesso.

## Marketo rispetterà le regole di convalida di Dynamics? {#will-marketo-respect-the-dynamics-validation-rules}

Sì, in caso di conflitto il risultato verrà registrato nel registro attività lead.
