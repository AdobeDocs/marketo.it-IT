---
unique-page-id: 12982903
description: Pianificazione dei programmi e-mail con fuso orario del destinatario - Documentazione di Marketo - Documentazione del prodotto
title: Pianificazione dei programmi e-mail con fuso orario del destinatario
exl-id: d0c3f3c1-9f21-4081-818d-7c5cb1766915
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# Pianificazione dei programmi e-mail con fuso orario del destinatario {#schedule-email-programs-with-recipient-time-zone}

Esistono due possibili scenari quando si pianifica un programma e-mail quando il fuso orario del destinatario è abilitato:

1. Programmazione dell&#39;esecuzione del programma **entro** le prossime 25 ore
1. Programmazione dell&#39;esecuzione del programma **altro** più di 25 ore nel futuro (cioè la prossima settimana)

## Scenario 1: entro 25 ore {#scenario-within-hours}

Supponiamo che tu approvi un programma e-mail con il Fuso orario del destinatario abilitato e un orario di consegna pianificato entro le prossime 25 ore. Potresti avere persone nella tua lista intelligente che vivono in fusi orari in cui l’ora pianificata è già passata.

In questo scenario, possiamo decidere cosa fare con questo sottoinsieme di persone qualificate. Fai clic sull’icona a forma di ingranaggio accanto a **Fuso orario destinatario** nel **Pianificazione** sezione del programma e-mail.

![](assets/image2017-12-5-10-3a46-3a42.png)

Questo offre due opzioni:

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**Definizione**
>
>* **Consegna il giorno successivo nel fuso orario del destinatario**: se l’e-mail è programmata per essere inviata martedì alle 9:00, le persone qualificate che vivono in fusi orari in cui l’ora pianificata è già passata riceveranno l’e-mail il *Mercoledì* alle 9.
>
>* **Consegna in base all’ora predefinita del programma**: se l’e-mail è programmata per essere inviata martedì alle 9, l’e-mail verrà inviata a persone qualificate che vivono in fusi orari in cui l’orario pianificato è già stato superato _in base alle impostazioni del fuso orario della sottoscrizione_. Quindi, se [impostazioni del fuso orario dell’abbonamento](/help/marketo/product-docs/administration/settings/select-your-language-locale-and-time-zone.md) sono impostati su PDT America/Los Angeles, questi destinatari riceveranno comunque l’e-mail martedì alle 9:00 PDT (a prescindere dall’ora nel proprio fuso orario).

>[!NOTE]
>
>[Ulteriori informazioni](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md#calculating-time-zone) informazioni su come Marketo calcola i fusi orari per i destinatari.

Consideriamo questo scenario più in dettaglio. Se sei a San Francisco, pianifica un’e-mail alle 07:00 per un appuntamento **09:00** invia. Nell’elenco avanzato sono presenti persone provenienti dalle seguenti aree geografiche:

* San Francisco
* Texas
* New York
* Italia

![](assets/image2017-12-6-10-3a52-3a41.png)

Le 9.00 sono già trascorse a New York e in Italia, pertanto le persone qualificate in questi due fusi orari riceveranno l’e-mail in base al **Impostazioni del fuso orario**:

* **Consegna il giorno seguente nel fuso orario del destinatario:** mercoledì alle 9 nei rispettivi fusi orari, **OPPURE**

* **Consegna in base all’ora predefinita del programma**: martedì alle 9 (New York - 12:00 EDT e Italia - 18:00 CET).

Una volta approvato il programma, quest’ultimo inizia a essere eseguito entro 15 minuti.

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>Anche se il programma avvierà il _processo_ dell&#39;invio di e-mail in 15 minuti, le e-mail non verranno _consegnato_ a quell&#39;ora. I destinatari continueranno a ricevere e-mail in base ai **Impostazioni del fuso orario** tu scegli.

## Scenario 2: più di 25 ore {#scenario-more-than-hours}

In questo secondo scenario, puoi approvare un programma e-mail con **Fuso orario destinatario** e un tempo di consegna pianificato superiore a 25 ore nel futuro. In questo caso, il programma inizierà a essere eseguito all&#39;ora pianificata nel **primissimo** il fuso orario nel mondo (UTC + 14:00). Potrebbero esserci persone che si qualificano per il tuo elenco avanzato in ogni fuso orario in tutto il mondo, quindi a partire dal fuso orario più prossimo ci consente di recapitare l’e-mail alla data/ora pianificata a tutti i destinatari nei loro rispettivi fusi orari.

**Inizio intestazione**

Ora, parliamo di come [Inizio intestazione](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) funziona con **Fuso orario destinatario**. La funzione Head Start richiede un programma con almeno 12 ore di anticipo. Cosa significa questo per il fuso orario del destinatario? Ricorda che quando il fuso orario del destinatario è abilitato, il programma e-mail viene eseguito all’ora pianificata nel fuso orario più vicino (UTC +14:00). Quindi, per abilitare **entrambi** Head Start e Recipient Time Zone, i programmi e-mail devono essere pianificati **almeno 12 ore prima dell’orario previsto in UTC +14:00.**

Ciò significa che se ti trovi in America/Los Angeles e desideri abilitare sia il fuso orario Head Start che quello del destinatario, devi pianificare il programma **34 ore** in anticipo. Come siamo arrivati a questo numero?

![](assets/image2017-12-5-13-3a11-3a38.png)

<br> 

In breve, i programmi e-mail pianificati con il fuso orario del destinatario devono iniziare a essere eseguiti all’ora pianificata nel fuso orario più vicino (ovvero, quando raggiunge prima la mezzanotte) per adattarsi a ogni fuso orario. Quindi, se pianifichi un programma e-mail...

* **con un tempo di consegna _entro_ 25 ore**, il programma inizia a funzionare entro 15 minuti. I destinatari che hanno già superato l’orario pianificato riceveranno l’e-mail in base alle impostazioni del fuso orario scelte.
* **con un tempo di consegna _più di_ 25 ore nel futuro**, il programma inizia a essere eseguito all’ora pianificata nel fuso orario più vicino (UTC +14:00).
* **con Head Start**, il programma inizia l’elaborazione 12 ore prima dell’ora pianificata nel fuso orario più vicino (UTC +14:00).

>[!CAUTION]
>
>Riceverai comunque l’e-mail da chiunque annulli l’abbonamento tra il momento in cui si avvia l’invio e quello in cui viene effettivamente consegnato. È consigliabile modificare la notifica di annullamento dell’abbonamento per riflettere il fatto che l’elaborazione degli annullamenti dell’abbonamento potrebbe richiedere 1-2 giorni lavorativi.

>[!MORELIKETHIS]
>
>* [Informazioni sul fuso orario del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Head Start per i programmi e-mail](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [Interrompi la consegna dei programmi e-mail pianificati con il fuso orario del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)
