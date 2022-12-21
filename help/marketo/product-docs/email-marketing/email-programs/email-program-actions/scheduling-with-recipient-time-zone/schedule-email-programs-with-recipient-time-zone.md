---
unique-page-id: 12982903
description: Pianificazione dei programmi e-mail con fuso orario destinatario - Documenti Marketo - Documentazione del prodotto
title: Pianificare programmi e-mail con il fuso orario del destinatario
exl-id: d0c3f3c1-9f21-4081-818d-7c5cb1766915
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# Pianificare programmi e-mail con il fuso orario del destinatario {#schedule-email-programs-with-recipient-time-zone}

Esistono due possibili scenari quando si pianifica un programma e-mail quando il fuso orario Destinatario è abilitato:

1. Pianificazione del programma da eseguire **entro** le prossime 25 ore
1. Pianificazione del programma da eseguire **more** più di 25 ore future (cioè la settimana prossima)

## Scenario 1: Entro 25 ore {#scenario-within-hours}

Supponiamo che tu approvi un programma e-mail con il fuso orario destinatario abilitato e un orario di consegna pianificato entro le prossime 25 ore. Potresti avere persone nella tua lista intelligente che vivono in fusi orari in cui l&#39;orario pianificato è già passato.

In questo scenario, ti permettiamo di decidere cosa fare con questo sottoinsieme di persone qualificate. Fai clic sull’icona a forma di ingranaggio accanto a **Fuso orario destinatario** in **Pianificazione** sezione del programma e-mail.

![](assets/image2017-12-5-10-3a46-3a42.png)

Questo offre due opzioni:

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**Definizione**
>
>* **Consegna del giorno successivo nel fuso orario del destinatario**: se l’e-mail verrà inviata martedì alle 09:00, le persone qualificate che vivono in fusi orari in cui l’orario pianificato è già passato riceveranno l’e-mail in *Mercoledì* alle 9.
>
>* **Consegna utilizzando l&#39;orario predefinito del programma**: se l’e-mail verrà inviata martedì alle 09:00, le persone qualificate che vivono in fusi orari in cui l’orario pianificato è già passato riceveranno l’e-mail _in base alle impostazioni del fuso orario dell’abbonamento_. Quindi, se il tuo [impostazioni del fuso orario della sottoscrizione](/help/marketo/product-docs/administration/settings/select-your-language-locale-and-time-zone.md) sono impostati su PDT America/Los Angeles, questi destinatari riceveranno ancora l&#39;e-mail martedì alle 9:00 PDT (a prescindere dall&#39;ora che può essere nel proprio fuso orario).


>[!NOTE]
>
>[Ulteriori informazioni](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md#calculating-time-zone) informazioni su come Marketo calcola i fusi orari dei destinatari.

Consideriamo questo scenario più dettagliatamente. Se sei a San Francisco, pianifica un&#39;e-mail alle 7:00 per un **9:00** invia. Nell’elenco smart sono presenti persone provenienti dalle seguenti aree:

* San Francisco
* Texas
* New York
* Italia

![](assets/image2017-12-6-10-3a52-3a41.png)

Le 9:00 sono già passate a New York e in Italia, così persone qualificate in questi due fusi orari riceveranno l&#39;e-mail basata sul **Impostazioni del fuso orario**:

* **Fornisci il giorno seguente nel fuso orario del destinatario:** Mercoledì alle 9.00 nei rispettivi fusi orari, **O**

* **Consegna utilizzando l&#39;orario predefinito del programma**: Martedì alle 9:00 PDT (New York - 12:00 EDT e Italia - 18:00 CET).

Una volta approvato il programma, questo inizia a funzionare entro 15 minuti.

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>Anche se il programma avvierà il _processo_ di inviare e-mail in 15 minuti, le e-mail non saranno _consegnato_ all&#39;epoca. I destinatari riceveranno ancora e-mail basate su **Impostazioni del fuso orario** scegli tu.

## Scenario 2: Oltre 25 ore {#scenario-more-than-hours}

In questo secondo scenario, approvi un programma e-mail con **Fuso orario destinatario** abilitato e un tempo di consegna pianificato superiore a 25 ore in futuro. In questo caso, il programma inizierà a funzionare all&#39;ora pianificata nella **primo** fuso orario nel mondo (UTC + 14.00). Ci possono essere persone idonee per il tuo smart list in ogni fuso orario del mondo, quindi a partire dal primo fuso orario possiamo inviare l’e-mail alla data/ora pianificata a tutti i destinatari nei rispettivi fusi orari.

**Inizio testina**

Ora, parliamo di come [Inizio testina](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) funziona con **Fuso orario destinatario**. La funzionalità Head Start esistente richiede che il programma sia programmato almeno con 12 ore di anticipo. Cosa significa questo per il fuso orario dei destinatari? Ricorda che quando il fuso orario del destinatario è abilitato, il programma e-mail viene eseguito all’ora pianificata nel primo fuso orario (UTC +14:00). Quindi, per **entrambi** Inizio intestazione e Fuso orario destinatario, i programmi e-mail devono essere pianificati **almeno 12 ore prima dell’orario previsto in UTC +14:00.**

Ciò significa che se sei in America/Los Angeles e vuoi abilitare sia Head Start che Recipient Time Zone, devi pianificare il programma **34 ore** in anticipo. Come siamo arrivati a questo numero?

![](assets/image2017-12-5-13-3a11-3a38.png)

<br> 

In breve, i programmi e-mail pianificati con il fuso orario del destinatario devono iniziare a essere in esecuzione all’ora pianificata nel primo fuso orario (cioè, dove raggiunge prima la mezzanotte) per adattarsi a ogni fuso orario. Quindi, se pianifichi un programma e-mail...

* **con tempi di consegna _entro_ 25 ore**, il programma inizia a funzionare entro 15 minuti. I destinatari che hanno già superato l’orario pianificato riceveranno l’e-mail in base alle impostazioni del fuso orario scelte.
* **con tempi di consegna _più di_ 25 ore future**, il programma inizia a funzionare all’ora pianificata nel primo fuso orario (UTC +14:00).
* **con inizio testa**, il programma inizia l’elaborazione 12 ore prima dell’ora pianificata nel primo fuso orario (UTC +14:00).

>[!CAUTION]
>
>Chiunque annulli l’abbonamento tra il momento in cui si avvia l’invio dell’e-mail e il momento in cui viene effettivamente consegnato riceverà comunque l’e-mail. È consigliabile regolare la notifica di annullamento dell’abbonamento in modo che rifletta che l’elaborazione degli abbonamenti potrebbe richiedere 1-2 giorni lavorativi.

>[!MORELIKETHIS]
>
>* [Informazioni sul fuso orario del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Avvio intestazione per programmi e-mail](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [Interrompi la consegna di programmi e-mail pianificati con il fuso orario del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)

