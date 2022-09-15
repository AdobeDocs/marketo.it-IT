---
unique-page-id: 2359424
description: Avvisare il rappresentante commerciale - Marketo Docs - Documentazione del prodotto
title: Avvisare il rappresentante commerciale
exl-id: 4ad7d7b8-ee1e-4605-b4e0-e72a7e573c05
source-git-commit: 1127928b43762086ed4d157719ff80d6c3de9ee3
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Avvisare il rappresentante commerciale {#alert-the-sales-rep}

## Missione: Segnala al rappresentante commerciale quando una persona compila un modulo sul tuo sito web {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

Per inviare automaticamente le e-mail di avviso ai rappresentanti commerciali, tutto ciò di cui hai bisogno è un’e-mail di avviso e una campagna e-mail. Ecco come farlo.

>[!PREREQUISITES]
>
>[Pagina di destinazione con un modulo](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}

## Passaggio 1: Creare un messaggio e-mail di avviso {#step-create-an-alert-email}

1. Vai a **Attività di marketing** area.

   ![](assets/alert-the-sales-rep-1.png)

1. Seleziona **Il mio programma** creato in [Pagina di destinazione con un modulo](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;} vittoria rapida, quindi sotto **Nuovo** click **Nuova risorsa locale**.

   ![](assets/alert-the-sales-rep-2.png)

1. Fai clic su **E-mail**.

   ![](assets/alert-the-sales-rep-3.png)

1. **Nome** l&#39;e-mail &quot;My Email Alert&quot;, seleziona un modello e fai clic su **Crea**.

   ![](assets/alert-the-sales-rep-4.png)

1. Inserisci il **Nome da**, **Da e-mail**, **Risposta** e **Oggetto** che vuoi che il tuo team di vendita veda.

   ![](assets/alert-the-sales-rep-5.png)

1. Fai doppio clic per modificare il testo dell’e-mail.

   ![](assets/alert-the-sales-rep-6.png)

1. Digita il contenuto dell’e-mail.

   ![](assets/alert-the-sales-rep-7.png)

1. Posizionare il cursore nel punto in cui si desidera inserire le informazioni di contatto della persona e fare clic sul **Inserisci token** icona.

   ![](assets/alert-the-sales-rep-8.png)

1. Trova e seleziona la `{{SP_Send_Alert_Info}}` **Token** e fai clic su **Inserisci**.

   ![](assets/alert-the-sales-rep-9.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} è un token speciale per le e-mail di avviso. Vedi [Utilizzare il token di invio delle informazioni di avviso](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target=&quot;_blank&quot;}{target=&quot;_blank&quot;} per ulteriori informazioni.

1. Fai clic su **Salva**.

   ![](assets/alert-the-sales-rep-10.png)

1. Fai clic sul pulsante **Azioni e-mail** a discesa e seleziona **Approva e chiudi**.

   ![](assets/alert-the-sales-rep-11.png)

## Passaggio 2: Creare una campagna di attivazione degli avvisi {#step-create-an-alert-trigger-campaign}

1. Seleziona **Il mio programma** creato in precedenza, quindi in **Nuovo** click **Nuova campagna Smart**.

   ![](assets/alert-the-sales-rep-12.png)

1. **Nome** la campagna &quot;My Alert Campaign&quot; (Campagna di avviso personale) e fai clic su **Crea**.

   ![](assets/alert-the-sales-rep-13.png)

1. Sotto la **Elenco avanzato** , trova e trascina **Riempie il modulo** attiva l’area di lavoro.

   ![](assets/alert-the-sales-rep-14.png)

1. Selezionare il modulo creato in precedenza.

   ![](assets/alert-the-sales-rep-15.png)

1. Sotto la **Flusso** , trova e trascina **Invia avviso** azione di scorrimento nell&#39;area di lavoro.

   ![](assets/alert-the-sales-rep-16.png)

1. Seleziona **E-mail di avviso** creato in precedenza e lasciato **Invia a** come **Proprietario vendite**.

   ![](assets/alert-the-sales-rep-17.png)

1. Digita il tuo indirizzo e-mail nel **Ad altre e-mail** campo .

   ![](assets/alert-the-sales-rep-18.png)

1. Vai a **Pianificazione** e fai clic su **Attiva** pulsante .

   ![](assets/alert-the-sales-rep-19.png)

   >[!TIP]
   >
   >Imposta la **Regole di qualifica** a **ogni volta** (modificando Smart Campaign) per consentire alla stessa persona di attivare gli avvisi più volte.

1. Fai clic su **Attiva** nella schermata di conferma.

   ![](assets/alert-the-sales-rep-20.png)

## Passaggio 3: Testa fuori! {#step-test-it-out}

1. Seleziona la pagina di destinazione e fai clic su **Visualizza pagina approvata**.

   ![](assets/alert-the-sales-21.png)

   >[!NOTE]
   >
   >Non dimenticare di approvare le pagine di destinazione; non vanno in diretta fino all&#39;approvazione.

1. Compila il modulo e fai clic su **Invia**.

   ![](assets/alert-the-sales-22.png)

1. A breve riceverai la tua e-mail. Dopo aver verificato che tutto funziona come dovrebbe, rimuovi il tuo indirizzo e-mail dal flusso di avvisi di invio (vedi il passaggio 2.7 sopra).

   >[!NOTE]
   >
   >Fai clic sul pulsante **Informazioni sulla persona** scheda in Marketo per visualizzare le informazioni sul contatto.

## Missione Completa! {#mission-complete}

<br> 

[◄ Missione 7: Personalizzare un’e-mail](/help/marketo/getting-started/quick-wins/personalize-an-email.md)

[Missione 9 Aggiorna dati personali ►](/help/marketo/getting-started/quick-wins/update-person-data.md)
