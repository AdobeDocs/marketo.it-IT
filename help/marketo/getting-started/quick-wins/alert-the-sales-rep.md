---
unique-page-id: 2359424
description: Avvisare il rappresentante commerciale - Marketo Docs - Documentazione del prodotto
title: Avvisare il rappresentante commerciale
exl-id: 4ad7d7b8-ee1e-4605-b4e0-e72a7e573c05
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# Avvisare il rappresentante commerciale {#alert-the-sales-rep}

## Missione: Avvisa il rappresentante commerciale quando una persona compila un modulo sul tuo sito web {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

Per inviare automaticamente le e-mail di avviso ai rappresentanti commerciali, tutto ciò di cui hai bisogno è un’e-mail di avviso e una campagna e-mail. Ecco come farlo.

>[!PREREQUISITES]
>
>[Pagina di destinazione con un modulo](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

## Passaggio 1: Creare un messaggio e-mail di avviso {#step-create-an-alert-email}

1. Vai all&#39;area **Attività di marketing**.

   ![](assets/one-5.png)

1. Seleziona **Il mio programma** che hai creato nella [Pagina di destinazione con una vittoria rapida di Form](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md), quindi in **Nuovo** fai clic su **Nuova risorsa locale**.

   ![](assets/two-6.png)

1. Fare clic su **Email**.

   ![](assets/three-5.png)

1. **** Assegna un nome all’e-mail &quot;My Email Alert&quot;, seleziona un modello e fai clic su  **Crea**.

   ![](assets/four-4.png)

1. Immetti i valori **Da nome**, **Da e-mail**, **Risposta-a** e **Oggetto** che desideri che venga visualizzato dal team di vendita.

   ![](assets/five-5.png)

1. Fai doppio clic per modificare il testo dell’e-mail.

   ![](assets/six-5.png)

1. Digita il contenuto dell’e-mail.

   ![](assets/seven-6.png)

1. Posizionare il cursore nel punto in cui si desidera inserire le informazioni di contatto della persona e fare clic sull&#39;icona **Inserisci token**.

   ![](assets/eight-4.png)

1. Trova e seleziona il `{{SP_Send_Alert_Info}}` **Token** e fai clic su **Inserisci**.

   ![](assets/image2014-9-24-13-3a10-3a0.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} è un token speciale per le e-mail di avviso. Per ulteriori informazioni, consulta [Utilizzare il token per le informazioni sull’invio degli avvisi](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) .

1. Fare clic su **Salva**.

   ![](assets/ten-5.png)

1. Chiudi la scheda/finestra dell’editor e-mail.

   ![](assets/eleven-5.png)

1. In **Azioni e-mail** fai clic su **Approva**.

   ![](assets/twelve-4.png)

## Passaggio 2: Creare una campagna di attivazione degli avvisi {#step-create-an-alert-trigger-campaign}

1. Seleziona **Il mio programma** creato in precedenza, quindi in **Nuovo** fai clic su **Nuova campagna avanzata**.

   ![](assets/image2014-9-24-13-3a14-3a17.png)

1. **** Denomina la campagna &quot;My Alert Campaign&quot; (Campagna di avviso personale) e fai clic su  **Crea**.

   ![](assets/image2014-9-24-13-3a14-3a28.png)

1. Sotto la scheda **Elenco avanzato** , trova e trascina il trigger **Riempie il modulo** sull’area di lavoro.

   ![](assets/image2014-9-24-13-3a14-3a43.png)

1. Selezionare il modulo creato in precedenza.

   ![](assets/image2014-9-24-13-3a14-3a58.png)

1. Nella scheda **Flusso** , trova e trascina l’azione di flusso **Invia avviso** nell’area di lavoro.

   ![](assets/image2014-9-24-13-3a15-3a10.png)

1. Seleziona **My Alert Email** creato in precedenza e lascia **Invia a** come **Proprietario vendite**.

   ![](assets/eighteen-1.png)

1. Digita il tuo indirizzo e-mail nel campo **Fino ad altre e-mail** .

   ![](assets/nineteen-2.png)

1. Vai alla scheda **Pianificazione** e fai clic sul pulsante **Attiva** .

   ![](assets/twenty-2.png)

   >[!TIP]
   >
   >Imposta le **Regole di qualifica** su **ogni volta** (modificando la Smart Campaign) per consentire alla stessa persona di attivare gli avvisi più volte.

1. Fai clic su **Attiva** nella schermata di conferma.

   ![](assets/twenty-one-1.png)

## Passaggio 3: Testa fuori! {#step-test-it-out}

1. Seleziona la pagina di destinazione e fai clic su **Visualizza pagina approvata**.

   ![](assets/image2014-9-24-13-3a17-3a8.png)

   >[!NOTE]
   >
   >Non dimenticare di approvare le pagine di destinazione; non vanno in diretta fino all&#39;approvazione.

1. Compila il modulo e fai clic su **Invia**.

   ![](assets/image2014-9-24-13-3a17-3a41.png)

1. A breve riceverai la tua e-mail. Dopo aver verificato che tutto funziona come dovrebbe, rimuovi il tuo indirizzo e-mail dal flusso di avvisi di invio (vedi il passaggio 2.7 sopra).

   >[!NOTE]
   >
   >Fai clic sulla scheda **Informazioni persona** in Marketo per visualizzare le informazioni sul contatto.

## Missione Completa! {#mission-complete}

<br> 

[◄ Missione 7: Personalizzare un’e-mail](personalize-an-email.md)

[Missione 9 Aggiorna dati lead ►](update-person-data.md)
