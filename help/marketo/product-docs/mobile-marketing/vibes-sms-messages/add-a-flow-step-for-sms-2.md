---
description: Aggiungere un passaggio di flusso per SMS - Documentazione di Marketo - Documentazione del prodotto
title: Aggiungere un passaggio di flusso per SMS
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Aggiungere un passaggio di flusso per SMS {#add-a-flow-step-for-sms}

Marketo Engage dispone di tre passaggi di flusso che puoi utilizzare nelle campagne SMS Smart:

<table>
<tbody>
  <tr>
    <td style="width:25%">Invia messaggio SMS</td>
    <td>Questa azione di flusso invia messaggi agli utenti di Marketo Smart List che sono abbonati a un elenco di abbonamenti Vibes con consenso dell’utente. Non avvia il processo di abbonamento. <a href="/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-a-vibes-sms-message.md">Ulteriori informazioni</a>.</td>
  </tr>

<tr>
    <td style="width:25%">Iscriviti all’elenco delle vibrazioni</td>
    <td>Questa azione di flusso avvia il processo di abbonamento SMS tramite una campagna di acquisizione Vibes selezionata dall’utente. Vibes invia quindi un messaggio di conferma e il destinatario deve rispondere con "Y" entro 24 ore per confermare l’opt-in. Una volta che l’utente ha acconsentito, diventerà membro dell’elenco di iscrizioni Vibes associato.</td>
  </tr>
  <tr>
    <td style="width:25%">Annulla iscrizione all’elenco delle vibrazioni</td>
    <td>Questa azione di flusso annulla l’abbonamento di ogni persona da un elenco di abbonamenti Vibes con consenso esplicito dell’utente. Quando un utente scrive "STOP" al codice, il record della persona viene aggiornato per indicare che non è più membro dell’elenco di abbonamento a Vibes.</td>
  </tr>
  </tbody>
</table>

>[!NOTE]
>
>Durante l’invio di messaggi SMS:
>
>* Deduplicazione Marketo per numero di telefono. Quindi, se più persone hanno lo stesso numero di telefono, solo una persona riceverà il messaggio se è membro di un solo elenco di abbonamenti Vibes. La deduplicazione viene eseguita a livello di elenco degli abbonamenti Vibes, non a livello di programma Marketo.
>* Marketo inserire nell&#39;elenco Bloccati non invierà a persone che sono state o Sospese dal marketing.

Per informazioni generali sulla configurazione dei passaggi di flusso, vedere [Aggiungere un passaggio di flusso a una campagna avanzata](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

Di seguito sono riportate le nozioni di base sull’utilizzo degli SMS.

1. In Il mio Marketo, fai clic su **Attività di marketing**.

   ![](assets/add-a-flow-step-for-sms-1.png)

1. Trova e seleziona la campagna avanzata a cui desideri aggiungere il flusso SMS.

   SCHERMATA

1. Nella scheda Elenco avanzato, scegli i trigger desiderati (ad esempio, &quot;Modulo compilato&quot;).

   SCHERMATA

1. Nella scheda **Flusso**, trascina il passaggio del flusso (ad esempio, **Invia messaggio SMS**). Seleziona il Messaggio SMS e l’elenco Vibes dai menu a discesa.

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >Il selettore Elenco vibrazioni funge da ulteriore filtro per il pubblico già identificato nell’elenco smart, in modo da eseguire il targeting solo dei lead che appartengono a tale elenco.
   >
   >I flussi **Abbonati all&#39;elenco delle vibrazioni** e **Annulla abbonamento all&#39;elenco delle vibrazioni** hanno requisiti diversi. Per **Abbonati**, devi selezionare l&#39;elenco Vibes e la campagna di acquisizione Vibes. Per **Annulla sottoscrizione**, è necessario solo l&#39;elenco Vibes.
