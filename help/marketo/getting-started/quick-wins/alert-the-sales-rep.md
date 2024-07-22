---
unique-page-id: 2359424
description: Avvisa il rappresentante di vendita - Documentazione Marketo - Documentazione del prodotto
title: Avvisa il rappresentante commerciale
exl-id: 4ad7d7b8-ee1e-4605-b4e0-e72a7e573c05
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Avvisa il rappresentante commerciale {#alert-the-sales-rep}

## Missione: avvisa il rappresentante commerciale quando una persona compila un modulo sul sito web {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

Per inviare automaticamente e-mail di avviso agli agenti di vendita, devi solo inviare un’e-mail di avviso e una campagna e-mail. Ecco come farlo.

>[!PREREQUISITES]
>
>[Pagina di destinazione con modulo](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## Passaggio 1: creare un messaggio e-mail di avviso {#step-create-an-alert-email}

1. Vai all&#39;area **[!UICONTROL Attività di marketing]**.

   ![](assets/alert-the-sales-rep-1.png)

1. Seleziona **Il mio programma** che hai creato nella [Pagina di destinazione con un modulo](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} vinto rapidamente, quindi in **[!UICONTROL Nuovo]** fai clic su **[!UICONTROL Nuova risorsa locale]**.

   ![](assets/alert-the-sales-rep-2.png)

1. Fai clic su **[!UICONTROL E-mail]**.

   ![](assets/alert-the-sales-rep-3.png)

1. **Denomina** l&#39;e-mail &quot;Avviso e-mail&quot;, seleziona un modello e fai clic su **[!UICONTROL Crea]**.

   ![](assets/alert-the-sales-rep-4.png)

1. Immetti **Da nome**, **Da e-mail**, **[!UICONTROL Rispondi a]** e **[!UICONTROL Oggetto]** che desideri che il tuo team vendite veda.

   ![](assets/alert-the-sales-rep-5.png)

1. Fai doppio clic per modificare il testo dell’e-mail.

   ![](assets/alert-the-sales-rep-6.png)

1. Digita il contenuto dell’e-mail.

   ![](assets/alert-the-sales-rep-7.png)

1. Posiziona il cursore nel punto in cui vuoi inserire le informazioni di contatto della persona e fai clic sull&#39;icona **Inserisci token**.

   ![](assets/alert-the-sales-rep-8.png)

1. Trova e seleziona il `{{SP_Send_Alert_Info}}` **[!UICONTROL Token]** e fai clic su **[!UICONTROL Inserisci]**.

   ![](assets/alert-the-sales-rep-9.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} è un token speciale per le e-mail di avviso. Per ulteriori informazioni, consulta [Utilizzare il token di informazioni per l&#39;invio degli avvisi](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target="_blank"}{target="_blank"}.

1. Fai clic su **[!UICONTROL Salva]**.

   ![](assets/alert-the-sales-rep-10.png)

1. Fai clic sul menu a discesa **[!UICONTROL Azioni e-mail]** e seleziona **[!UICONTROL Approva e chiudi]**.

   ![](assets/alert-the-sales-rep-11.png)

## Passaggio 2: creare una campagna di attivazione degli avvisi {#step-create-an-alert-trigger-campaign}

1. Seleziona **Il mio programma** creato in precedenza, quindi in **[!UICONTROL Nuovo]** fai clic su **[!UICONTROL Nuova campagna avanzata]**.

   ![](assets/alert-the-sales-rep-12.png)

1. **Denomina** la campagna &quot;La mia campagna di avvisi&quot; e fai clic su **[!UICONTROL Crea]**.

   ![](assets/alert-the-sales-rep-13.png)

1. Nella scheda **[!UICONTROL Elenco avanzato]**, individua e trascina il trigger **[!UICONTROL Compila modulo]** nell&#39;area di lavoro.

   ![](assets/alert-the-sales-rep-14.png)

1. Seleziona il modulo creato in precedenza.

   ![](assets/alert-the-sales-rep-15.png)

1. Nella scheda **[!UICONTROL Flusso]**, individua e trascina l&#39;azione di flusso **[!UICONTROL Invia avviso]** nell&#39;area di lavoro.

   ![](assets/alert-the-sales-rep-16.png)

1. Seleziona **[!UICONTROL Il mio avviso e-mail]** creato in precedenza e lascia **[!UICONTROL Invia a]** come **[!UICONTROL Proprietario vendite]**.

   ![](assets/alert-the-sales-rep-17.png)

1. Digita il tuo indirizzo e-mail nel campo **[!UICONTROL Altre e-mail]**.

   ![](assets/alert-the-sales-rep-18.png)

1. Vai alla scheda **[!UICONTROL Pianifica]** e fai clic sul pulsante **[!UICONTROL Attiva]**.

   ![](assets/alert-the-sales-rep-19.png)

   >[!TIP]
   >
   >Imposta le **[!UICONTROL regole per la qualifica]** su **[!UICONTROL ogni volta]** (modificando Smart Campaign) per consentire alla stessa persona di attivare gli avvisi più volte.

1. Fai clic su **[!UICONTROL Attiva]** nella schermata di conferma.

   ![](assets/alert-the-sales-rep-20.png)

## Passaggio 3: Testarlo! {#step-test-it-out}

1. Seleziona la pagina di destinazione e fai clic su **[!UICONTROL Visualizza pagina approvata]**.

   ![](assets/alert-the-sales-21.png)

   >[!NOTE]
   >
   >Non dimenticare di approvare le pagine di destinazione, che verranno pubblicate solo dopo l’approvazione.

1. Compila il modulo e fai clic su **[!UICONTROL Invia]**.

   ![](assets/alert-the-sales-22.png)

1. Riceverai la tua e-mail a breve. Dopo aver verificato che tutto funzioni come previsto, rimuovi il tuo indirizzo e-mail dal flusso di invio degli avvisi (vedi il precedente passaggio 2.7).

   >[!NOTE]
   >
   >Fare clic sulla scheda **[!UICONTROL Informazioni persona]** in Marketo per visualizzare le informazioni di contatto.

## Missione completata! {#mission-complete}

<br> 

[◄ Mission 7: Personalizzare un’e-mail](/help/marketo/getting-started/quick-wins/personalize-an-email.md)

[Missione 9: aggiornare i dati ► persona](/help/marketo/getting-started/quick-wins/update-person-data.md)
