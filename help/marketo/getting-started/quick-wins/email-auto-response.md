---
unique-page-id: 2359416
description: Risposta automatica e-mail - Documenti Marketo - Documentazione prodotto
title: Risposta automatica e-mail
translation-type: tm+mt
source-git-commit: 09dbd3a141fed0525aec8bf1ca6d141be2a6ce46
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---


# Risposta automatica e-mail {#email-auto-response}

## Missione: Invio di un messaggio e-mail di ringraziamento quando una persona compila il modulo {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}

>[!NOTE]
>
>**FYI**
>
>Marketo sta ora standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che l&#39;iscrizione contenga lead/lead e la persona/persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

>[!NOTE]
>
>**Prerequisiti**
>
>* [Configurazione e aggiunta di una persona](get-set-up-and-add-a-person.md)
>* [Pagina di destinazione con un modulo](landing-page-with-a-form.md)

>



## Passaggio 1: Creare un messaggio e-mail {#step-create-an-email}

1. Andate all&#39;area Attività di marketing.

   ![](assets/one-2.png)

1. Selezionate Programma personale nel menu a sinistra, fate clic sul menu a discesa Nuovo e selezionate Nuova risorsa locale.

   ![](assets/two-3.png)

1. Fate clic su E-mail.

   ![](assets/three-2.png)

1. Assegnate al messaggio e-mail il nome &quot;E-mail di risposta automatica&quot;, scegliete un modello e fate clic su Crea.

   ![](assets/four-1.png)

   Viene aperto un editor e-mail in una nuova finestra o scheda. Se i pop-up sono bloccati, fate clic su*** Modifica bozza* nella pagina di riepilogo delle risorse per accedere al messaggio e-mail.

1. Immettete un oggetto e fate doppio clic sull’area modificabile dell’e-mail.

   ![](assets/five-2.png)

   Viene aperto un editor Rich Text sopra all’editor e-mail.

1. Evidenzia il contenuto dell’e-mail esistente.

   ![](assets/six-2.png)

1. Digitate il contenuto e-mail e fate clic su Salva.

   ![](assets/seven-2.png)

1. Le modifiche vengono salvate automaticamente. Chiudete la scheda o la finestra dell’editor e-mail.

   ![](assets/eight-1.png)

1. Selezionate il nuovo messaggio e-mail. In Azioni e-mail fare clic su Approva.

   ![](assets/image2014-9-24-11-3a55-3a16.png)

## Passaggio 2: Creare una campagna intelligente {#step-create-a-smart-campaign}

1. Fai clic con il pulsante destro del mouse sul **programma** personale e fai clic su **Nuova campagna** avanzata.

   ![](assets/image2014-9-24-11-3a56-3a13.png)

1. **Denominate** la campagna intelligente &quot;Auto Response Campaign&quot; e fate clic su **Crea**.

   ![](assets/image2014-9-24-11-3a56-3a25.png)

1. Vai alla scheda **Smart List **4.

   ![](assets/image2014-9-24-11-3a56-3a38.png)

   Questa campagna viene impostata per essere eseguita ogni volta che una persona compila il modulo creato in Pagina di [**destinazione con un modulo**](landing-page-with-a-form.md).

1. Individua e trascina l&#39;attivatore **Riempimento modulo** sul quadro sinistro.

   ![](assets/image2014-9-24-11-3a57-3a18.png)

1. Selezionare **Modulo** personale dal menu a discesa. Fare clic sulla scheda **Flusso **2.

   ![](assets/image2014-9-24-11-3a57-3a29.png)

1. Trascinare l&#39;azione di flusso **Invia e-mail **sul quadro sinistro.

   ![](assets/image2014-9-24-11-3a57-3a41.png)

1. Selezionate il messaggio e-mail **di risposta** automatica e passate alla scheda **Schedule **tab.

   ![](assets/image2014-9-24-11-3a57-3a53.png)

1. Fate clic su **Modifica**.

   ![](assets/8.png)
Selezionate ogni volta e fate clic su Salva .
   ![](assets/9.png)

1. Fate clic su **Attiva**.

   ![](assets/10.png)

1. Fare clic su **Activate **nella schermata di conferma.

   ![](assets/11.png)

>[!NOTE]
>
>Una volta attiva, questa campagna viene eseguita ogni volta che una persona compila il modulo specificato. La campagna continuerà a essere attiva finché non verrà disattivata.

## Passaggio 3: Compilare il modulo {#step-fill-out-the-form}

1. Selezionate **Pagina** personale. Questo è stato creato nella pagina di [destinazione con una vittoria rapida Form](landing-page-with-a-form.md) .

   ![](assets/image2014-9-24-12-3a0-3a8.png)

1. Fate clic su **Visualizza pagina** approvata.

   ![](assets/image2014-9-24-12-3a0-3a18.png)

   La pagina di destinazione &quot;Versione di prova gratuita&quot; verrà aperta in una nuova scheda.

1. Compilate il modulo con il vostro nome, cognome e indirizzo e-mail, quindi fate clic su **Invia**.

   ![](assets/image2014-9-24-12-3a0-3a28.png)

>[!NOTE]
>
>Accertatevi di usare il vostro indirizzo e-mail effettivo per ricevere l&#39;e-mail.

## Missione completata {#mission-complete}

Nel giro di pochi minuti dovreste visualizzare il messaggio e-mail di risposta automatica nella vostra inbox. Ottimo lavoro!

<br> 

[◄ Missione 3: Punteggio](simple-scoring.md) semplice [Missione 5: Importa un elenco di lead ►](import-a-list-of-people.md)