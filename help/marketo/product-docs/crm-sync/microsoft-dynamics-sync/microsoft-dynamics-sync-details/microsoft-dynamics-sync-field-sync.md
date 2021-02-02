---
unique-page-id: 3571838
description: Microsoft Dynamics Sync -Field Sync - Marketo Docs - Documentazione prodotto
title: Microsoft Dynamics Sync - Sincronizzazione campi
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Sincronizzazione campo {#microsoft-dynamics-sync-field-sync}

La sincronizzazione tra Marketo e Dynamics è super potente. Ecco i dettagli.

## Come vengono mantenuti sincronizzati i dettagli del campo tra i due sistemi? {#how-are-field-details-kept-in-sync-between-the-two-systems}

La sincronizzazione è bidirezionale per le entità lead e contatto. Se apporti modifiche a un lead o a un contatto in Dynamics o a una persona in Marketo, gli aggiornamenti si rifletteranno su entrambi i sistemi.

Per le entità account, utente, opportunità, team e personalizzate, la sincronizzazione è unidirezionale: Dinamica a Marketo. Se apporti modifiche a queste entità in Dynamics, gli aggiornamenti si rifletteranno su Marketo.

## Cosa succede se nello stesso campo vengono apportate modifiche contemporaneamente in entrambi i sistemi? (Collisione dati) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Anche se questo è raro, Marketo vincerà per le persone (lead) e Dynamics vincerà per i contatti. Questo perché riteniamo che il reparto marketing sia autorevole per le persone, mentre il sistema ufficiale di registrazione dei contatti è nel reparto vendite (CRM). Per le entità di sincronizzazione unidirezionale, Dynamics vincerà sempre.

## Posso creare un campo in Dynamics utilizzando Marketo? {#can-i-create-a-field-in-dynamics-using-marketo}

No, al momento non è supportato.

## Ho creato un campo in Dynamics. Posso sincronizzarlo con Marketo? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Sì, è possibile [sincronizzare il campo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) purché l&#39;utente della sincronizzazione abbia accesso ad esso in Dynamics.

Quali campi verranno sincronizzati con Marketo?

È possibile [selezionare i campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) durante la configurazione.

## Cosa succede se devo aggiungere un campo personalizzato dopo che Marketo e Dynamics sono stati sincronizzati? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

Puoi aggiungere campi in qualsiasi momento e prevedere che i dati saranno aggiornati da Dynamics a Marketo. Per ulteriori informazioni, vedere [Utilizzare la sincronizzazione rapida con Microsoft Dynamics per un nuovo campo personalizzato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md).
