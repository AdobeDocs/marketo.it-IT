---
unique-page-id: 11379045
description: Aggiungere un passaggio di flusso per SMS - Documenti Marketo - Documentazione del prodotto
title: Aggiungere un passaggio di flusso per SMS
exl-id: 8e96f6ad-43c9-4d64-8cb6-241664956d72
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Aggiungere un passaggio di flusso per SMS {#add-a-flow-step-for-sms}

Marketo dispone di tre passaggi di flusso da utilizzare nelle campagne smart SMS:

* **Invia messaggio SMS** - Questa azione di flusso invia messaggi alle persone dell’elenco di smartlist Marketo abbonate a un elenco di sottoscrizioni Vibes selezionato dall’utente. Non avvia il processo di abbonamento.
* **Iscriviti all’elenco Vibes** - Questa azione di flusso avvia il processo di abbonamento SMS tramite una campagna di acquisizione Vibes selezionata dall’utente. Vibes invia quindi un messaggio di conferma; il destinatario deve rispondere per completare il processo di abbonamento.
* **Annulla iscrizione a Vibes List** - Questa azione di flusso annulla l’iscrizione di ogni persona da un elenco di sottoscrizioni Vibes selezionato dall’utente.

>[!NOTE]
>
>Quando si inviano messaggi SMS:
>
>* Marketo si deduplica per numero di telefono. Quindi, se più persone hanno lo stesso numero di telefono, solo una persona riceverà il messaggio.
>* Marketo non invierà a persone inserire nell&#39;elenco Bloccati o sospese dal marketing.


Per informazioni generali sulla configurazione dei passaggi di flusso, vedi [Aggiungere un passaggio di flusso a una campagna avanzata](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

Di seguito sono riportate le nozioni di base per l’utilizzo di SMS.

1. In My Marketo, fai clic su **Attività di marketing**.

   ![](assets/image2016-7-28-11-3a41-3a17.png)

1. Trova la campagna intelligente a cui desideri aggiungere il flusso SMS. Fai clic sul pulsante **Flusso** scheda .

   ![](assets/image2016-7-28-11-3a43-3a41.png)

1. Trascina il cursore sul flusso, ad esempio **Invia messaggio SMS**. Seleziona il messaggio SMS e l’elenco Vibes dal menu a discesa.

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >Il selettore Elenco variabili funge da ulteriore filtro per il pubblico già identificato nell’elenco avanzato, in modo da eseguire il targeting solo per i lead che appartengono a tale elenco Vibes.
   >
   >La **Iscriviti all’elenco Vibes** e **Annulla iscrizione a Vibes List** i flussi hanno requisiti diversi. Per **Abbonati**, devi selezionare l’elenco Vibes e la campagna di acquisizione Vibes . Per **Annulla sottoscrizione**, è necessario solo l’elenco Vibes .
