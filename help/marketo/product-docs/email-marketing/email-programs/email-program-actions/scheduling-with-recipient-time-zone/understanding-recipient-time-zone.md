---
unique-page-id: 12983291
description: Fuso orario destinatario - Documenti Marketo - Documentazione prodotto
title: Informazioni sul fuso orario del destinatario
translation-type: tm+mt
source-git-commit: 8d45a28e1c2adad3e04645f7150f1757414092f0
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---


# Informazioni sul fuso orario del destinatario {#understanding-recipient-time-zone}

I programmi di e-mail e di coinvolgimento possono essere configurati per essere inviati in base ai fusi orari dei destinatari, eliminando la necessità di creare più programmi: una volta e Marketo trattengono automaticamente l&#39;e-mail fino all&#39;ora locale corretta.

>[!NOTE]
>
>Il fuso orario del destinatario attualmente funziona **solo** con il contenuto dell&#39;e-mail. Non funzionerà per i programmi di coinvolgimento predefiniti.

## Programmi e-mail {#email-programs}

Esistono due scenari principali in cui [pianificare un programma e-mail](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md):

1. Programmare l&#39;esecuzione del programma entro le prossime 25 ore.
1. Programmare l&#39;esecuzione del programma per più di 25 ore in futuro (ad esempio, la settimana successiva).

Per adattarsi a ogni fuso orario, i programmi e-mail pianificati con il fuso orario del destinatario iniziano a essere in esecuzione a mezzanotte nel fuso orario **primo/primo** del mondo (UTC +14:00).

## Programmi di coinvolgimento {#engagement-programs}

Quando [pianificate un flusso di programmi di coinvolgimento](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) e il fuso orario destinatario è attivo, il cast del programma inizierà a partire da mezzanotte all&#39;ora UTC +14:00. È necessario pianificare il primo cast per almeno 25 ore in futuro (24 ore + un po&#39; di tempo per avviare la campagna) perché le persone possono qualificarsi per il cast in ogni fuso orario del mondo. A partire da questa elaborazione in UTC +14:00 garantiamo che l&#39;e-mail verrà inviata alla data e all&#39;ora previste per ogni utente idoneo per questo cast.

## Calcolo del fuso orario {#calculating-time-zone}

Marketo calcola il fuso orario in base alla città, allo stato, al paese o al codice postale di una persona. Se non siamo in grado di calcolare il fuso orario di qualcuno in base a questi valori, torneremo ai campi Città inferta, Stato inferto, Paese ferito e Codice postale.

Nei casi in cui è disponibile **solo** Paese o **solo** Stato:

* Per i paesi con tre o meno fusi orari, selezioniamo il fuso orario intermedio.
* Per gli stati con due fusi orari, viene selezionata la prima delle due.

Se non riusciamo ancora a determinare il fuso orario di un utente da una qualsiasi combinazione di questi campi, **non** assegneremo un fuso orario e l&#39;e-mail verrà recapitata in base al fuso orario dell&#39;iscrizione di Marketo. Pertanto, se il programma è pianificato per le 9:00 PDT, le persone senza fuso orario riceveranno l&#39;e-mail alle 9:00 PDT.

>[!NOTE]
>
>Marketo ricalcola automaticamente il fuso orario di una persona quando uno dei campi di input di cui sopra cambia.

>[!MORELIKETHIS]
>
>* [Pianificazione dei programmi e-mail con il fuso orario del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Head Start for Email Programs](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)

   >
   >
* [Pianificazione dei programmi di coinvolgimento con il fuso orario del destinatario](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)

