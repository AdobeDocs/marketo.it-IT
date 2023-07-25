---
unique-page-id: 3571838
description: Sincronizzazione Microsoft Dynamics - Sincronizzazione campi - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione Microsoft Dynamics - Sincronizzazione campi
exl-id: 78eef0eb-4086-45c5-bce3-a3399016f228
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Sincronizzazione Microsoft Dynamics: Sincronizzazione campi {#microsoft-dynamics-sync-field-sync}

La sincronizzazione tra Marketo e Dynamics è estremamente potente. Ecco i dettagli.

## In che modo i dettagli dei campi vengono mantenuti sincronizzati tra i due sistemi? {#how-are-field-details-kept-in-sync-between-the-two-systems}

La sincronizzazione è bidirezionale per le entità lead e contatto. Se apporti modifiche a un lead o a un contatto in Dynamics o a una persona in Marketo, gli aggiornamenti verranno applicati a entrambi i sistemi.

Per account, utente, opportunità, team ed entità personalizzate, la sincronizzazione è unidirezionale: da Dynamics a Marketo. Se apporti modifiche a queste entità in Dynamics, i tuoi aggiornamenti si rifletteranno in Marketo.

## Cosa succede se vengono apportate modifiche allo stesso campo in entrambi i sistemi contemporaneamente? (Conflitto di dati) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Anche se si tratta di una situazione rara, Marketo vincerà per le persone (lead) e Dynamics vincerà per i contatti. Questo perché consideriamo il reparto marketing come autorevole per le persone, mentre il sistema ufficiale di registrazione per i contatti è nel reparto vendite (CRM). Per le entità di sincronizzazione unidirezionale, Dynamics vincerà sempre.

## È possibile creare un campo in Dynamics utilizzando Marketo? {#can-i-create-a-field-in-dynamics-using-marketo}

No, al momento non è supportato.

## Ho creato un campo in Dynamics. Posso sincronizzarlo con Marketo? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Sì, è possibile [sincronizza il campo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) purché l’utente che esegue la sincronizzazione vi abbia accesso in Dynamics.

## Quali campi verranno sincronizzati con Marketo? {#what-fields-will-sync-to-marketo}

È possibile [seleziona i campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) durante l&#39;installazione.

## Cosa succede se devo aggiungere un campo personalizzato dopo la sincronizzazione di Marketo e Dynamics? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

Puoi aggiungere campi in qualsiasi momento e aspettarti che i dati vengano aggiornati da Dynamics a Marketo. Consulta [Utilizzare la sincronizzazione rapida con Microsoft Dynamics per un nuovo campo personalizzato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md) per i dettagli.

## Cosa succede se voglio eliminare un campo in Dynamics dopo che il campo è stato aggiunto per la sincronizzazione? {#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketo memorizza un riferimento ai campi da sincronizzare. Se elimini un campo in Dynamics, è consigliabile eseguire questa operazione con [sincronizzazione disabilitata](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Quindi aggiorna lo schema in Marketo modificando e salvando il file [Seleziona campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).
