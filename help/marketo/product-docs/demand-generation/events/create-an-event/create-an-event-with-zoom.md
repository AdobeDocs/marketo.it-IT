---
unique-page-id: 17728023
description: Creare un evento con zoom - Documentazione di Marketo - Documentazione del prodotto
title: Creare un evento con zoom
exl-id: 6a2aec58-902c-4e40-ab59-9cc33ec83cea
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# Creare un evento con zoom {#create-an-event-with-zoom}

>[!PREREQUISITES]
>
>* [Aggiungere zoom come servizio LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-zoom-as-a-launchpoint-service.md)
>* [Creare un nuovo programma evento](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Impostare il [azioni di flusso](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)per tenere traccia del coinvolgimento

Crea il webinar in Zoom. Alcune impostazioni per la creazione dello zoom vengono utilizzate da Marketo, mentre altre vengono utilizzate solo da Zoom.

Dopo aver creato un evento Marketo e aver associato a esso un webinar Zoom, i sistemi saranno in grado di condividere le informazioni sulla registrazione e sulla partecipazione. Per assistenza nella creazione di un webinar, consulta  [Guida introduttiva ai webinar Zoom](https://support.zoom.us/hc/en-us/articles/200917029-Getting-Started-With-Webinar).

Immetti le seguenti informazioni per il webinar, che verranno inserite in Marketo tramite l’adattatore. Se apporti modifiche a queste informazioni, fai clic sul collegamento &quot;Aggiorna dal provider di webinar&quot; in Azioni evento per consentire a Marketo di visualizzare le modifiche.

**Titolo e descrizione**

* **Nome webinar** - Immetti il nome del webinar. Questo nome sarà visualizzabile in Marketo.

* **Descrizione** (facoltativo) - Immetti la descrizione del webinar. La descrizione sarà visibile in Marketo.

**Data e ora**

* **Data di inizio** - Inserire la data di inizio. Questo sarà visibile in Marketo.

* **Ora di inizio** - Immettere l&#39;ora di inizio. Questo sarà visibile in Marketo.

* **Durata** - Inserire la durata. L’ora di inizio e l’ora di fine saranno visualizzabili in Marketo.

* **Fuso orario** - Selezionare il fuso orario applicabile. Questo sarà visibile in Marketo.

* **Webinar ricorrente**- Mantieni deselezionato.

* **Registrazione** - Selezionare questa casella per richiedere la registrazione. Utilizzerai un modulo/pagina di destinazione Marketo per acquisire le informazioni di registrazione che verranno inviate a Zoom.

>[!NOTE]
>
>Al momento Marketo non supporta i webinar ricorrenti. Devi impostare una singola sessione tra ogni webinar Marketo Event e Zoom.

![](assets/overview2.png)

>[!TIP]
>
>Sono presenti campi aggiuntivi che verranno configurati in Zoom che NON influiranno sull’integrazione. Consulta la sezione [Centro assistenza per webinar Zoom](https://support.zoom.us/hc/en-us/sections/200324965-Video-Webinar) per ulteriori informazioni su questi campi.

Ora, saltiamo su Marketo!

1. Seleziona un evento. Clic **Azioni evento** e scegli **Impostazioni evento**.

   ![](assets/image2015-5-14-14-3a53-3a10-1.png)

   >[!NOTE]
   >
   >Il tipo di canale dell’evento selezionato deve essere **webinar**.

1. Scegli **Zoom** dal **Evento** **Partner** Elenco.

   ![](assets/eventsettings1.png)

1. Scegli l’account Zoom a cui associare l’evento.

   ![](assets/selectaccount.png)

1. Seleziona il webinar.

   ![](assets/selectevent.png)

1. Clic **Salva**.

   ![](assets/eventsettingssave.png)

   Eccellente! Ora l’evento viene sincronizzato e pianificato da Zoom.

   >[!NOTE]
   >
   >I campi inviati da Marketo sono: Nome, Cognome, Indirizzo e-mail.

   >[!TIP]
   >
   >Per compilare l’e-mail di conferma con questo URL univoco, utilizza il seguente token nell’e-mail: `{{member.webinar url}}`. Quando l’URL di conferma viene inviato, questo token viene automaticamente risolto nell’URL di conferma univoco della persona.
   >
   >Imposta l’e-mail di conferma su **Operativo** per garantire che le persone che si registrano e potrebbero annullare l’abbonamento ricevano comunque le informazioni di conferma.

   Le persone che si registrano al webinar verranno inviate al provider del webinar tramite **Modifica stato programma** passaggio di flusso quando il nuovo stato è impostato su &quot;Registrato&quot;. Nessun altro stato spingerà la persona oltre. Inoltre, assicurati di **Modifica stato programma** #1 della fase di flusso e **Invia e-mail** #2. passaggio di flusso

   ![](assets/goto-webinar-1.png)

   >[!CAUTION]
   >
   >Evita di utilizzare programmi e-mail nidificati per inviare le e-mail di conferma. Utilizza invece la campagna intelligente del programma dell’evento, come illustrato in precedenza.

   >[!TIP]
   >
   >La visualizzazione dei dati in Marketo può richiedere fino a 48 ore. Se dopo aver atteso a lungo non vedi ancora nulla, seleziona **Aggiorna dal provider del webinar** dal menu Azioni evento nel **Riepilogo** dell’evento.
