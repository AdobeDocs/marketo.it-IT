---
unique-page-id: 3571838
description: Microsoft Dynamics Sync -Field Sync - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione Microsoft Dynamics - Sincronizzazione campi
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---


# Sincronizzazione Microsoft Dynamics: Sincronizzazione dei campi {#microsoft-dynamics-sync-field-sync}

La sincronizzazione da Marketo a Dynamics è estremamente potente. Ecco i dettagli.

## Come vengono mantenuti sincronizzati i dettagli del campo tra i due sistemi? {#how-are-field-details-kept-in-sync-between-the-two-systems}

La sincronizzazione è bidirezionale per le entità lead e contatti. Se apporti modifiche a un lead o a un contatto in Dynamics o a una persona in Marketo, gli aggiornamenti verranno rispecchiati in entrambi i sistemi.

Per account, utenti, opportunità, team ed entità personalizzate, la sincronizzazione è unidirezionale: Dinamica a Marketo. Se apporti modifiche a queste entità in Dynamics, gli aggiornamenti verranno rispecchiati in Marketo.

## Cosa succede se contemporaneamente vengono apportate modifiche allo stesso campo in entrambi i sistemi? (Collisione dati) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Anche se questo è raro, Marketo vincerà per le persone (lead) e Dynamics vincerà per i contatti. Questo perché riteniamo che il reparto marketing sia autorevole per le persone, mentre il sistema ufficiale di registrazione dei contatti è nel reparto vendite (CRM). Per le entità di sincronizzazione unidirezionale, Dynamics vincerà sempre.

## Posso creare un campo in Dynamics utilizzando Marketo? {#can-i-create-a-field-in-dynamics-using-marketo}

No, al momento non è supportato.

## Ho creato un campo in Dynamics. Posso sincronizzarlo con Marketo? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Sì, puoi [sincronizzare il campo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) purché l’utente sincronizzato abbia accesso a esso in Dynamics.

## Quali campi verranno sincronizzati con Marketo? {#what-fields-will-sync-to-marketo}

È possibile [selezionare i campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) durante la configurazione.

## Cosa succede se devo aggiungere un campo personalizzato dopo la sincronizzazione di Marketo e Dynamics? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

Puoi aggiungere campi in qualsiasi momento e prevedere l’aggiornamento dei dati da Dynamics a Marketo. Per ulteriori informazioni, consulta [Utilizzare la sincronizzazione rapida con Microsoft Dynamics per un nuovo campo personalizzato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md) .

## Cosa succede se desidero eliminare un campo in Dynamics dopo l’aggiunta del campo alla sincronizzazione? {#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketo memorizza un riferimento ai campi da sincronizzare. Se elimini un campo in Dynamics, è consigliabile eseguire questa operazione con la funzione [sincronizzazione disabilitata](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Quindi aggiorna lo schema in Marketo modificando e salvando [Seleziona campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).