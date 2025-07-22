---
unique-page-id: 17728023
description: Creazione di un evento con  [!DNL Zoom] - Documentazione di Marketo - Documentazione del prodotto
title: Crea un evento con  [!DNL Zoom]
exl-id: 6a2aec58-902c-4e40-ab59-9cc33ec83cea
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 0%

---

# Crea un evento con [!DNL Zoom] {#create-an-event-with-zoom}

>[!PREREQUISITES]
>
>* [Aggiungi [!DNL Zoom] come  [!DNL LaunchPoint] Servizio](/help/marketo/product-docs/administration/additional-integrations/add-zoom-as-a-launchpoint-service.md)
>* [Crea un nuovo programma eventi](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Imposta le [azioni di flusso](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) appropriate per tenere traccia del coinvolgimento

Crea il tuo webinar in [!DNL Zoom]. Alcune impostazioni nella creazione di [!DNL Zoom] sono utilizzate da Marketo, altre solo da [!DNL Zoom].

Dopo la creazione di un evento Marketo e l&#39;associazione di un webinar [!DNL Zoom], i sistemi potranno condividere le informazioni sulla registrazione e sulla partecipazione. Per informazioni sulla creazione di un webinar, vedere [Guida introduttiva di [!DNL Zoom] webinar](https://support.zoom.us/hc/en-us/articles/200917029-Getting-Started-With-Webinar).

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

* **Registrazione** - Selezionare questa casella per rendere obbligatoria la registrazione. Verrà utilizzato un modulo/pagina di destinazione di Marketo per acquisire le informazioni di registrazione che verranno inviate a [!DNL Zoom].

>[!NOTE]
>
>Al momento Marketo non supporta i webinar ricorrenti. È necessario impostare una singola sessione tra ogni evento Marketo e [!DNL Zoom] webinar.

![](assets/overview2.png)

>[!TIP]
>
>Sono presenti campi aggiuntivi che verranno configurati in [!DNL Zoom] che NON influiranno sull&#39;integrazione. Fare riferimento al [[!DNL Zoom] Centro assistenza webinar](https://support.zoom.us/hc/en-us/sections/200324965-Video-Webinar) per ulteriori informazioni su questi campi.

Ora, saltiamo su Marketo!

1. Seleziona un evento. Fare clic su **[!UICONTROL Event Actions]** e scegliere **[!UICONTROL Event Settings]**.

   ![](assets/image2015-5-14-14-3a53-3a10-1.png)

   >[!NOTE]
   >
   >Il tipo di canale dell&#39;evento selezionato deve essere **webinar**.

1. Scegliere **[!UICONTROL Zoom]** dall&#39;elenco **[!UICONTROL Event Partner]**.

   ![](assets/eventsettings1.png)

1. Scegliere l&#39;account [!DNL Zoom] a cui associare l&#39;evento.

   ![](assets/selectaccount.png)

1. Seleziona il webinar.

   ![](assets/selectevent.png)

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/eventsettingssave.png)

   Eccellente! Ora l&#39;evento è sincronizzato e pianificato da [!DNL Zoom].

   >[!NOTE]
   >
   >I campi inviati da Marketo sono: Nome, Cognome, Indirizzo e-mail.

   >[!TIP]
   >
   >Per compilare l&#39;e-mail di conferma con questo URL univoco, utilizza il seguente token nell&#39;e-mail: `{{member.webinar url}}`. Quando l’URL di conferma viene inviato, questo token viene automaticamente risolto nell’URL di conferma univoco della persona.
   >
   >Imposta l&#39;e-mail di conferma su **Operativo** per garantire che le persone che si registrano e potrebbero annullare l&#39;iscrizione ricevano comunque le informazioni di conferma.

   Le persone che si registrano al webinar verranno inviate al provider del webinar tramite il passaggio di flusso **[!UICONTROL Change Program Status]** quando [!UICONTROL New Status] è impostato su &quot;Registrato&quot;. Nessun altro stato spingerà la persona oltre. Assicurarsi inoltre di #1 **[!UICONTROL Change Program Status]** passaggio di flusso e #2. **[!UICONTROL Send Email]** passaggio di flusso

   ![](assets/goto-webinar-1.png)

   >[!CAUTION]
   >
   >Evita di utilizzare programmi e-mail nidificati per inviare le e-mail di conferma. Utilizza invece la campagna intelligente del programma dell’evento, come illustrato in precedenza.

   >[!TIP]
   >
   >La visualizzazione dei dati in Marketo può richiedere fino a 48 ore. Se dopo aver atteso così a lungo non trovi ancora nulla, seleziona **Aggiorna dal provider webinar** dal menu Azioni evento nella scheda **Riepilogo** dell&#39;evento, quindi fai clic sull&#39;icona di aggiornamento in basso a destra dello schermo.
