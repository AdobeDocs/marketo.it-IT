---
unique-page-id: 12983291
description: Informazioni sul fuso orario del destinatario - Documentazione Marketo - Documentazione del prodotto
title: Informazioni sul fuso orario del destinatario
exl-id: 8895241e-94c9-43a2-9158-11c1994df09b
source-git-commit: 46812deb41ed56328a4a64fbd36340d13c50dde4
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Informazioni sul fuso orario del destinatario {#understanding-recipient-time-zone}

I programmi e-mail e di coinvolgimento possono essere configurati in modo da essere consegnati in base ai fusi orari dei destinatari, eliminando la necessità di creare più programmi: invia una volta e Marketo blocca automaticamente l’e-mail fino all’ora locale corretta.

>[!NOTE]
>
>Il fuso orario destinatario attualmente funziona **solo** con il contenuto dell&#39;e-mail. Non funzionerà per i programmi di coinvolgimento predefiniti.

## Programmi e-mail {#email-programs}

Esistono due scenari principali in cui [è in corso la pianificazione di un programma e-mail](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md):

1. Programmazione del programma da eseguire entro le prossime 25 ore.
1. Programmazione del programma in modo che venga eseguito più di 25 ore in futuro (ad esempio, la settimana successiva).

Per adattarsi a ogni fuso orario, i programmi e-mail pianificati con il fuso orario Destinatario iniziano a essere in esecuzione a mezzanotte nel fuso orario **primo/primo** del mondo (UTC +14:00).

## Programmi di coinvolgimento {#engagement-programs}

Quando [pianifichi un flusso di programmi di coinvolgimento](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) e il fuso orario destinatario è attivo, il cast del programma inizierà a partire dalla mezzanotte in UTC +14:00. Ti chiediamo di pianificare il primo cast almeno 25 ore nel futuro (24 ore + un po &#39;di tempo per avviare la campagna) perché le persone possono qualificarsi per il cast in ogni fuso orario in tutto il mondo. A partire da questa elaborazione in UTC +14:00 garantisce che l’e-mail verrà inviata alla data e all’ora pianificate per ogni persona idonea a questo cast.

## Calcolo del fuso orario {#calculating-time-zone}

Marketo calcola il fuso orario in base alla città, allo stato, al paese o al codice postale di una persona. Se non siamo in grado di calcolare il fuso orario di qualcuno in base a questi valori, torniamo ai campi Città di riferimento, Stato di provenienza, Paese di provenienza e Codice postale di provenienza.

Nei casi in cui abbiamo **solo** Paese o **solo** Stato disponibile:

* Per i paesi con tre o meno fusi orari, selezioniamo il fuso orario intermedio.
* Per gli stati con due fusi orari, selezioniamo il primo dei due.

Se non è ancora possibile determinare il fuso orario di un utente in base a una combinazione di questi campi, **non** assegneremo un fuso orario e l’e-mail verrà inviata in base al fuso orario dell’abbonamento a Marketo. Quindi, se il tuo programma è pianificato per le 9:00 PDT, le persone senza fuso orario assegnato verranno inviate l’e-mail alle 9:00 PDT.

>[!NOTE]
>
>Marketo ricalcola automaticamente il fuso orario di una persona quando uno qualsiasi dei campi di input di cui sopra cambia.

>[!MORELIKETHIS]
>
>* [Pianificare programmi e-mail con il fuso orario del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Avvio intestazione per programmi e-mail](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [Pianificazione dei programmi di coinvolgimento con il fuso orario del destinatario](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)

