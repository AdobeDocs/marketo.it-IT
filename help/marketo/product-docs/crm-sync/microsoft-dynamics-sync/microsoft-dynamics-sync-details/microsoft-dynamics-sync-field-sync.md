---
unique-page-id: 3571838
description: Sincronizzazione Microsoft Dynamics - Sincronizzazione campi - Documentazione Marketo - Documentazione del prodotto
title: Sincronizzazione Microsoft Dynamics - Sincronizzazione campi
exl-id: 78eef0eb-4086-45c5-bce3-a3399016f228
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# Sincronizzazione [!DNL Microsoft Dynamics]: Sincronizzazione campi {#microsoft-dynamics-sync-field-sync}

La sincronizzazione tra Marketo e [!DNL Dynamics] è estremamente potente. Ecco i dettagli.

## In che modo i dettagli dei campi vengono mantenuti sincronizzati tra i due sistemi? {#how-are-field-details-kept-in-sync-between-the-two-systems}

La sincronizzazione è bidirezionale per le entità lead e contatto. Se si apportano modifiche a un lead o a un contatto in [!DNL Dynamics] o a una persona in Marketo, gli aggiornamenti verranno applicati a entrambi i sistemi.

Per account, utente, opportunità, team ed entità personalizzate, la sincronizzazione è unidirezionale: [!DNL Dynamics] a Marketo. Se si apportano modifiche a queste entità in [!DNL Dynamics], gli aggiornamenti verranno rispecchiati in Marketo.

## Cosa succede se vengono apportate modifiche allo stesso campo in entrambi i sistemi contemporaneamente? (Conflitto di dati) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Anche se si tratta di una situazione rara, Marketo vincerà per le persone (lead) e [!DNL Dynamics] per i contatti. Questo perché consideriamo il reparto marketing come autorevole per le persone, mentre il sistema ufficiale di registrazione per i contatti è nel reparto vendite (CRM). Per le entità di sincronizzazione unidirezionale, [!DNL Dynamics] vincerà sempre.

## È possibile creare un campo in [!DNL Dynamics] utilizzando Marketo? {#can-i-create-a-field-in-dynamics-using-marketo}

No, al momento non è supportato.

## Ho creato un campo in [!DNL Dynamics]. Posso sincronizzarlo con Marketo? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Sì, puoi [sincronizzare il campo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) se l&#39;utente di sincronizzazione ha accesso a esso in [!DNL Dynamics].

## Quali campi verranno sincronizzati con Marketo? {#what-fields-will-sync-to-marketo}

È possibile [selezionare i campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} durante l&#39;installazione.

## Cosa succede se devo aggiungere un campo personalizzato dopo la sincronizzazione di Marketo e [!DNL Dynamics]? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

È possibile aggiungere campi in qualsiasi momento e si prevede che i dati vengano aggiornati da [!DNL Dynamics] a Marketo. Per ulteriori dettagli, vedere [Utilizzare la sincronizzazione rapida con [!DNL Microsoft Dynamics] per un nuovo campo personalizzato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md).

## Cosa succede se si desidera eliminare un campo in [!DNL Dynamics] dopo che il campo è stato aggiunto per la sincronizzazione? {#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketo memorizza un riferimento ai campi da sincronizzare. Se elimini un campo in [!DNL Dynamics], è consigliabile eliminare [sync disabilitato](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Quindi aggiorna lo schema in Marketo modificando e salvando [Seleziona campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).
