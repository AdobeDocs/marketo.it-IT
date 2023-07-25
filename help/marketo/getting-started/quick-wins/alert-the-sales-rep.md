---
unique-page-id: 2359424
description: Avvisa il rappresentante di vendita - Documentazione Marketo - Documentazione del prodotto
title: Avvisa il rappresentante commerciale
exl-id: 4ad7d7b8-ee1e-4605-b4e0-e72a7e573c05
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# Avvisa il rappresentante commerciale {#alert-the-sales-rep}

## Missione: avvisa il rappresentante commerciale quando una persona compila un modulo sul sito web {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

Per inviare automaticamente e-mail di avviso agli agenti di vendita, devi solo inviare un’e-mail di avviso e una campagna e-mail. Ecco come farlo.

>[!PREREQUISITES]
>
>[Pagina di destinazione con un modulo](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## Passaggio 1: creare un messaggio e-mail di avviso {#step-create-an-alert-email}

1. Vai a **[!UICONTROL Attività di marketing]** area.

   ![](assets/alert-the-sales-rep-1.png)

1. Seleziona **Il mio programma** che hai creato in [Pagina di destinazione con un modulo](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} vittoria rapida, quindi sotto **[!UICONTROL Nuovo]** click **[!UICONTROL Nuova risorsa locale]**.

   ![](assets/alert-the-sales-rep-2.png)

1. Clic **[!UICONTROL E-mail]**.

   ![](assets/alert-the-sales-rep-3.png)

1. **Nome** nell’e-mail &quot;Il mio avviso e-mail&quot;, seleziona un modello e fai clic su **[!UICONTROL Crea]**.

   ![](assets/alert-the-sales-rep-4.png)

1. Inserisci il **Nome mittente**, **Da e-mail**, **[!UICONTROL Risposta]**, e **[!UICONTROL Oggetto]** che vuoi far vedere al tuo sales team.

   ![](assets/alert-the-sales-rep-5.png)

1. Fai doppio clic per modificare il testo dell’e-mail.

   ![](assets/alert-the-sales-rep-6.png)

1. Digita il contenuto dell’e-mail.

   ![](assets/alert-the-sales-rep-7.png)

1. Posizionare il cursore nel punto in cui si desidera inserire le informazioni di contatto della persona e fare clic sul pulsante **Inserisci token** icona.

   ![](assets/alert-the-sales-rep-8.png)

1. Trova e seleziona la `{{SP_Send_Alert_Info}}` **[!UICONTROL Token]** e fai clic su **[!UICONTROL Inserisci]**.

   ![](assets/alert-the-sales-rep-9.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} è un token speciale per le e-mail di avviso. Consulta [Utilizza il token di informazioni sull’invio dell’avviso](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target="_blank"}{target="_blank"} per ulteriori informazioni.

1. Clic **[!UICONTROL Salva]**.

   ![](assets/alert-the-sales-rep-10.png)

1. Fai clic su **[!UICONTROL Azioni e-mail]** a discesa e selezionare **[!UICONTROL Approva e chiudi]**.

   ![](assets/alert-the-sales-rep-11.png)

## Passaggio 2: creare una campagna di attivazione degli avvisi {#step-create-an-alert-trigger-campaign}

1. Seleziona **Il mio programma** creato in precedenza, quindi in **[!UICONTROL Nuovo]** click **[!UICONTROL Nuova campagna avanzata]**.

   ![](assets/alert-the-sales-rep-12.png)

1. **Nome** la campagna &quot;La mia campagna di avvisi&quot; e fai clic su **[!UICONTROL Crea]**.

   ![](assets/alert-the-sales-rep-13.png)

1. Sotto **[!UICONTROL Elenco avanzato]** , trovare e trascinare il **[!UICONTROL Compila modulo]** attiva l’area di lavoro.

   ![](assets/alert-the-sales-rep-14.png)

1. Seleziona il modulo creato in precedenza.

   ![](assets/alert-the-sales-rep-15.png)

1. Sotto **[!UICONTROL Flusso]** , trovare e trascinare il **[!UICONTROL Invia avviso]** eseguire l’azione di flusso nell’area di lavoro.

   ![](assets/alert-the-sales-rep-16.png)

1. Seleziona **[!UICONTROL E-mail avviso personale]** creato in precedenza e lascia **[!UICONTROL Invia a]** as **[!UICONTROL Proprietario vendite]**.

   ![](assets/alert-the-sales-rep-17.png)

1. Digita il tuo indirizzo e-mail in **[!UICONTROL Ad Altre E-Mail]** campo.

   ![](assets/alert-the-sales-rep-18.png)

1. Vai a **[!UICONTROL Pianificazione]** e fai clic sul pulsante **[!UICONTROL Attiva]** pulsante.

   ![](assets/alert-the-sales-rep-19.png)

   >[!TIP]
   >
   >Imposta il **[!UICONTROL Regole di qualificazione]** a **[!UICONTROL ogni volta]** (modificando Smart Campaign) per consentire alla stessa persona di attivare gli avvisi più volte.

1. Clic **[!UICONTROL Attiva]** nella schermata di conferma.

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
   >Fai clic su **[!UICONTROL Informazioni persona]** in Marketo per visualizzare le informazioni di contatto.

## Missione completata! {#mission-complete}

<br> 

[◄ Mission 7: Personalizzare un’e-mail](/help/marketo/getting-started/quick-wins/personalize-an-email.md)

[Missione 9: aggiornare i dati ► persona](/help/marketo/getting-started/quick-wins/update-person-data.md)
