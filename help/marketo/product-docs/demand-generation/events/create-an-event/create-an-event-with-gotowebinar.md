---
unique-page-id: 2949874
description: Creare un evento con GotoWebinar - Marketo Docs - Documentazione del prodotto
title: Creare un evento con GotoWebinar
exl-id: c0f0a202-e416-4523-b7d6-dbcfafc536cd
source-git-commit: 8b0625a7192a80986bc4295726cd13473493ddd7
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Creare un evento con GotoWebinar {#create-an-event-with-gotowebinar}

>[!PREREQUISITES]
>
>* [Aggiungi GoToWebinar come servizio LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-gotowebinar-as-a-launchpoint-service.md)
>* [Creare un nuovo programma evento](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Imposta il valore appropriato [azioni di flusso](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)tracciare il coinvolgimento


Crea prima il tuo webinar in GoToWebinar. Alcune impostazioni nella creazione del tuo GoToWebinar sono utilizzate da Marketo e alcune sono utilizzate solo da GoToWebinar.

Dopo aver creato un evento Marketo e associato il Webinar GoToWebinar, i sistemi saranno in grado di condividere le informazioni di registrazione e partecipazione.

Di seguito è riportato un elenco delle impostazioni utilizzate da Marketo.

## Titolo e descrizione {#title-and-description}

**Nome webinar** - immetti il nome del webinar. Questo nome sarà visibile in Marketo.

**Descrizione** (facoltativo) - immetti la descrizione del webinar. La descrizione sarà visibile in Marketo.

![](assets/image2015-5-28-15-3a1-3a36.png)

## Data e ora {#date-time}

Immetti le seguenti informazioni per il tuo webinar e verrà estratto in Marketo tramite l&#39;adattatore. Se apporti modifiche a queste informazioni, fai clic sul collegamento &quot;**Aggiorna da Webinar Provider**&quot; **Azioni evento** affinché Marketo possa visualizzare le modifiche.

**Data di inizio** - inserire la data di inizio. Questo sarà visibile in Marketo.

**Ora di inizio** - inserire l&#39;ora di inizio. Questo sarà visibile in Marketo.

**Ora di fine** - inserisci l&#39;ora di fine. Questo sarà visibile in Marketo.

**Fuso orario** - selezionare il fuso orario applicabile. Sarà visibile in Marketo.

**Tipo -** impostato su **Una sessione**.

![](assets/image2015-5-28-15-3a7-3a1.png)

>[!NOTE]
>
>Marketo al momento non supporta i webinar ricorrenti. È necessario impostare una singola sessione tra ciascun webinar Marketo Event e GoToWebinar.

>[!TIP]
>
>Se hai bisogno di ulteriore aiuto per GoToWebinar, visita la [Sito della Guida](https://support.logmeininc.com/gotowebinar).

Ora, saltiamo su Marketo!

1. Seleziona un evento. Fai clic su **Azioni evento** e scegli **Impostazioni evento**.

   ![](assets/image2015-5-14-14-3a53-3a10.png)

   >[!NOTE]
   >
   >Il tipo di canale dell’evento selezionato deve essere **webinar**.

1. Scegli **Webinar GoTo** dal **Partner evento** Elenco.

   ![](assets/image2015-5-14-14-3a55-3a20.png)

1. Scegli l&#39;account.

   ![](assets/rtaimage-2.png)

1. Seleziona il webinar.

   ![](assets/image2015-5-14-14-3a57-3a31.png)

1. Fai clic su **Salva**.

   ![](assets/image2015-5-14-14-3a58-3a54.png)

1. Eccellente! Ora l’evento viene sincronizzato e pianificato da **Webinar GoTo**.

   ![](assets/image2015-5-14-15-3a0-3a47.png)

   >[!NOTE]
   >
   >I campi inviati da Marketo sono: Nome, Cognome, Indirizzo E-Mail. Questi campi sono obbligatori e non devono essere vuoti.

   >[!TIP]
   >
   >Per popolare l’e-mail di conferma con questo URL univoco, utilizza il seguente token nella tua e-mail: `{{member.webinar url}}`. Quando l’URL di conferma viene inviato, questo token viene automaticamente risolto nell’URL di conferma univoco della persona.
   >
   >Imposta l’e-mail di conferma su **Operativo** per garantire che le persone che si registrano e possono essere cancellate ricevano comunque le informazioni di conferma.

   ![](assets/goto-webinar.png)

   >[!CAUTION]
   >
   >Evita di utilizzare programmi e-mail nidificati per inviare le e-mail di conferma. Utilizza invece la campagna intelligente del programma dell’evento, come illustrato in precedenza.

   >[!TIP]
   >
   >La visualizzazione dei dati in Marketo può richiedere fino a 48 ore. Se dopo aver aspettato così a lungo non vedi ancora nulla, seleziona **Aggiorna da Webinar Provider** dal menu Azioni evento in **Riepilogo** scheda dell’evento.

Le persone che si iscrivono al tuo webinar riceveranno un push al tuo provider tramite il passaggio Cambia lo stato del programma quando il nuovo stato è impostato su &quot;Registrato&quot;. Nessun altro stato invierà la persona. Inoltre, assicurati di fare il passaggio di flusso Modifica stato programma n. 1 e Invia passaggio di flusso e-mail n. 2.

## Visualizzazione della pianificazione  {#viewing-the-schedule}

Nella vista Programmazione programma fare clic sulla voce del calendario relativa all&#39;evento. La pianificazione viene visualizzata sul lato destro dello schermo.

>[!NOTE]
>
>Per modificare la pianificazione degli eventi, è necessario modificare il webinar su GoToWebinar.

![](assets/image2015-5-14-15-3a3-3a13.png)
