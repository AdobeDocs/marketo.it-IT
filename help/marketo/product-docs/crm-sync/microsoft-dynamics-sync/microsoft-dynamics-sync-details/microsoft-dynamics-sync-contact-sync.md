---
unique-page-id: 3571833
description: Sincronizzazione Microsoft Dynamics - Sincronizzazione contatti - Documentazione Marketo - Documentazione del prodotto
title: Sincronizzazione Microsoft Dynamics - Sincronizzazione contatti
exl-id: d4583ea0-2b52-415e-b28c-a8eafebeff64
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Sincronizzazione [!DNL Microsoft Dynamics]: Sincronizzazione contatti {#microsoft-dynamics-sync-contact-sync}

Lo sapevi che Marketo sincronizza l&#39;intero database con [!DNL Dynamics]? Si sincronizza, poi aspetta 5 minuti e poi si sincronizza di nuovo, tutto il giorno, ogni giorno. Ecco alcuni dettagli su come Marketo tratta in modo specifico i contatti di [!DNL Dynamics].

## Come vengono mantenuti sincroni i dettagli tra i due sistemi? {#how-are-details-kept-in-sync-between-the-two-systems}

La sincronizzazione dei contatti è bidirezionale. Se si apportano modifiche a un contatto in [!DNL Dynamics] o a una persona in Marketo, gli aggiornamenti verranno applicati a entrambi i sistemi.

## Cosa succede se vengono apportate modifiche allo stesso campo in entrambi i sistemi contemporaneamente? (Conflitto di dati) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Anche se si tratta di un fenomeno raro, Marketo vincerà per le persone e [!DNL Dynamics] per i contatti. Questo perché consideriamo il reparto marketing come autorevole per le persone, mentre il sistema ufficiale di registrazione per i contatti è nel reparto vendite (CRM).

## Posso creare un contatto con Marketo? {#can-i-create-a-contact-using-marketo}

Sì.  [Ecco come](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md){target="_blank"}.

>[!NOTE]
>
>Quando si utilizza l&#39;azione di flusso &quot;Sincronizza persona con Microsoft&quot; (solo in una campagna di attivazione), il lead/contatto verrà creato in tempo reale in [!DNL Dynamics].

## È possibile forzare manualmente la sincronizzazione di una persona o di un contatto? {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

No, la sincronizzazione automatica in background è l&#39;unico modo per sincronizzare gli aggiornamenti tra Marketo e [!DNL Dynamics]. [Sincronizza persona con Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) non forzerà la sincronizzazione del lead.

## Quali campi verranno sincronizzati con Marketo? {#what-fields-will-sync-to-marketo}

È possibile [selezionare i campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) durante l&#39;installazione. Ma Marketo sincronizzerà solo i campi a cui l&#39;utente di sincronizzazione [!DNL Dynamics] ha accesso.

## Marketo rispetterà le regole di convalida [!DNL Dynamics]? {#will-marketo-respect-the-dynamics-validation-rules}

Sì, se si verifica un conflitto, il risultato verrà registrato nel registro attività lead.
