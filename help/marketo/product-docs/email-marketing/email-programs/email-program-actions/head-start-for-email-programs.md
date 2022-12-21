---
unique-page-id: 10097202
description: Avvio principale per i programmi e-mail - Marketo Docs - Documentazione del prodotto
title: Avvio intestazione per programmi e-mail
exl-id: f7c8b082-4d83-4e3b-8aa4-7b252e3dacd3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Avvio intestazione per programmi e-mail {#head-start-for-email-programs}

>[!PREREQUISITES]
>
>[Creare un programma e-mail](/help/marketo/product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)

Quando scegli una data/ora per un programma e-mail, determina quando il programma inizierà l’elaborazione. Se desideri che le e-mail vengano lanciate al momento selezionato, Avvia intestazione ti offre tale opzione elaborando il programma in anticipo.

## Inizio testina standard {#standard-head-start}

1. Fai clic su **Attività di marketing**.

   ![](assets/one-1.png)

1. Trova e seleziona il tuo programma e-mail.

   ![](assets/selectemailprogram-4.jpg)

   >[!NOTE]
   >
   >Impossibile utilizzare l&#39;avvio dell&#39;intestazione con il test A/B.

1. Nella sezione Pianifica , pianifica l’e-mail e seleziona la **Inizio testina** scatola.

   ![](assets/three-1.png)

   Selezionando l&#39;opzione Avvio testa, il programma inizierà l&#39;elaborazione circa 12 ore prima dell&#39;orario previsto. Una volta avviata l&#39;elaborazione, il programma viene bloccato.

   >[!CAUTION]
   >
   >Chiunque dal tuo pubblico annulli l’iscrizione dopo il blocco del programma riceverà comunque l’e-mail. È consigliabile regolare la notifica di annullamento dell’abbonamento in modo che rifletta che l’elaborazione degli abbonamenti potrebbe richiedere 1-2 giorni lavorativi.

1. Fai clic su **Approva programma**.

   ![](assets/four-1.png)

   Dopo l&#39;approvazione del programma, è possibile visualizzare quattro stati diversi nella sezione Approvazione.

   * **In attesa di esecuzione:** Dopo l&#39;approvazione del programma.
   * **Elaborazione avviata, in attesa di esecuzione:** Elaborazione in corso.
   * **Elaborazione completata, in attesa di esecuzione:** Elaborazione completata. Ora e-mail in attesa dell’ora pianificata per l’avvio.
   * **Completato:** Programma completato.

   >[!TIP]
   >
   >Vuoi annullare dopo che il programma si blocca ma prima dell&#39;invio dell&#39;e-mail? Nessun problema! Fai clic su **Programma di interruzione** in basso a destra della sezione Approvazione.

   >[!NOTE]
   >
   >Se disapprovi il tuo programma e-mail con meno di 12 ore prima del suo orario di esecuzione pianificato, ma poi cambi idea, dovrai scegliere una nuova data/ora che sia almeno 12 ore prima di quando lo approvi.

## Inizia con il fuso orario del destinatario {#head-start-with-recipient-time-zone}

La funzionalità Head Start esistente richiede che il programma sia programmato almeno con 12 ore di anticipo. Cosa significa questo per il fuso orario del destinatario? Ricorda che quando il fuso orario del destinatario è attivo, il programma e-mail inizia a essere eseguito a mezzanotte nel primo fuso orario (UTC +14:00). Quindi, per **entrambi** Start di testa e fuso orario destinatario, i programmi devono essere pianificati **almeno 12 ore prima del primo fuso orario (UTC +14:00**.)

Ciò significa che se sei in America/Los Angeles e vuoi abilitare sia Head Start che Recipient Time Zone, devi pianificare il programma **34 ore** in anticipo. Come siamo arrivati a questo numero?

![](assets/image2017-12-5-13-3a11-3a46.png)

[Ulteriori informazioni](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md) informazioni su come pianificare i programmi e-mail con il fuso orario destinatario.

>[!MORELIKETHIS]
>
>* [Programma e-mail](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/schedule-your-email-program.md)
>* [Pianificare programmi e-mail con il fuso orario del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Informazioni sul fuso orario del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)

