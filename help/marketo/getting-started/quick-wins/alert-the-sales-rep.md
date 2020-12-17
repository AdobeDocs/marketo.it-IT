---
unique-page-id: 2359424
description: Avvisare il rappresentante vendite - Documenti Marketo - Documentazione prodotto
title: Avvisa il rappresentante vendite
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---


# Avvisare il rappresentante commerciale {#alert-the-sales-rep}

## Missione: Avvisare il responsabile vendite quando una persona compila un modulo sul sito Web {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

Per inviare automaticamente le e-mail di avviso agli agenti di vendita, è sufficiente disporre di un messaggio e-mail di avviso e di una campagna e-mail. Ecco come farlo.

>[!PREREQUISITES]
>
>[Pagina di destinazione con un modulo](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

## Passaggio 1: Creare un&#39;e-mail di avviso {#step-create-an-alert-email}

1. Andate all&#39;area **Attività di marketing**.

   ![](assets/one-5.png)

1. Selezionare **My Program** creato nella pagina di destinazione con una vittoria rapida di Form](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md), quindi in **New** fare clic su **New Local Asset** (Nuova risorsa locale).[

   ![](assets/two-6.png)

1. Fare clic su **E-mail**.

   ![](assets/three-5.png)

1. **Denominate** l’e-mail &quot;My Email Alert&quot;, selezionate un modello e fate clic su  **Crea**.

   ![](assets/four-4.png)

1. Immettere il **Da nome**, **Da e-mail**, **Rispondi a** e **Oggetto** che si desidera vengano visualizzati dal team di vendita.

   ![](assets/five-5.png)

1. Fate doppio clic per modificare il testo dell’e-mail.

   ![](assets/six-5.png)

1. Digitate il contenuto dell’e-mail.

   ![](assets/seven-6.png)

1. Posizionare il cursore nel punto in cui si desidera inserire le informazioni di contatto della persona e fare clic sull&#39;icona **Inserisci token**.

   ![](assets/eight-4.png)

1. Trovare e selezionare il `{{SP_Send_Alert_Info}}` **Token** e fare clic su **Inserisci**.

   ![](assets/image2014-9-24-13-3a10-3a0.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} è un token speciale per le e-mail di avviso. Per ulteriori informazioni, vedere [Utilizzare il token di invio delle informazioni di avviso](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md).

1. Fare clic su **Salva**.

   ![](assets/ten-5.png)

1. Chiudete la scheda o la finestra dell’editor e-mail.

   ![](assets/eleven-5.png)

1. In **Azioni e-mail** fare clic su **Approva**.

   ![](assets/twelve-4.png)

## Passaggio 2: Creare una campagna di attivazione avvisi {#step-create-an-alert-trigger-campaign}

1. Selezionare **My Program** creato in precedenza, quindi in **New** fare clic su **New Smart Campaign**.

   ![](assets/image2014-9-24-13-3a14-3a17.png)

1. **Denominate** la campagna &quot;My Alert Campaign&quot; e fate clic su  **Create (Crea**).

   ![](assets/image2014-9-24-13-3a14-3a28.png)

1. Nella scheda **Smart List**, individuare e trascinare il trigger **Riempi modulo** sull&#39;area di lavoro.

   ![](assets/image2014-9-24-13-3a14-3a43.png)

1. Selezionare il modulo creato in precedenza.

   ![](assets/image2014-9-24-13-3a14-3a58.png)

1. Nella scheda **Flusso**, individuare e trascinare l&#39;azione di flusso **Invia avviso** nell&#39;area di lavoro.

   ![](assets/image2014-9-24-13-3a15-3a10.png)

1. Selezionare **My Alert Email** creato in precedenza e lasciare **Send To** come **Sales Owner**.

   ![](assets/eighteen-1.png)

1. Digitare l&#39;indirizzo e-mail nel campo **Alle altre e-mail**.

   ![](assets/nineteen-2.png)

1. Fare clic sulla scheda **Pianificazione** e quindi sul pulsante **Attiva**.

   ![](assets/twenty-2.png)

   >[!TIP]
   >
   >Impostate le **Regole di qualifica** su **ogni volta** (modificando la Smart Campaign) per consentire alla stessa persona di attivare più volte gli avvisi.

1. Fare clic su **Attiva** nella schermata di conferma.

   ![](assets/twenty-one-1.png)

## Passaggio 3: Test! {#step-test-it-out}

1. Selezionate la pagina di destinazione e fate clic su **Visualizza pagina approvata**.

   ![](assets/image2014-9-24-13-3a17-3a8.png)

   >[!NOTE]
   >
   >Non dimenticare di approvare le pagine di destinazione; non vanno in diretta fino all&#39;approvazione.

1. Compilare il modulo e fare clic su **Invia**.

   ![](assets/image2014-9-24-13-3a17-3a41.png)

1. Dovreste ricevere la vostra e-mail a breve. Una volta verificato che tutto funziona correttamente, rimuovete il vostro indirizzo e-mail dal flusso di avvisi di invio (vedere il passaggio 2.7 precedente).

   >[!NOTE]
   >
   >Fare clic sulla scheda **Informazioni sulla persona** in Markeper visualizzare le informazioni sul contatto.

## Missione Completa! {#mission-complete}

<br> 

[◄ Missione 7: Personalizzare un&#39;e-mail](personalize-an-email.md)

[Missione 9: Aggiorna dati lead ►](update-person-data.md)
