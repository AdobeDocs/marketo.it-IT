---
description: Creazione di un evento con Webex - Documentazione di Marketo - Documentazione del prodotto
title: Creare un evento con Webex
hide: true
hidefromtoc: true
feature: Events
source-git-commit: 286e1b7b563be70e932206adec6f80b4877b7953
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# Creare un evento con Webex {#create-an-event-with-webex}

>[!PREREQUISITES]
>
>* [Aggiungere Webex as a LaunchPoint Service](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [Creare un nuovo programma evento](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Impostare il [azioni di flusso](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) per tenere traccia del coinvolgimento

## Pianificare un webinar {#schedule-a-webinar}

Crea un webinar in [Webex](https://www.webex.com/){target="_blank"}. Marketo Engage only uses specific settings and fields for your integration, which we'll go through shortly. For additional information, please see the [Webex Webinars Help Documentation](https://help.webex.com/en-us/landing/ld-7srxjs-WebexWebinars/Webex-Webinars){target="_blank"}.

>[!NOTE]
>
>Puoi scegliere le impostazioni preferite in Webex, ma nel Marketo Engage sono visualizzabili solo le seguenti informazioni: nome del webinar, data e ora di inizio/fine, fuso orario e descrizione.

### Informazioni di base {#basic-information}

![](assets/create-an-event-with-webex-1.png)

* **Argomento**: questo è il nome del tuo evento e sarà visualizzabile in Marketo.
* **Data e ora**: in Marketo è possibile visualizzare data/fine, ora di inizio/fine, durata e fuso orario.
* **Numero massimo di partecipanti**: il numero massimo di partecipanti determina quali funzioni Webex sono supportate.
* **Visualizzazione Webcast per i partecipanti**: seleziona questa opzione per far sì che il webinar venga trasmesso in streaming a tutti i partecipanti.
* **Membri dei pannelli**: invita persone specifiche a diventare membri del gruppo nel tuo webinar.
* **Agenda del webinar**: compila questa opzione se desideri fornire il contesto nell’invito e-mail inviato ai membri del panelist.

### Sicurezza {#security}

![](assets/create-an-event-with-webex-2.png)

* **Password webinar**: (facoltativo) se utilizzi questo campo, assicurati di includerlo nell’e-mail di conferma.
* **Password del ruolo del pannello**: (facoltativo) se utilizzi questo campo, assicurati di includerlo nell’agenda del webinar.
* **Richiedi account**: limita i partecipanti solo a coloro che hanno account Webex.

### Opzioni di connessione audio {#audio-connection-options}

![](assets/create-an-event-with-webex-3.png)

* **Tipo di connessione audio**: scegli in che modo i partecipanti al webinar si uniscono alla parte audio del webinar.
* **Tono di entrata e uscita**: seleziona il suono desiderato per gli utenti quando qualcuno entra o esce dal webinar (è richiesta la connessione audio del telefono).
* **Disattiva audio panelist**: scegli le impostazioni di disattivazione audio del panelist desiderate.

### Opzioni avanzate {#advanced-options}

![](assets/create-an-event-with-webex-4.png)

* **Registrazione automatica**: seleziona questa opzione per registrare automaticamente il webinar.
* **Esercitazione**: selezionare questa opzione per avviare un&#39;esercitazione all&#39;inizio del webinar.
* **Sessioni Breakout**: le sessioni di suddivisione consentono di preassegnare i membri del gruppo e i partecipanti prima dell’inizio del webinar o di partecipare durante il webinar.
* **Serie di webinar**: l’aggiunta a una serie di webinar consente alle persone di vedere il webinar, che sia pubblico o meno.
* **Registrazione**: richiede ai partecipanti di registrarsi e ricevere l’approvazione dell’host prima di partecipare.
* **Promemoria e-mail**: scegli un promemoria e-mail che va da 15 minuti prima dell’inizio del webinar fino a due giorni.
* **Opzioni webinar**: determina le funzioni disponibili per i partecipanti al webinar.
* **Privilegi partecipante**: i privilegi dei partecipanti determinano le azioni disponibili per i partecipanti al webinar.

>[!NOTE]
>
>L’integrazione Marketo-Webex non supporta l’invio di e-mail di conferma da Webex. La conferma deve essere inviata tramite Marketo. Dopo aver pianificato l’evento, copia le informazioni sull’evento nell’e-mail di conferma di Marketo e imposta l’indirizzo e-mail come _Operativo_.

Ora siamo pronti a saltare in Marketo Engage!

## Sincronizza evento con Marketo Engage {#sync-your-event-with-marketo-engage}

1. In Marketo, individua e seleziona il Programma evento creato. In **Azioni evento** a discesa, seleziona **Impostazioni evento**.

   ![](assets/create-an-event-with-webex-5.png)

   >[!NOTE]
   >
   >Il tipo di canale dell’evento selezionato deve essere **webinar**.

1. In **Partner evento** a discesa, seleziona **Webinar Webex**.

   ![](assets/create-an-event-with-webex-6.png)

1. In **Login** , scegli il tuo accesso a Webex.

   ![](assets/create-an-event-with-webex-7.png)

1. In **Evento** , scegli il tuo evento Webex.

   ![](assets/create-an-event-with-webex-8.png)

1. I dettagli del webinar verranno compilati. Fai clic su **Salva**.

   ![](assets/create-an-event-with-webex-9.png)

Il tuo evento Webex è ora sincronizzato con il tuo evento Marketo. Le persone che si registrano al webinar verranno inviate al provider del webinar tramite _Modifica stato programma_ passaggio di flusso quando il nuovo stato è impostato su &quot;Registrato&quot;. Nessun altro stato spingerà la persona oltre. Assicurati di _Modifica stato programma_ #1 della fase di flusso e _Invia e-mail_ #2. passaggio di flusso

## Aspetti da considerare {#things-to-note}

* Evita di utilizzare i programmi e-mail nidificati per inviare le e-mail di conferma. Al suo posto, utilizza la campagna avanzata del programma per eventi.

* La visualizzazione dei dati in Marketo può richiedere fino a 48 ore. Se dopo aver atteso così a lungo non vedi ancora nulla, fai clic su **Aggiorna dal provider del webinar** nel **Azioni evento** menu a discesa nella **Riepilogo** del programma dell’evento.
