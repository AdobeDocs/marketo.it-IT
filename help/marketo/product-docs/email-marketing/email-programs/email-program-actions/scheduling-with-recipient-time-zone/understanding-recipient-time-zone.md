---
unique-page-id: 12983291
description: Fuso orario del destinatario - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni sul fuso orario del destinatario
exl-id: 8895241e-94c9-43a2-9158-11c1994df09b
feature: Email Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 3%

---

# Informazioni sul fuso orario del destinatario {#understanding-recipient-time-zone}

I programmi di e-mail e coinvolgimento possono essere configurati in modo da consegnare i messaggi in base ai fusi orari dei destinatari, eliminando la necessità di creare più programmi: invia una volta e Marketo conserva automaticamente l’e-mail fino all’ora locale corretta.

>[!NOTE]
>
>[!UICONTROL Recipient Time Zone] al momento funziona **solo** con contenuto e-mail. Non funzionerà per i programmi di coinvolgimento predefiniti.

## Programmi e-mail {#email-programs}

Esistono due scenari principali durante la [pianificazione di un programma di posta elettronica](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md):

1. Programmazione dell&#39;esecuzione del programma entro le 25 ore successive.
1. Pianificazione dell&#39;esecuzione futura del programma per più di 25 ore (ovvero la prossima settimana).

Per soddisfare ogni fuso orario, i programmi e-mail pianificati con [!UICONTROL Recipient Time Zone] iniziano a essere eseguiti a mezzanotte nel **primo/primo** fuso orario nel mondo (UTC +14:00).

## Programmi di coinvolgimento {#engagement-programs}

Quando [pianifichi un flusso di programma di coinvolgimento](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) e [!UICONTROL Recipient Time Zone] è attivo, il cast del programma inizia a essere eseguito a mezzanotte in UTC +14:00. È necessario pianificare il primo cast almeno 25 ore in futuro (24 ore + un po’ di tempo per avviare la campagna), perché le persone potrebbero qualificarsi per il cast in ogni fuso orario del mondo. L&#39;avvio dell&#39;elaborazione in questo momento in UTC +14:00 garantisce che l&#39;e-mail venga inviata alla data e all&#39;ora pianificate per ogni persona che si qualifica per questo cast.

## Calcolo del fuso orario {#calculating-time-zone}

Marketo calcola il fuso orario in base alla città, allo stato, al paese o al CAP di una persona. Se non siamo in grado di calcolare il fuso orario di qualcuno da questi valori, torniamo ai campi Città, Stato, Paese e CAP.

Nei casi in cui è disponibile **solo** paese o **solo** stato:

* Per i paesi con tre o meno fusi orari, viene selezionato il fuso orario intermedio.
* Per gli stati con due fusi orari, viene selezionato il primo dei due.

Se non è ancora possibile determinare il fuso orario di un utente da una combinazione di questi campi, **non** assegnerà un fuso orario e l&#39;e-mail verrà inviata in base al fuso orario dell&#39;abbonamento a Marketo. Pertanto, se il programma è pianificato per 9:00am PDT, le persone a cui non è assegnato alcun fuso orario riceveranno l’e-mail a 9:00am PDT.

>[!NOTE]
>
>Marketo ricalcola automaticamente il fuso orario di una persona quando cambia uno dei campi di input precedenti.

>[!MORELIKETHIS]
>
>* [Programmi e-mail pianificati con [!UICONTROL Recipient Time Zone]](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Inizio intestazione per programmi e-mail](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [Programmi di coinvolgimento pianificati con [!UICONTROL Recipient Time Zone]](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)
