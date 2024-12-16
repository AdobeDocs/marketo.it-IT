---
unique-page-id: 17728023
description: Creare un evento con zoom - Documentazione di Marketo - Documentazione del prodotto
title: Creare un evento con zoom
exl-id: 6a2aec58-902c-4e40-ab59-9cc33ec83cea
feature: Events
source-git-commit: c10ecc0ccad28f2e480343acefe10f5eca2ae578
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# Creare un evento con zoom {#create-an-event-with-zoom}

>[!PREREQUISITES]
>
>* [Aggiungi zoom come servizio LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-zoom-as-a-launchpoint-service.md)
>* [Crea un nuovo programma eventi](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Imposta le [azioni di flusso](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) appropriate per tenere traccia del coinvolgimento

Crea il webinar in Zoom. Alcune impostazioni per la creazione dello zoom vengono utilizzate da Marketo, mentre altre vengono utilizzate solo da Zoom.

Dopo aver creato un evento Marketo e aver associato a esso un webinar Zoom, i sistemi saranno in grado di condividere le informazioni sulla registrazione e sulla partecipazione. Per informazioni sulla creazione di un webinar, vedere [Guida introduttiva ai webinar Zoom](https://support.zoom.us/hc/en-us/articles/200917029-Getting-Started-With-Webinar).

Immetti le seguenti informazioni per il webinar, che verranno inserite in Marketo tramite l’adattatore. Se apporti modifiche a queste informazioni, fai clic sul collegamento &quot;Aggiorna dal provider di webinar&quot; in Azioni evento per consentire a Marketo di visualizzare le modifiche.

**Titolo e descrizione**

* **Nome webinar** - Immettere il nome del webinar. Questo nome sarà visualizzabile in Marketo.

* **Descrizione** (facoltativo): immettere la descrizione del webinar. La descrizione sarà visibile in Marketo.

**Data e ora**

* **Data inizio** - Immettere la data di inizio. Questo sarà visibile in Marketo.

* **Ora di inizio** - Immettere l&#39;ora di inizio. Questo sarà visibile in Marketo.

* **Durata** - Immettere la durata. L’ora di inizio e l’ora di fine saranno visualizzabili in Marketo.

* **Fuso orario** - Seleziona il fuso orario applicabile. Questo sarà visibile in Marketo.

* **Webinar ricorrente**- Non selezionare.

* **Registrazione** - Selezionare questa casella per rendere obbligatoria la registrazione. Utilizzerai un modulo/pagina di destinazione Marketo per acquisire le informazioni di registrazione che verranno inviate a Zoom.

>[!NOTE]
>
>Al momento Marketo non supporta i webinar ricorrenti. Devi impostare una singola sessione tra ogni webinar Marketo Event e Zoom.

![](assets/overview2.png)

>[!TIP]
>
>Sono presenti campi aggiuntivi che verranno configurati in Zoom che NON influiranno sull’integrazione. Per ulteriori informazioni su questi campi, consultare il [Centro assistenza per webinar Zoom](https://support.zoom.us/hc/en-us/sections/200324965-Video-Webinar).

Ora, saltiamo su Marketo!

1. Seleziona un evento. Fai clic su **Azioni evento** e scegli **Impostazioni evento**.

   ![](assets/image2015-5-14-14-3a53-3a10-1.png)

   >[!NOTE]
   >
   >Il tipo di canale dell&#39;evento selezionato deve essere **webinar**.

1. Scegli **Zoom** dall&#39;elenco **Evento** **Partner**.

   ![](assets/eventsettings1.png)

1. Scegli l’account Zoom a cui associare l’evento.

   ![](assets/selectaccount.png)

1. Seleziona il webinar.

   ![](assets/selectevent.png)

1. Fai clic su **Salva**.

   ![](assets/eventsettingssave.png)

   Eccellente! Ora l’evento viene sincronizzato e pianificato da Zoom.

   >[!NOTE]
   >
   >I campi inviati da Marketo sono: Nome, Cognome, Indirizzo e-mail.

   >[!TIP]
   >
   >Per compilare l&#39;e-mail di conferma con questo URL univoco, utilizza il seguente token nell&#39;e-mail: `{{member.webinar url}}`. Quando l’URL di conferma viene inviato, questo token viene automaticamente risolto nell’URL di conferma univoco della persona.
   >
   >Imposta l&#39;e-mail di conferma su **Operativo** per garantire che le persone che si registrano e potrebbero annullare l&#39;iscrizione ricevano comunque le informazioni di conferma.

   Le persone che si registrano al webinar verranno inviate al provider del webinar tramite il passaggio di flusso **Modifica stato programma** quando il nuovo stato è impostato su &quot;Registrato&quot;. Nessun altro stato spingerà la persona oltre. Assicurati inoltre di #1 #2. il passaggio di flusso **Modifica stato programma** e il passaggio di flusso **Invia e-mail**

   ![](assets/goto-webinar-1.png)

   >[!CAUTION]
   >
   >Evita di utilizzare programmi e-mail nidificati per inviare le e-mail di conferma. Utilizza invece la campagna intelligente del programma dell’evento, come illustrato in precedenza.

   >[!TIP]
   >
   >La visualizzazione dei dati in Marketo può richiedere fino a 48 ore. Se dopo aver atteso così a lungo non trovi ancora nulla, seleziona **Aggiorna dal provider webinar** dal menu Azioni evento nella scheda **Riepilogo** dell&#39;evento, quindi fai clic sull&#39;icona di aggiornamento in basso a destra dello schermo.
