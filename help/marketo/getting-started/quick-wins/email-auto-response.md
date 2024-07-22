---
unique-page-id: 2359416
description: Risposta automatica e-mail - Documenti Marketo - Documentazione del prodotto
title: Risposta automatica e-mail
exl-id: c9c0a154-65ec-4845-97a0-a2100223cb13
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Risposta automatica e-mail {#email-auto-response}

## Missione: Inviare un’e-mail di ringraziamento quando una persona compila un modulo {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}

>[!PREREQUISITES]
>
>* [Configurazione e aggiunta di una persona](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [Pagina di destinazione con modulo](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## Passaggio 1: creare un messaggio e-mail {#step-create-an-email}

1. Vai all&#39;area **[!UICONTROL Attività di marketing]**.

   ![](assets/email-auto-response-1.png)

1. Seleziona il programma nel menu a sinistra, fai clic sul menu a discesa **[!UICONTROL Nuovo]** e seleziona **[!UICONTROL Nuova risorsa locale]**.

   ![](assets/email-auto-response-2.png)

1. Seleziona **[!UICONTROL E-mail]**.

   ![](assets/email-auto-response-3.png)

1. Denomina il tuo indirizzo e-mail di risposta automatica, scegli un modello e fai clic su **[!UICONTROL Crea]**.

   ![](assets/email-auto-response-4.png)

   Un editor e-mail si aprirà in una nuova finestra o scheda. Se i popup sono bloccati, fai clic su **[!UICONTROL Modifica bozza]** nella pagina di riepilogo risorse per accedere all&#39;e-mail.

1. Inserisci un oggetto, quindi fai doppio clic sull’area modificabile dell’e-mail.

   ![](assets/email-auto-response-5.png)

   _Verrà aperto un editor Rich Text sopra l&#39;editor e-mail._

1. Evidenzia il contenuto dell’e-mail esistente.

   ![](assets/email-auto-response-6.png)

1. Digita il contenuto dell&#39;e-mail e fai clic su **[!UICONTROL Salva]**.

   ![](assets/email-auto-response-7.png)

1. Fai clic sul menu a discesa **[!UICONTROL Azioni e-mail]** e seleziona **[!UICONTROL Approva e chiudi]**.

   ![](assets/email-auto-response-8.png)

## Passaggio 2: creare una campagna avanzata {#step-create-a-smart-campaign}

1. Seleziona il programma, fai clic sul menu a discesa **[!UICONTROL Nuovo]** e seleziona **[!UICONTROL Nuova campagna avanzata]**.

   ![](assets/email-auto-response-9.png)

1. **Denomina** la tua smart campaign &quot;Auto Response Campaign&quot; (Campagna di risposta automatica) e fai clic su **[!UICONTROL Crea]**.

   ![](assets/email-auto-response-10.png)

1. Passa alla scheda **[!UICONTROL Elenco avanzato]**.

   ![](assets/email-auto-response-11.png)

   Questa campagna verrà impostata per essere eseguita ogni volta che una persona compila il modulo creato in [**Pagina di destinazione con un modulo**](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}.

1. Trova e trascina il trigger **[!UICONTROL Compila modulo]** nell&#39;area di lavoro.

   ![](assets/email-auto-response-12.png)

1. Seleziona **[!UICONTROL Modulo]** nel menu a discesa. Quindi fare clic sulla scheda **[!UICONTROL Flusso]**.

   ![](assets/email-auto-response-13.png)

1. Trascina l&#39;azione di flusso **[!UICONTROL Invia e-mail]** nell&#39;area di lavoro a sinistra.

   ![](assets/email-auto-response-14.png)

1. Seleziona **Indirizzo e-mail di risposta automatico**. Quindi fare clic sulla scheda **[!UICONTROL Pianificazione]**.

   ![](assets/email-auto-response-15.png)

1. Fai clic su **[!UICONTROL Modifica]**.

   ![](assets/email-auto-response-16.png)

1. Seleziona **[!UICONTROL ogni volta]** e fai clic su **[!UICONTROL Salva]**.

   ![](assets/email-auto-response-17.png)

1. Fare clic su **[!UICONTROL Attiva]**.

   ![](assets/email-auto-response-18.png)

1. Fai clic su **[!UICONTROL Attiva]** nella schermata di conferma.

   ![](assets/email-auto-response-19.png)

>[!NOTE]
>
>Una volta attivata, questa campagna verrà eseguita ogni volta che una persona compila il modulo specificato. La campagna continuerà a essere in esecuzione fino a quando non verrà disattivata.

## Passaggio 3: compilare il modulo {#step-fill-out-the-form}

1. Seleziona **Pagina personale** (creata nella [Pagina di destinazione con modulo](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} vinto rapidamente) e fai clic su **[!UICONTROL Anteprima]**.

   ![](assets/email-auto-response-20.png)

   _La pagina di destinazione &quot;Prova gratuita&quot; verrà aperta in una nuova scheda._

1. Compila il modulo con il tuo nome, cognome e indirizzo e-mail, quindi fai clic su **[!UICONTROL Invia]**.

   ![](assets/email-auto-response-21.png)

>[!NOTE]
>
>Assicurati di utilizzare il tuo indirizzo e-mail effettivo in modo da poter ottenere l’e-mail.

## Missione completata {#mission-complete}

In pochi minuti dovresti visualizzare l’e-mail di risposta automatica nella tua casella in entrata. Ottimo lavoro!

<br> 

[◄ Mission 3: punteggio semplice](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[Missione 5: importare un elenco di persone ►](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
