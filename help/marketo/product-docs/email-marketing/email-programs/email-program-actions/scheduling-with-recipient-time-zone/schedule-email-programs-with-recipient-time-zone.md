---
unique-page-id: 12982903
description: Pianificazione di programmi e-mail con fuso orario destinatario - Documenti Marketo - Documentazione prodotto
title: Pianificazione dei programmi e-mail con il fuso orario del destinatario
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 0%

---


# Pianificazione dei programmi e-mail con il fuso orario del destinatario {#schedule-email-programs-with-recipient-time-zone}

Esistono due possibili scenari quando si pianifica un programma e-mail mentre il fuso orario del destinatario è abilitato:

1. Pianificazione dell&#39;esecuzione del programma **entro** le prossime 25 ore
1. Programmazione del programma per eseguire **più** di 25 ore in futuro (ad esempio, la settimana successiva)

## Scenario 1: Entro 25 ore {#scenario-within-hours}

Supponiamo che tu approvi un programma e-mail con l&#39;opzione Fuso orario destinatario abilitata e un orario di consegna pianificato entro le prossime 25 ore. È possibile che nell&#39;elenco smart siano presenti persone che vivono in fusi orari in cui l&#39;ora pianificata è già passata.

In questo scenario, vi consentiamo di decidere cosa fare con questo sottoinsieme di persone qualificate. Fate clic sull&#39;icona a forma di ingranaggio accanto a **Recipient Time Zone** (Fuso orario destinatario) nella sezione **Schedule** (Pianificazione)del programma e-mail.

![](assets/image2017-12-5-10-3a46-3a42.png)

Sono disponibili due opzioni:

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**Definizione**
>
>* **Consegna del giorno seguente nel fuso** orario del destinatario: se l&#39;e-mail è prevista per martedì alle 9:00, le persone qualificate che vivono in fusi orari in cui l&#39;orario previsto è già passato riceveranno l&#39;e-mail il *mercoledì* alle 9:00.
   >
   >
* **Eseguire utilizzando l&#39;ora** predefinita del programma: se l&#39;e-mail è pianificata per uscire martedì alle 9:00, le persone qualificate che vivono in fusi orari in cui l&#39;ora pianificata è già passata riceveranno l&#39;e-mail *in base alle impostazioni* del fuso orario dell&#39;iscrizione. Pertanto, se le impostazioni relative al fuso orario [dell&#39;](../../../../../product-docs/administration/settings/select-your-language-locale-and-time-zone.md) iscrizione sono impostate [](../../../../../product-docs/administration/settings/set-default-location-settings-for-a-subscription.md) su PDT America/Los Angeles, questi destinatari riceveranno comunque l&#39;e-mail il martedì alle 9:00 PDT (a prescindere dall&#39;ora in cui si trova il fuso orario).

>



>[!NOTE]
>
>[Ulteriori](https://docs.marketo.com/display/DOCS/Understanding+Recipient+Time+Zone#UnderstandingRecipientTimeZone-CalculatingTimeZone) informazioni sul modo in cui Marketo calcola i fusi orari per i destinatari.

Consideriamo questo scenario più dettagliatamente. Se sei a San Francisco, pianifica un&#39;e-mail alle 7:00 per un invio alle **9:00** . Nell&#39;elenco smart, sono presenti persone provenienti dalle seguenti aree:

* San Francisco
* Texas
* New York
* Italia

![](assets/image2017-12-6-10-3a52-3a41.png)

Le 9:00 sono già passate a New York e in Italia, così le persone qualificate in questi due fusi orari riceveranno l&#39;e-mail in base alle impostazioni **del** fuso orario:

* **Consegna del giorno seguente nel fuso orario del destinatario:** Mercoledì alle 9:00 nei rispettivi fusi orari, **OPPURE**

* **Eseguire utilizzando l&#39;ora** predefinita del programma: Martedì alle 9:00 PDT (New York - 12:00 EDT e Italia - 18:00 CET).

Una volta approvato, il programma inizia a funzionare entro 15 minuti.

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>Anche se il programma avvierà il *processo* di invio di e-mail in 15 minuti, le e-mail non verranno *recapitate* in quel momento. I destinatari continueranno a ricevere e-mail in base alle impostazioni **del fuso** orario prescelte.

## Scenario 2: Oltre 25 ore {#scenario-more-than-hours}

In questo secondo scenario, approvi un programma e-mail con fuso orario **** Destinatario abilitato e un orario di consegna pianificato superiore a 25 ore in futuro. In questo caso, il programma inizierà a funzionare all&#39;ora prevista nel fuso orario **più** vicino al mondo (UTC + 14:00). Ci possono essere persone idonee per il tuo elenco smart in ogni fuso orario del mondo, quindi a partire dal primo fuso orario ci permette di inviare l&#39;e-mail alla data/ora pianificata a tutti i destinatari nei rispettivi fusi orari.

Inizio punta

Ora, parliamo di come [Head Start](../../../../../product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) funziona con **Recipient Time Zone**. La funzione Head Start richiede che il programma sia pianificato almeno con 12 ore di anticipo. Cosa significa questo per Recipiente Fuso orario? Ricorda che quando l&#39;opzione Fuso orario destinatario è abilitata, il programma e-mail viene avviato all&#39;ora pianificata nel fuso orario più recente (UTC +14:00). Pertanto, per attivare **sia** Head Start che il Recipient Time Zone, i programmi e-mail devono essere pianificati **almeno 12 ore prima dell&#39;ora pianificata in UTC +14:00.**

Ciò significa che se sei in America/Los Angeles e vuoi attivare sia Head Start che Recipient Time Zone, devi pianificare il programma con **34 ore** di anticipo. Come siamo arrivati a questo numero?

![](assets/image2017-12-5-13-3a11-3a38.png)

<br> 

In breve, i programmi e-mail pianificati con il fuso orario del destinatario devono iniziare a essere in esecuzione all&#39;ora pianificata nel primo fuso orario (ovvero, dove arriva prima la mezzanotte) per poter ospitare ogni fuso orario. Quindi, se pianifichi un programma email...

* **con un tempo di consegna *entro* 25 ore**, il programma inizia a funzionare entro 15 minuti. I destinatari che hanno già superato l&#39;orario previsto riceveranno l&#39;e-mail in base alle impostazioni del fuso orario prescelte.
* **con un tempo di consegna *superiore* *a 25 ore in futuro***, il programma inizia a funzionare all&#39;ora pianificata nel fuso orario più vicino (UTC +14:00).
* **con Head Start**, il programma inizia l&#39;elaborazione 12 ore prima dell&#39;orario previsto nel fuso orario più vicino (UTC +14:00).

>[!CAUTION]
>
>Chiunque annulla l’iscrizione tra il momento in cui viene avviata l’invio e-mail e il momento in cui viene effettivamente recapitato riceverà comunque l’e-mail. È consigliabile regolare la notifica di annullamento dell’iscrizione in modo da riflettere il fatto che l’elaborazione degli abbonamenti potrebbe richiedere 1-2 giorni lavorativi.

>[!NOTE]
>
>**Articoli correlati**
>
>* [Informazioni sul fuso orario del destinatario](understanding-recipient-time-zone.md)
>* [Head Start for Email Programs](../../../../../product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [Interrompi consegna programmi e-mail pianificati con il fuso orario del destinatario](abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)

>



