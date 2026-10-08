---
unique-page-id: 12983291
description: Scopri come pianificare il fuso orario dei destinatari per i programmi e-mail. Consegna le e-mail alla stessa ora locale per ogni destinatario.
title: Informazioni sul fuso orario del destinatario
exl-id: 8895241e-94c9-43a2-9158-11c1994df09b
feature: Email Programs
TQID: 'https://experienceleague.adobe.com/KAj3dO4Md7Zel5SqR4m2OrTjp93ZD735gNWWRinNV5k'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
    internal-label: Programs
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: c0f0afc1-a5a8-4b01-8b43-cc38f9169499
    internal-label: Email programs
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '399'
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

Quando [pianifichi un flusso di programma di coinvolgimento](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) e [!UICONTROL Recipient Time Zone] è attivo, il cast del programma inizia a essere eseguito a mezzanotte in UTC +14:00. È necessario pianificare il primo cast almeno 25 ore in futuro (24 ore + un po’ di tempo per avviare la campagna), perché le persone potrebbero qualificarsi per il cast in ogni fuso orario del mondo. L’elaborazione in questo momento in UTC +14:00 garantisce che l’e-mail venga inviata alla data e all’ora pianificate per ogni persona qualificata per questo cast.

## Calcolo del fuso orario {#calculating-time-zone}

Marketo calcola il fuso orario in base alla città, allo stato, al paese o al CAP di una persona. Se non siamo in grado di calcolare il fuso orario di qualcuno da questi valori, torniamo ai campi Città, Stato, Paese e CAP.

Nei casi in cui è disponibile **solo** paese o **solo** stato:

* Per i paesi con tre o meno fusi orari, viene selezionato il fuso orario intermedio.
* Per gli stati con due fusi orari, viene selezionato il primo dei due.

Se non è ancora possibile determinare il fuso orario di un utente da una combinazione di questi campi, **non** assegnerà un fuso orario e l&#39;e-mail verrà inviata in base al fuso orario dell&#39;abbonamento a Marketo. Quindi, se il programma è pianificato per le 9:00 PDT, alle persone a cui non è assegnato alcun fuso orario verrà inviata l’e-mail alle 9:00 PDT.

>[!NOTE]
>
>Marketo ricalcola automaticamente il fuso orario di una persona quando cambia uno dei campi di input precedenti.

>[!MORELIKETHIS]
>
>* [Programmi e-mail pianificati con [!UICONTROL Recipient Time Zone]](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Inizio intestazione per programmi e-mail](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [Programmi di coinvolgimento pianificati con [!UICONTROL Recipient Time Zone]](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)
