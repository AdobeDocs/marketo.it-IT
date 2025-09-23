---
unique-page-id: 2359416
description: Risposta automatica e-mail - Documentazione di Marketo - Documentazione del prodotto
title: Risposta automatica e-mail
exl-id: c9c0a154-65ec-4845-97a0-a2100223cb13
feature: Getting Started
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 100%

---

# Risposta automatica e-mail {#email-auto-response}

## Missione: inviare un’e-mail di ringraziamento quando una persona compila un modulo {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}

>[!PREREQUISITES]
>
>* [Configurare e aggiungere una persona](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [Pagina di destinazione con modulo](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## Passaggio 1: creare un messaggio e-mail {#step-create-an-email}

1. Passa all&#39;area [!UICONTROL Marketing Activities].

   ![](assets/email-auto-response-1.png)

1. Seleziona il programma nel menu a sinistra, fai clic sul menu a discesa **[!UICONTROL New]** e seleziona **[!UICONTROL New Local Asset]**.

   ![](assets/email-auto-response-2.png)

1. Seleziona **[!UICONTROL Email]**.

   ![](assets/email-auto-response-3.png)

1. Assegna un nome all&#39;indirizzo e-mail di risposta automatica, scegli un modello e fai clic su **[!UICONTROL Create]**.

   ![](assets/email-auto-response-4.png)

   Un editor e-mail si aprirà in una nuova finestra o scheda. Se i pop-up sono bloccati, fai clic su **[!UICONTROL Edit Draft]** nella pagina di riepilogo delle risorse per accedere all&#39;e-mail.

1. Inserisci un oggetto, quindi fai doppio clic sull’area modificabile dell’e-mail.

   ![](assets/email-auto-response-5.png)

   _Verrà aperto un editor Rich Text sopra l&#39;editor e-mail._

1. Evidenzia il contenuto dell’e-mail esistente.

   ![](assets/email-auto-response-6.png)

1. Digita il contenuto dell&#39;e-mail e fai clic su **[!UICONTROL Save]**.

   ![](assets/email-auto-response-7.png)

1. Fai clic sul menu a discesa **[!UICONTROL Email Actions]** e seleziona **[!UICONTROL Approve and Close]**.

   ![](assets/email-auto-response-8.png)

## Passaggio 2: creare una campagna avanzata {#step-create-a-smart-campaign}

1. Seleziona il programma, fai clic sul menu a discesa **[!UICONTROL New]** e seleziona **[!UICONTROL New Smart Campaign]**.

   ![](assets/email-auto-response-9.png)

1. **Assegna un nome** alla campagna avanzata &quot;Campagna di risposta automatica&quot; e fai clic su **[!UICONTROL Create]**.

   ![](assets/email-auto-response-10.png)

1. Passa alla scheda **[!UICONTROL Smart List]**.

   ![](assets/email-auto-response-11.png)

   Questa campagna verrà impostata per essere eseguita ogni volta che una persona compila il modulo creato in [**Pagina di destinazione con un modulo**](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}.

1. Trova e trascina il trigger **[!UICONTROL Fills Out Form]** nell&#39;area di lavoro.

   ![](assets/email-auto-response-12.png)

1. Seleziona **[!UICONTROL My Form]** nel menu a discesa. Quindi fai clic sulla scheda **[!UICONTROL Flow]**.

   ![](assets/email-auto-response-13.png)

1. Trascina l&#39;azione di flusso **[!UICONTROL Send Email]** nell&#39;area di lavoro a sinistra.

   ![](assets/email-auto-response-14.png)

1. Seleziona **E-mail di risposta automatica**. Quindi fai clic sulla scheda **[!UICONTROL Schedule]**.

   ![](assets/email-auto-response-15.png)

1. Fai clic su **[!UICONTROL Edit]**.

   ![](assets/email-auto-response-16.png)

1. Seleziona **[!UICONTROL every time]** e fai clic su **[!UICONTROL Save]**.

   ![](assets/email-auto-response-17.png)

1. Fai clic su **[!UICONTROL Activate]**.

   ![](assets/email-auto-response-18.png)

1. Fai clic su **[!UICONTROL Activate]** nella schermata di conferma.

   ![](assets/email-auto-response-19.png)

>[!NOTE]
>
>Una volta attivata, questa campagna verrà eseguita ogni volta che una persona compila il modulo specificato. La campagna continuerà a essere attiva fino a quando non verrà disattivata.

## Passaggio 3: compilare il modulo {#step-fill-out-the-form}

1. Seleziona **Pagina personale** (creata rapidamente nella [Pagina di destinazione con modulo](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}) e fai clic su **[!UICONTROL Preview]**.

   ![](assets/email-auto-response-20.png)

   _La pagina di destinazione &quot;Prova gratuita&quot; verrà aperta in una nuova scheda._

1. Compila il modulo con il tuo nome, cognome e indirizzo e-mail, quindi fai clic su **[!UICONTROL Submit]**.

   ![](assets/email-auto-response-21.png)

>[!NOTE]
>
>Assicurati di utilizzare il tuo indirizzo e-mail reale in modo da poter ottenere l’e-mail.

## Missione completata {#mission-complete}

In pochi minuti dovresti visualizzare l’e-mail di risposta automatica nella tua casella in entrata.

[◄ Missione 3: punteggio semplice](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[Missione 5: importare un elenco di persone ►](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
