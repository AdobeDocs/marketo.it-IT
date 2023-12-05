---
description: Aggiungere un passaggio di flusso per SMS - Documentazione di Marketo - Documentazione del prodotto
title: Aggiungere un passaggio di flusso per SMS
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: cd09ad43c08855af63131aa385c4fd406c963926
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# Aggiungere un passaggio di flusso per SMS {#add-a-flow-step-for-sms}

Il Marketo Engage dispone di tre passaggi di flusso che puoi utilizzare nelle campagne SMS Smart:

* **Invia messaggio SMS** - Questa azione di flusso invia messaggi agli utenti iscritti a un elenco di iscrizioni Vibes con consenso esplicito di Marketo Smart List. Non avvia il processo di abbonamento.
* **Iscriviti all’elenco delle vibrazioni** : questa azione di flusso avvia il processo di abbonamento SMS tramite una campagna di acquisizione Vibes selezionata dall’utente. Vibes invia quindi un messaggio di conferma; il destinatario deve rispondere &quot;Y&quot; per confermare l’opt-in entro 24 ore. Una volta che l’utente ha acconsentito, diventerà membro dell’elenco di iscrizioni Vibes associato.
* **Annulla iscrizione all’elenco delle vibrazioni** : questa azione di flusso annulla l’abbonamento di ogni persona da un elenco di abbonamenti Vibes con consenso esplicito dell’utente. Quando un utente scrive &quot;stop&quot; al codice, il record della persona viene aggiornato per indicare che non è più membro dell’elenco di abbonamento a Vibes.

>[!NOTE]
>
>Durante l’invio di messaggi SMS:
>
>* Deduplicazione Marketo per numero di telefono. Quindi, se più persone hanno lo stesso numero di telefono, solo una persona riceverà il messaggio se è membro di un solo elenco di abbonamenti Vibes. La deduplicazione viene eseguita a livello di elenco degli abbonamenti Vibes, non a livello di programma Marketo.
>* Marketo inserire nell&#39;elenco Bloccati non invierà a persone che sono state o Sospese dal marketing.

Per informazioni generali sull&#39;impostazione delle fasi del flusso, vedere [Aggiungere un passaggio di flusso a una campagna avanzata](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

Di seguito sono riportate le nozioni di base sull’utilizzo degli SMS.

1. In Il mio Marketo, fai clic su **Attività di marketing**.

   ![](assets/add-a-flow-step-for-sms-1.png)

1. Trova e seleziona la campagna avanzata a cui desideri aggiungere il flusso SMS.

   SCHERMATA

1. Nella scheda Elenco avanzato, scegli i trigger desiderati (ad esempio, &quot;Modulo compilato&quot;).

   SCHERMATA

1. In **Flusso** , trascina sul passaggio del flusso (ad es. **Invia messaggio SMS**). Seleziona il Messaggio SMS e l’elenco Vibes dai menu a discesa.

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >Il selettore Elenco vibrazioni funge da ulteriore filtro per il pubblico già identificato nell’elenco smart, in modo da eseguire il targeting solo dei lead che appartengono a tale elenco.
   >
   >Il **Iscriviti all’elenco delle vibrazioni** e **Annulla iscrizione all’elenco delle vibrazioni** i flussi hanno requisiti diversi. Per **Abbonati**, è necessario selezionare l’elenco Vibes e la campagna di acquisizione Vibes. Per **Annulla iscrizione**, è necessario solo l’elenco Vibes.
