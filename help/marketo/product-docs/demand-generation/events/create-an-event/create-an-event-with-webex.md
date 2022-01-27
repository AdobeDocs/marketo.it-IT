---
unique-page-id: 2949863
description: Creare un evento con WebEx - Documenti Marketo - Documentazione del prodotto
title: Crea un evento con WebEx
exl-id: 25266a6b-3951-46d1-8700-b36d7086ad2c
source-git-commit: ed9146f48aecd34025d61abf14d76a714726dcc9
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---

# Crea un evento con WebEx {#create-an-event-with-webex}

>[!PREREQUISITES]
>
>* [Aggiungere WebEx come servizio LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [Creare un nuovo programma evento](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Imposta il valore appropriato [azioni di flusso](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) tracciare il coinvolgimento
>* Assicurati di utilizzare Eventi Webex (classico)


Creare innanzitutto un evento Webex nel Centro eventi WebEx. Marketo utilizza solo impostazioni e campi specifici per l’integrazione, che verranno esaminati a breve. Gli altri campi che è possibile configurare per WebEx sono descritti nella sezione [Guida utente del Centro eventi WebEx](https://www.cisco.com/c/dam/en/us/td/docs/collaboration/meeting_center/wbs298/wx_ec_host_ug.pdf).

>[!IMPORTANT]
>
>Marketi Engage supporta solo gli eventi creati in Eventi Web (classic). Al momento, Marketo non supporta gli eventi creati in Eventi Web (nuovi).

## Informazioni di base {#basic-information}

* **Nome evento -** Questo nome sarà visibile in Marketo.
* **Casella di controllo non elencata**

   * Si consiglia di farlo **not** elenca l’evento. In questo modo tutte le persone si registreranno tramite la pagina di destinazione di Marketo. Le persone che si registrano attraverso un meccanismo diverso da Marketo verranno visualizzate in Marketo dopo la conclusione dell&#39;evento E solo se hanno partecipato all&#39;evento.
   * Se scegli di elencare l’evento, questo verrà visualizzato nella pagina Elenco eventi per chiunque visiti il sito web del Centro eventi.

* **Registrazione -** Selezionare questa casella per impostare su &quot;obbligatorio&quot;. Utilizzare un modulo Marketo/pagina di destinazione per acquisire le informazioni di registrazione che verranno inviate a WebEx.
* **Password evento**- (facoltativo) Se utilizzi questo campo assicurati di includerlo nell’e-mail di conferma!

![](assets/image2015-5-28-13-3a30-3a55.png)

## Data e ora {#date-time}

* **Data di inizio** - Inserire la data di inizio. Questo sarà visibile in Marketo.

* **Ora di inizio** - Inserire l&#39;ora di inizio. Questo sarà visibile in Marketo.

* **Durata stimata** - Specifica la durata dell’evento. Questo sarà visibile in Marketo.

* **Fusi orari** - Inserire i fusi orari applicabili. Saranno visualizzabili in Marketo.

![](assets/image2015-5-28-13-3a37-3a39.png)

## Impostazioni di audioconferenza {#audio-conference-settings}

Queste impostazioni risiedono solo in WebEx. Non sono utilizzati da o visualizzabili in Marketo, ma possono essere importanti per il tuo webinar, quindi controllali due volte!

## Descrizione dell’evento e opzioni  {#event-description-options}

Le seguenti opzioni sono utilizzate da o visualizzabili in Marketo. Gli altri campi risiedono solo in WebEx.

* **Descrizione** - Inserire una descrizione. Questo sarà visibile ma non modificabile in Marketo.
* **Sondaggio post-evento** - Al momento Marketo non è in grado di acquisire le informazioni su un sondaggio post-evento WebEx.
* **URL di destinazione** - (facoltativo) Puoi immettere l’URL di una pagina di destinazione Marketo da usare come URL di destinazione da visualizzare al termine della sessione.

![](assets/image2015-5-28-13-3a48-3a49.png)

## Partecipanti e registrazione {#attendees-registration}

Controllerai l’elenco degli inviti, il modulo di registrazione e altre e-mail utilizzando un evento Marketo. Altre funzionalità non saranno supportate da Marketo, tra cui:

* **Numero massimo di dichiaranti** - Attualmente **not** supportato tramite l&#39;integrazione Marketo-WebEx.  L&#39;approvazione manuale dei dichiaranti è disponibile utilizzando lo stato di avanzamento dell&#39;approvazione in sospeso in Marketo.

* **ID registrazione richiesto** - Attualmente supportato tramite l’integrazione Marketo-WebEx. Puoi utilizzare Marketo per inviare l’e-mail di conferma dell’evento. Quando la persona si registra, riceve un URL univoco che utilizza per accedere all’evento.

   >[!TIP]
   >
   >Per popolare l’e-mail di conferma con questo URL univoco, utilizza il seguente token nella tua e-mail: `{{member.webinar url}}`. Quando l’URL di conferma viene inviato, questo token viene automaticamente risolto nell’URL di conferma univoco della persona.
   >
   >Imposta l’e-mail di conferma su **Operativo** per garantire che le persone che si registrano e possono essere cancellate ricevano comunque le informazioni di conferma.

* **Password registrazione** - (Facoltativo) Attualmente non supportato con l&#39;integrazione Marketo-WebEx.
* **Regole di approvazione** - Attualmente non supportato tramite l&#39;integrazione Marketo-WebEx. Tuttavia, è possibile utilizzare campagne intelligenti in Marketo per controllare le approvazioni.

![](assets/image2015-5-28-14-3a4-3a41.png)

### Presentatori e pannelli {#presenters-panelists}

Le informazioni configurate in questa sezione non vengono trasmesse a Marketo.

### Messaggi e-mail {#email-messages}

Utilizzerai Marketo per inviare e-mail ai tuoi utenti registrati, e-mail di conferma, ecc. Non è necessario configurare nulla in questa sezione. Disattiva (deseleziona) le opzioni del messaggio e-mail all&#39;interno di WebEx.

![](assets/image2015-5-28-14-3a9-3a14.png)

>[!NOTE]
>
>L&#39;integrazione Marketo-WebEx non supporta l&#39;invio di e-mail di conferma da WebEx. La conferma deve essere inviata tramite Marketo. Dopo aver pianificato l’evento, assicurati di copiare le informazioni sull’evento nell’e-mail di conferma di Marketo e impostare l’e-mail come **Operativo**.

Ora siamo pronti per entrare in Marketo!

1. Seleziona l’evento creato. Apri **Azioni evento** a discesa. Scegli **Impostazioni evento.**

   ![](assets/image2015-5-14-16-3a7-3a31.png)

   >[!NOTE]
   >
   >Il tipo di canale dell’evento selezionato deve essere **webinar**.

1. Sotto **Partner evento**, seleziona **WebEx**.

   ![](assets/image2015-1-30-13-3a58-3a2.png)

1. Sotto **Login**, scegli l&#39;accesso a WebEx.

   ![](assets/image2015-5-18-12-3a2-3a26.png)

1. Sotto **Evento**, scegli l&#39;evento WebEx appena creato. Quindi, seleziona una pagina di backup facoltativa e fai clic su **Salva**.

   ![](assets/image2015-5-14-16-3a15-3a55.png)

1. Selezionare una pagina di backup facoltativa per l&#39;evento WebEx. Scegli dall’elenco a discesa delle pagine di destinazione Marketo approvate o immetti l’URL di una pagina di destinazione non Marketo.

   >[!TIP]
   >
   >Imposta una pagina di backup per indirizzare un membro a una pagina specifica se fa clic sull&#39;URL dell&#39;evento personalizzato prima dell&#39;ora di inizio dell&#39;evento.

   >[!NOTE]
   >
   >I campi inviati da Marketo sono: Nome, Cognome, Indirizzo E-Mail.

   ![](assets/webex.png)

   >[!CAUTION]
   >
   >Evita di utilizzare programmi e-mail nidificati per inviare le e-mail di conferma. Utilizza invece la campagna intelligente del programma dell’evento, come illustrato in precedenza.

   >[!TIP]
   >
   >La visualizzazione dei dati in Marketo può richiedere fino a 48 ore. Se dopo aver aspettato così a lungo non vedi ancora nulla, seleziona **Aggiorna da Webinar Provider** dal menu Azioni evento in **Riepilogo** scheda dell’evento.

Dolce! L&#39;evento WebEx viene ora sincronizzato con l&#39;evento Marketo.  Le persone che si iscrivono al tuo webinar riceveranno un push al tuo provider tramite il passaggio Cambia lo stato del programma quando il nuovo stato è impostato su &quot;Registrato&quot;. Nessun altro stato invierà la persona. Inoltre, assicurati di fare il passaggio di flusso Modifica stato programma n. 1 e Invia passaggio di flusso e-mail n. 2.

## Visualizzazione della pianificazione  {#viewing-the-schedule}

Nella vista Programmazione programma fare clic sulla voce del calendario relativa all&#39;evento. Puoi visualizzare la pianificazione sul lato destro dello schermo!

![](assets/image2015-5-14-16-3a21-3a41.png)

>[!NOTE]
>
>Per modificare la pianificazione degli eventi è necessario modificare il webinar su WebEx.
