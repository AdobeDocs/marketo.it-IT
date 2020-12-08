---
unique-page-id: 2359424
description: Avvisare il rappresentante vendite - Documenti Marketo - Documentazione prodotto
title: Avvisa il rappresentante vendite
translation-type: tm+mt
source-git-commit: 09dbd3a141fed0525aec8bf1ca6d141be2a6ce46
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---


# Avvisa il rappresentante vendite {#alert-the-sales-rep}

## Missione: Avvisa il rappresentante commerciale quando una persona compila un modulo sul sito Web {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

Per inviare automaticamente le e-mail di avviso agli agenti di vendita, è sufficiente disporre di un messaggio e-mail di avviso e di una campagna e-mail. Ecco come farlo.

>[!NOTE]
>
>**FYI**
>
>Marketo sta standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che nell&#39;abbonamento siano presenti lead/lead e persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

>[!NOTE]
>
>**Prerequisiti**
>
>* [Pagina di destinazione con un modulo](landing-page-with-a-form.md)

>



## Passaggio 1: Creare un messaggio e-mail di avviso {#step-create-an-alert-email}

1. Andate all&#39;area **Attività** di marketing.

   ![](assets/one-5.png)

1. Selezionate **Il programma** personale creato nella pagina di [destinazione con una vittoria rapida del modulo](landing-page-with-a-form.md) , quindi in **Nuovo** fate clic su **Nuova risorsa** locale.

   ![](assets/two-6.png)

1. Fate clic su **E-mail**.

   ![](assets/three-5.png)

1. **Denominate** l’e-mail &quot;My Email Alert&quot;, selezionate un modello e fate clic su **Crea**.

   ![](assets/four-4.png)

1. Inserire il **Nome**, **Da e-mail**, **Rispondi** e **Oggetto** che si desidera venga visualizzato dal team di vendita.

   ![](assets/five-5.png)

1. Fate doppio clic per modificare il testo dell’e-mail.

   ![](assets/six-5.png)

1. Digitate il contenuto dell’e-mail.

   ![](assets/seven-6.png)

1. Posizionare il cursore nel punto in cui si desidera inserire le informazioni di contatto della persona e fare clic sull&#39;icona **Inserisci token** .

   ![](assets/eight-4.png)

1. Trova e seleziona il `{{SP_Send_Alert_Info}}` token **e fai clic su** Inserisci ****.

   ![](assets/image2014-9-24-13-3a10-3a0.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} è un token speciale per le e-mail di avviso. Consultate [Usare il token](../../product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) Invia informazioni di avviso per ulteriori informazioni.

1. Fate clic su **Salva**.

   ![](assets/ten-5.png)

1. Chiudete la scheda o la finestra dell’editor e-mail.

   ![](assets/eleven-5.png)

1. In Azioni **e-** mail fare clic su **Approva**.

   ![](assets/twelve-4.png)

## Passaggio 2: Creare una campagna di attivazione avvisi {#step-create-an-alert-trigger-campaign}

1. Selezionate **Il programma** precedentemente creato, quindi in **Nuovo **fate clic su **Nuova campagna** avanzata.

   ![](assets/image2014-9-24-13-3a14-3a17.png)

1. **Denominate** la campagna &quot;My Alert Campaign&quot; e fate clic su **Create (Crea**).

   ![](assets/image2014-9-24-13-3a14-3a28.png)

1. Nella scheda Elenco **** avanzato, individuare e trascinare il trigger **Riempi modulo** nell&#39;area di lavoro.

   ![](assets/image2014-9-24-13-3a14-3a43.png)

1. Selezionare il modulo creato in precedenza.

   ![](assets/image2014-9-24-13-3a14-3a58.png)

1. Nella scheda **Flusso** , trova e trascina l’azione di flusso **Invia avviso** nell’area di lavoro.

   ![](assets/image2014-9-24-13-3a15-3a10.png)

1. Seleziona **Il mio messaggio e-mail** di avviso creato in precedenza e lascia **Invia a** come proprietario **** delle vendite.

   ![](assets/eighteen-1.png)

1. Digitate il vostro indirizzo e-mail nel campo **A altre e-mail** .

   ![](assets/nineteen-2.png)

1. Vai alla scheda **Pianificazione** e fai clic sul pulsante **Activate **button.

   ![](assets/twenty-2.png)

   >[!TIP]
   >
   >
   >Imposta le regole **di** qualifica su **ogni volta** (modificando Smart Campaign) per consentire alla stessa persona di attivare gli avvisi più volte.

1. Fate clic su **Attiva** nella schermata di conferma.

   ![](assets/twenty-one-1.png)

## Passaggio 3: Test! {#step-test-it-out}

1. Selezionate la pagina di destinazione e fate clic su **Visualizza pagina** approvata.

   ![](assets/image2014-9-24-13-3a17-3a8.png)

   >[!NOTE]
   >
   >**Promemoria**
   >
   >
   >Non dimenticare di approvare le pagine di destinazione; non vanno in diretta fino all&#39;approvazione.

1. Compilare il modulo e fare clic su **Invia**.

   ![](assets/image2014-9-24-13-3a17-3a41.png)

1. Dovreste ricevere la vostra e-mail a breve. Una volta verificato che tutto funziona correttamente, rimuovete il vostro indirizzo e-mail dal flusso di avvisi di invio (vedere il passaggio 2.7 precedente).

   >[!NOTE]
   >
   >Fate clic sulla scheda Informazioni **** persona in Markech per visualizzare le informazioni di contatto.

## Missione Completa! {#mission-complete}

<br> 

[◄ Missione 7: Personalizza una](personalize-an-email.md) missione e-mail [9: Aggiorna dati lead ►](update-person-data.md)