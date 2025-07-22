---
unique-page-id: 3571848
description: Sincronizzazione Microsoft Dynamics - Sincronizzazione lead - Documentazione Marketo - Documentazione del prodotto
title: Sincronizzazione Microsoft Dynamics - Sincronizzazione lead
exl-id: ea04a039-32f7-41f9-85fb-18df8e236390
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# Sincronizzazione [!DNL Microsoft Dynamics]: Sincronizzazione lead {#microsoft-dynamics-sync-lead-sync}

La sincronizzazione tra Marketo e [!DNL Dynamics] è estremamente potente. Ecco i dettagli:

## Come vengono mantenuti sincroni i dettagli tra i due sistemi? {#how-are-details-kept-in-sync-between-the-two-systems}

La sincronizzazione è bidirezionale. Se si apportano modifiche a un lead in [!DNL Dynamics] o a una persona in Marketo, l&#39;aggiornamento verrà applicato a entrambi i sistemi.

>[!NOTE]
>
>Le eliminazioni non sempre si sincronizzano automaticamente in entrambe le direzioni. Vedere [Eliminazione di un lead o di un contatto](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md){target="_blank"}.

## Cosa succede se vengono apportate modifiche allo stesso campo in entrambi i sistemi contemporaneamente? (Conflitto di dati) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Anche se si tratta di una situazione rara, Marketo vincerà per le persone (lead) e [!DNL Dynamics] per i contatti. Questo perché consideriamo il reparto marketing come autorevole per le persone, mentre il sistema ufficiale di registrazione per i contatti è nel reparto vendite (CRM).

## Posso creare un lead in [!DNL Dynamics] utilizzando Marketo? {#can-i-create-a-lead-in-dynamics-using-marketo}

Sì, utilizza l&#39;azione di flusso [[!UICONTROL Sync Person to Microsoft]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md). Questo creerà un lead in [!DNL Dynamics] se il lead non esiste. Se il lead esiste, il passaggio di flusso non eseguirà alcuna azione.

>[!NOTE]
>
>Quando si utilizza l&#39;azione di flusso &quot;[!UICONTROL Sync Person to Microsoft]&quot; (solo in una campagna trigger), il lead/contatto verrà creato in tempo reale in [!DNL Dynamics].

## È possibile forzare manualmente la sincronizzazione di una persona da Marketo a un lead in [!DNL Dynamics]? {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

No, la sincronizzazione automatica in background è l&#39;unico modo per sincronizzare gli aggiornamenti tra Marketo e [!DNL Dynamics]. L&#39;azione di flusso [[!UICONTROL Sync Person to Microsoft]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) non forzerà la sincronizzazione del lead.

## Quali campi verranno sincronizzati con Marketo? {#what-fields-will-sync-to-marketo}

È possibile [selezionare i campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} durante l&#39;installazione.

## Marketo rispetterà le regole di convalida [!DNL Dynamics]? {#will-marketo-respect-the-dynamics-validation-rules}

Sì.  La sincronizzazione non riuscirà se il formato dei dati non è corretto o se mancano le informazioni richieste sul campo. In questo caso, Marketo registrerà il risultato nel registro attività della persona.
