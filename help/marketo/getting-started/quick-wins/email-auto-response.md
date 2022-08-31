---
unique-page-id: 2359416
description: Risposta automatica e-mail - Documenti Marketo - Documentazione del prodotto
title: Risposta automatica e-mail
exl-id: c9c0a154-65ec-4845-97a0-a2100223cb13
source-git-commit: 1c350eb17992e45b9e0f825e1abd5c86555d0a0a
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# Risposta automatica e-mail {#email-auto-response}

## Missione: Invia un messaggio e-mail di ringraziamento quando una persona compila un modulo {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}

>[!PREREQUISITES]
>
>* [Configurazione e aggiunta di una persona](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target=&quot;_blank&quot;}
>* [Pagina di destinazione con un modulo](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}


## Passaggio 1: Creare un messaggio e-mail {#step-create-an-email}

1. Vai all’area Attività di marketing .

   ![](assets/email-auto-response-1.png)

1. Seleziona il programma nel menu a sinistra, fai clic sul **Nuovo** a discesa e seleziona **Nuova risorsa locale**.

   ![](assets/email-auto-response-2.png)

1. Seleziona **E-mail**.

   ![](assets/email-auto-response-3.png)

1. Denomina l&#39;e-mail &quot;Auto Response Email&quot;, scegli un modello e fai clic su **Crea**.

   ![](assets/email-auto-response-4.png)

   Viene aperto un editor e-mail in una nuova finestra o scheda. Se i popup sono bloccati, fare clic su **Modifica bozza** nella pagina di riepilogo delle risorse per accedere all’e-mail.

1. Inserisci un oggetto, quindi fai doppio clic sull’area modificabile dell’e-mail.

   ![](assets/email-auto-response-5.png)

   _Viene aperto un editor Rich Text sopra l’editor e-mail._

1. Evidenzia il contenuto dell’e-mail esistente.

   ![](assets/email-auto-response-6.png)

1. Digita il contenuto dell’e-mail e fai clic su **Salva**.

   ![](assets/email-auto-response-7.png)

1. Fai clic sul pulsante **Azioni e-mail** a discesa e seleziona **Approva e chiudi**.

   ![](assets/email-auto-response-8.png)

## Passaggio 2: Creare una campagna avanzata {#step-create-a-smart-campaign}

1. Seleziona il programma e fai clic sul pulsante **Nuovo** a discesa e seleziona **Nuova campagna Smart**.

   ![](assets/email-auto-response-9.png)

1. **Nome** la campagna intelligente &quot;Auto Response Campaign&quot; e fai clic su **Crea**.

   ![](assets/email-auto-response-10.png)

1. Vai a **Elenco avanzato** scheda .

   ![](assets/email-auto-response-11.png)

   Questa campagna viene impostata per essere eseguita ogni volta che una persona compila il modulo creato in [**Pagina di destinazione con un modulo**](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}.

1. Trova e trascina **Riempie il modulo** attiva l’area di lavoro.

   ![](assets/email-auto-response-12.png)

1. Seleziona **Modulo personale** nel menu a discesa . Quindi fai clic sul pulsante **Flusso** scheda .

   ![](assets/email-auto-response-13.png)

1. Trascina **Invia e-mail** azione di scorrimento verso l&#39;area di lavoro sinistra.

   ![](assets/email-auto-response-14.png)

1. Seleziona la tua **E-mail di risposta automatica**. Quindi fai clic sul pulsante **Pianificazione** scheda .

   ![](assets/email-auto-response-15.png)

1. Fai clic su **Modifica**.

   ![](assets/email-auto-response-16.png)

1. Seleziona **Ogni volta** e fai clic su **Salva**.

   ![](assets/email-auto-response-17.png)

1. Fai clic su **Attiva**.

   ![](assets/email-auto-response-18.png)

1. Fai clic su **Attiva** nella schermata di conferma.

   ![](assets/email-auto-response-19.png)

>[!NOTE]
>
>Una volta attivata, questa campagna viene eseguita ogni volta che una persona compila il modulo specificato. La campagna continuerà a essere in esecuzione finché non viene disattivata.

## Passaggio 3: Compilare il modulo {#step-fill-out-the-form}

1. Seleziona **Pagina personale** (creato nella sezione [Pagina di destinazione con un modulo](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;} vittoria rapida) e fai clic su **Anteprima**.

   ![](assets/email-auto-response-20.png)

   _La pagina di destinazione &quot;Prova gratuita&quot; si aprirà in una nuova scheda._

1. Compila il modulo con il tuo nome, cognome e indirizzo e-mail, quindi fai clic su **Invia**.

   ![](assets/email-auto-response-21.png)

>[!NOTE]
>
>Assicurati di utilizzare il tuo indirizzo e-mail effettivo in modo da poter ricevere l&#39;e-mail.

## Missione completata {#mission-complete}

Nel giro di pochi minuti dovresti visualizzare l’e-mail di risposta automatica nella tua casella in entrata. Ottimo lavoro!

<br> 

[◄ Missione 3: Punteggio semplice](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[Missione 5: Importa un elenco di persone ►](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
