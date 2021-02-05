---
unique-page-id: 10097202
description: Head Start for Email Programs - Marketo Docs - Documentazione prodotto
title: Head Start for Email Programs
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---


# Avvio principale per programmi e-mail {#head-start-for-email-programs}

>[!PREREQUISITES]
>
>* [Creare un programma e-mail](../../../../product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)

>



Quando si sceglie una data/ora per un programma e-mail, questo determina quando il programma inizierà l&#39;elaborazione. Se desiderate che le e-mail vengano avviate al momento selezionato, Head Start vi offre tale opzione elaborando il programma in anticipo.

## Inizio testina standard {#standard-head-start}

1. Fate clic su **Attività marketing**.

   ![](assets/one-1.png)

1. Trova e seleziona il tuo programma e-mail.

   ![](assets/selectemailprogram-4.jpg)

   >[!NOTE]
   >
   >Impossibile utilizzare Head Start con test A/B.

1. Nella sezione Pianificazione, pianificate l&#39;e-mail, quindi selezionate la casella **Inizio intestazione**.

   ![](assets/three-1.png)

   Con Head Start selezionato, il programma inizierà l&#39;elaborazione circa 12 ore prima del tempo previsto. Una volta avviata l&#39;elaborazione, il programma viene bloccato.

   >[!CAUTION]
   >
   >Chiunque dal pubblico che annulla l&#39;iscrizione dopo il blocco del programma riceverà comunque l&#39;e-mail. È consigliabile regolare la notifica di annullamento dell’iscrizione in modo da riflettere il fatto che l’elaborazione degli abbonamenti potrebbe richiedere 1-2 giorni lavorativi.

1. Fare clic su **Approva programma**.

   ![](assets/four-1.png)

   Dopo l&#39;approvazione del programma, ci sono quattro stati diversi che si possono vedere nella sezione Approvazione.

   * **Attesa dell&#39;esecuzione:** dopo l&#39;approvazione del programma.
   * **Elaborazione avviata, in attesa di esecuzione:** Elaborazione in corso.
   * **Elaborazione completata, in attesa di esecuzione:** Elaborazione completata, ora l&#39;e-mail è in attesa dell&#39;ora pianificata per l&#39;avvio.
   * **Finito:** Programma completato.

   >[!TIP]
   >
   >Vuoi annullare dopo che il programma si blocca ma prima che l&#39;e-mail invia? Nessun problema! Fare clic su **Interrompi programma** in basso a destra nella sezione Approvazione.

   >[!NOTE]
   >
   >Se non approvi il tuo programma e-mail con meno di 12 ore prima del suo orario di esecuzione pianificato, ma poi cambi idea, dovrai scegliere una nuova data/ora che sia almeno 12 ore prima di quando lo approvi.

## Inizio intestazione con fuso orario destinatario {#head-start-with-recipient-time-zone}

La funzione Head Start richiede che il programma sia pianificato almeno con 12 ore di anticipo. Cosa significa questo per il fuso orario del destinatario? Ricorda che quando il fuso orario del destinatario è attivo, il programma e-mail inizia a essere eseguito a mezzanotte nel primo fuso orario (UTC +14:00). Pertanto, per abilitare **sia** Head Start che Recipient Time Zone, i programmi devono essere programmati **almeno 12 ore prima del fuso orario precedente (UTC +14:00**).

Ciò significa che se siete in America/Los Angeles e desiderate attivare sia Head Start che Recipient Time Zone, è necessario pianificare il programma **34 ore** in anticipo. Come siamo arrivati a questo numero?

![](assets/image2017-12-5-13-3a11-3a46.png)

[Scopri ](scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md) di più su come pianificare programmi e-mail con il fuso orario del destinatario.

>[!MORELIKETHIS]
>
>* [Pianificazione del programma e-mail](schedule-your-email-program.md)
>* [Pianificazione dei programmi e-mail con il fuso orario del destinatario](scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Informazioni sul fuso orario del destinatario](scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)

>



