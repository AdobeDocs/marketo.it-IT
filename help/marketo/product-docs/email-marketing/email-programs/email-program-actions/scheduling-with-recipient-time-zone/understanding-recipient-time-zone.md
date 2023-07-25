---
unique-page-id: 12983291
description: Fuso orario del destinatario - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni sul fuso orario del destinatario
exl-id: 8895241e-94c9-43a2-9158-11c1994df09b
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Informazioni sul fuso orario del destinatario {#understanding-recipient-time-zone}

I programmi di e-mail e coinvolgimento possono essere configurati per essere consegnati in base ai fusi orari dei destinatari, eliminando la necessità di creare più programmi: invia una volta e Marketo conserva automaticamente l’e-mail fino all’ora locale corretta.

>[!NOTE]
>
>Il fuso orario del destinatario attualmente funziona **solo** con contenuti e-mail. Non funzionerà per i programmi di coinvolgimento predefiniti.

## Programmi e-mail {#email-programs}

Esistono due scenari principali quando [pianificazione di un programma e-mail](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md):

1. Programmazione dell&#39;esecuzione del programma entro le 25 ore successive.
1. Pianificazione dell&#39;esecuzione futura del programma per più di 25 ore (ad esempio, la prossima settimana).

Per soddisfare ogni fuso orario, i programmi e-mail pianificati con il fuso orario del destinatario iniziano a essere eseguiti a mezzanotte nel **primo/primo** il fuso orario nel mondo (UTC +14:00).

## Programmi di coinvolgimento {#engagement-programs}

Quando [pianificare un flusso di programma di coinvolgimento](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) e Recipient Time Zone è attivo, il cast del programma inizierà a essere eseguito a mezzanotte (UTC) +14:00. È necessario pianificare il primo cast almeno 25 ore in futuro (24 ore + un po’ di tempo per avviare la campagna), perché le persone potrebbero qualificarsi per il cast in ogni fuso orario del mondo. L’avvio dell’elaborazione in questo momento in UTC +14:00 garantisce l’invio dell’e-mail alla data e all’ora pianificate per ogni persona qualificata per questo cast.

## Calcolo del fuso orario {#calculating-time-zone}

Marketo calcola il fuso orario in base alla città, allo stato, al paese o al CAP di una persona. Se non siamo in grado di calcolare il fuso orario di qualcuno da questi valori, torniamo ai campi Città, Stato, Paese e CAP.

Nei casi in cui **solo** Paese o **solo** Stato disponibile:

* Per i paesi con tre o meno fusi orari, viene selezionato il fuso orario intermedio.
* Per gli stati con due fusi orari, viene selezionato il primo dei due.

Se non siamo ancora in grado di determinare il fuso orario di qualcuno da qualsiasi combinazione di questi campi, **non** assegna un fuso orario e l’e-mail verrà inviata in base al fuso orario dell’abbonamento a Marketo. Quindi, se il programma è pianificato per le 9:00 PDT, alle persone a cui non è assegnato alcun fuso orario verrà inviata l’e-mail alle 9:00 PDT.

>[!NOTE]
>
>Marketo ricalcola automaticamente il fuso orario di una persona quando cambia uno dei campi di input precedenti.

>[!MORELIKETHIS]
>
>* [Pianificazione dei programmi e-mail con fuso orario del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Head Start per i programmi e-mail](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [Programmi di pianificazione del coinvolgimento con fuso orario del destinatario](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)
