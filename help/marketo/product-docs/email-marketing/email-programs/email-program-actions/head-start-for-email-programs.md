---
unique-page-id: 10097202
description: Head Start per i programmi e-mail - Documentazione Marketo - Documentazione del prodotto
title: Head Start per i programmi e-mail
exl-id: f7c8b082-4d83-4e3b-8aa4-7b252e3dacd3
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# Head Start per i programmi e-mail {#head-start-for-email-programs}

>[!PREREQUISITES]
>
>[Crea un programma di posta elettronica](/help/marketo/product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)

Quando scegli una data/ora per un programma e-mail, questo determina quando inizierà l’elaborazione del programma. Se desideri che le e-mail vengano avviate all’ora selezionata, Head Start offre tale opzione elaborando in anticipo il programma.

## Inizio testina standard {#standard-head-start}

1. Fai clic su **Attività di marketing**.

   ![](assets/one-1.png)

1. Trova e seleziona il programma e-mail.

   ![](assets/selectemailprogram-4.jpg)

   >[!NOTE]
   >
   >Head Start non può essere utilizzato con test A/B.

1. Nel riquadro Pianificazione, pianifica l&#39;e-mail, quindi seleziona la casella **Inizio intestazione**.

   ![](assets/three-1.png)

   Selezionando Head Start, l&#39;elaborazione del programma inizierà circa 12 ore prima dell&#39;orario previsto. Una volta avviata l’elaborazione, il programma viene bloccato.

   >[!CAUTION]
   >
   >L’e-mail verrà comunque inviata a tutti gli utenti del pubblico che annullano l’abbonamento dopo il blocco del programma. È consigliabile modificare la notifica di annullamento dell’abbonamento per riflettere il fatto che l’elaborazione degli annullamenti dell’abbonamento potrebbe richiedere 1-2 giorni lavorativi.

1. Fare clic su **Approva programma**.

   ![](assets/four-1.png)

   Dopo l’approvazione del programma, puoi visualizzare quattro stati diversi nel riquadro Approvazione.

   * **In attesa di esecuzione:** dopo l&#39;approvazione del programma.
   * **Elaborazione avviata, in attesa di esecuzione:** Elaborazione in corso.
   * **Elaborazione terminata, in attesa di esecuzione:** Elaborazione completata, e-mail in attesa dell&#39;ora pianificata per l&#39;avvio.
   * **Completato:** programma completato.

   >[!TIP]
   >
   >Vuoi annullare l’operazione dopo il blocco del programma ma prima dell’invio dell’e-mail? Nessun problema! Fai clic su **Interrompi programma** nella parte inferiore destra del riquadro Approvazione.

   >[!NOTE]
   >
   >Se annulli l’approvazione del programma e-mail con meno di 12 ore di anticipo rispetto all’ora di esecuzione pianificata, ma poi cambi idea, dovrai scegliere una nuova data/ora che preceda di almeno 12 ore l’approvazione.

## Inizio intestazione con fuso orario destinatario {#head-start-with-recipient-time-zone}

La funzione Head Start richiede un programma con almeno 12 ore di anticipo. Che cosa significa per il fuso orario del destinatario? Ricorda che quando il fuso orario del destinatario è attivo, iniziamo a eseguire il programma e-mail a mezzanotte nel fuso orario più vicino (UTC +14:00). Pertanto, per abilitare **sia** Inizio intestazione che Fuso orario destinatario, i programmi devono essere pianificati **con almeno 12 ore di anticipo rispetto al fuso orario più vicino (UTC +14:00**).

Ciò significa che se ti trovi in America/Los Angeles e desideri abilitare sia Head Start che Recipient Time Zone, devi pianificare il programma con **34 ore** di anticipo. Come siamo arrivati a questo numero?

![](assets/image2017-12-5-13-3a11-3a46.png)

[Ulteriori informazioni](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md) su come pianificare i programmi e-mail con il fuso orario del destinatario.

>[!MORELIKETHIS]
>
>* [Pianifica Il Programma Di Posta Elettronica](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/schedule-your-email-program.md)
>* [Programmazione di programmi e-mail con fuso orario destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Informazioni sul fuso orario del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
