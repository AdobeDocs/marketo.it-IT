---
description: Inviare un messaggio SMS Vibes - Documentazione di Marketo - Documentazione del prodotto
title: Inviare un messaggio SMS Vibes
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: d4bd94b22b4f9da993150a94d2757014cbf87d80
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---

# Inviare un messaggio SMS Vibes {#send-a-vibes-sms-message}

Hai [ha creato il messaggio Vibes SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md), ora è il momento di inviarlo. Puoi inviarlo tramite Batch o Trigger Campaign.

>[!NOTE]
>
>Durante l’invio di messaggi SMS:
>
>* Deduplicazione Marketo Engage per numero di telefono. Quindi, se più persone hanno lo stesso numero di telefono, solo una persona riceverà il messaggio se è membro di un solo elenco di abbonamenti Vibes. La deduplicazione viene eseguita a livello di elenco degli abbonamenti Vibes, non a livello di programma Marketo.
>* Marketo inserire nell&#39;elenco Bloccati non invierà a persone che sono state o Sospese dal marketing.

## Inviare un SMS in batch {#send-a-batch-sms}

1. In Il mio Marketo, fai clic su **Attività di marketing**.

   ![](assets/send-a-vibes-sms-message-1.png)

1. Trova e seleziona la campagna avanzata desiderata.

   ![](assets/send-a-vibes-sms-message-2.png)

1. Fai clic su **Elenco avanzato** e definisci il pubblico per l’SMS. In questo esempio invieremo a tutti gli utenti del nostro Database la cui azienda è indicata come &quot;Adobe&quot;.

   ![](assets/send-a-vibes-sms-message-3.png)

1. In **Flusso** , trascinare **Invia messaggio SMS**. Seleziona l’elenco Messaggi SMS e vibrazioni desiderato dai menu a discesa.

   ![](assets/send-a-vibes-sms-message-4.png)

   >[!NOTE]
   >
   >Il selettore Elenco vibrazioni funge da ulteriore filtro per il pubblico già identificato nell’Elenco avanzato in modo da eseguire il targeting solo delle persone che appartengono a tale elenco.

1. Fai clic su **Pianificazione** e pianifica l’SMS.

   ![](assets/send-a-vibes-sms-message-5.png)

## Invia un SMS di attivazione {#send-a-trigger-sms}

1. In Il mio Marketo, fai clic su **Attività di marketing**.

   ![](assets/send-a-vibes-sms-message-6.png)

1. Trova e seleziona la campagna avanzata desiderata.

   ![](assets/send-a-vibes-sms-message-7.png)

1. Fai clic su **Elenco avanzato** , selezionare il trigger desiderato e definirne il valore. In questo esempio utilizziamo **Compila modulo**.

   ![](assets/send-a-vibes-sms-message-8.png)

1. In **Flusso** , trascinare **Invia messaggio SMS**. Seleziona l’elenco Messaggi SMS e vibrazioni desiderato dai menu a discesa.

   ![](assets/send-a-vibes-sms-message-9.png)

   >[!NOTE]
   >
   >Il selettore Elenco vibrazioni funge da ulteriore filtro per il pubblico già identificato nell’Elenco avanzato in modo da eseguire il targeting solo delle persone che appartengono a tale elenco.

1. Fai clic su **Pianificazione** , quindi **Attiva**.

   ![](assets/send-a-vibes-sms-message-10.png)

>[!MORELIKETHIS]
>
>* [Creare un messaggio vibrazioni](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md)
>* Passaggi del flusso delle vibrazioni

