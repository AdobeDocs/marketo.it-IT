---
unique-page-id: 11379045
description: Aggiungere un passaggio di flusso per SMS - Documentazione di Marketo - Documentazione del prodotto
title: Aggiungere un passaggio di flusso per SMS
exl-id: 8e96f6ad-43c9-4d64-8cb6-241664956d72
feature: Mobile Marketing
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Aggiungere un passaggio di flusso per SMS {#add-a-flow-step-for-sms}

Marketo dispone di tre passaggi di flusso che puoi utilizzare nelle campagne SMS intelligenti:

* **Invia messaggio SMS** - Questa azione di flusso invia messaggi agli utenti dello smartlist di Marketo che sono abbonati a un elenco di abbonamenti Vibes selezionato dall’utente. Non avvia il processo di abbonamento.
* **Iscriviti all’elenco delle vibrazioni** : questa azione di flusso avvia il processo di abbonamento SMS tramite una campagna di acquisizione Vibes selezionata dall’utente. Vibes invia quindi un messaggio di conferma; il destinatario deve rispondere a esso per completare il processo di abbonamento.
* **Annulla iscrizione all’elenco delle vibrazioni** - Questa azione di flusso annulla l’abbonamento di ogni persona da un elenco di abbonamenti Vibes selezionato dall’utente.

>[!NOTE]
>
>Durante l’invio di messaggi SMS:
>
>* Deduplicazione Marketo per numero di telefono. Quindi, se più persone hanno lo stesso numero di telefono, solo una persona riceverà il messaggio.
>* Marketo inserire nell&#39;elenco Bloccati non invierà a persone che sono state o Sospese dal marketing.

Per informazioni generali sull&#39;impostazione delle fasi del flusso, vedere [Aggiungere un passaggio di flusso a una campagna avanzata](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

Di seguito sono riportate le nozioni di base sull’utilizzo degli SMS.

1. In Il mio Marketo, fai clic su **Attività di marketing**.

   ![](assets/image2016-7-28-11-3a41-3a17.png)

1. Trova la campagna intelligente a cui desideri aggiungere il flusso SMS. Fai clic su **Flusso** scheda.

   ![](assets/image2016-7-28-11-3a43-3a41.png)

1. Trascina sul flusso, ad esempio: **Invia messaggio SMS**. Seleziona il Messaggio SMS e l’elenco Vibes dai menu a discesa.

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >Il selettore Elenco vibrazioni funge da ulteriore filtro per il pubblico già identificato nell’elenco smart, in modo da eseguire il targeting solo dei lead che appartengono a tale elenco.
   >
   >Il **Iscriviti all’elenco delle vibrazioni** e **Annulla iscrizione all’elenco delle vibrazioni** i flussi hanno requisiti diversi. Per **Abbonati**, è necessario selezionare l’elenco Vibes e la campagna di acquisizione Vibes. Per **Annulla iscrizione**, è necessario solo l’elenco Vibes.
