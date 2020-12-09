---
unique-page-id: 2949863
description: Creazione di un evento con WebEx - Marketo Docs - Documentazione prodotto
title: Creazione di un evento con WebEx
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '940'
ht-degree: 0%

---


# Creazione di un evento con WebEx {#create-an-event-with-webex}

>[!PREREQUISITES]
>
>* [Aggiungi WebEx come servizio LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [Creare un nuovo programma evento](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Imposta le [azioni di flusso appropriate](http://docs.marketo.com/display/DOCS/Flow+Actions)per monitorare il coinvolgimento


Creare innanzitutto un evento Webex nel Centro eventi WebEx. Marketo utilizza solo impostazioni e campi specifici per l’integrazione, che verranno esaminati a breve. Altri campi che è possibile configurare per WebEx sono descritti nella Guida [utente del Centro eventi](http://www.cisco.com/c/dam/en/us/td/docs/collaboration/meeting_center/wbs298/wx_ec_host_ug.pdf)WebEx.

## Informazioni di base {#basic-information}

* **Nome evento -** Questo nome sarà visibile in Marketo.
* **Casella di controllo non elencata**

   * Si consiglia di **non** elencare l’evento. In questo modo tutte le persone si registreranno nella pagina di destinazione Marketo. Le persone che si registrano attraverso un meccanismo diverso da Marketo verranno visualizzate a Marketo dopo la conclusione dell&#39;evento E solo se hanno partecipato all&#39;evento.
   * Se scegliete di elencare l’evento, questo verrà visualizzato nella pagina Elenco eventi per chiunque visiti il sito Web del Centro eventi.

* **Registrazione -** Selezionare questa casella per impostare su &quot;obbligatorio&quot;. Utilizzerete un modulo Marketo/pagina di destinazione per acquisire le informazioni di registrazione che verranno inviate a WebEx.
* **Password** evento- (facoltativo) Se utilizzate questo campo, assicuratevi di includerlo nel messaggio e-mail di conferma!

![](assets/image2015-5-28-13-3a30-3a55.png)

## Data e ora {#date-time}

* **Data** inizio - Inserisci la data di inizio. Questo sarà visibile in Marketo.

* **Ora** inizio - Inserisci l&#39;ora di inizio. Questo sarà visibile in Marketo.

* **Durata** stimata - Specificate la durata dell&#39;evento. Questo sarà visibile in Marketo.

* **Fusi orari** - Inserire i fusi orari applicabili. Saranno visualizzabili a Marketo.

![](assets/image2015-5-28-13-3a37-3a39.png)

## Impostazioni audioconferenza {#audio-conference-settings}

Queste impostazioni risiedono solo in WebEx. Non sono né utilizzati né visualizzabili in Marketo, ma possono essere importanti per il webinar, quindi controllateli due volte!

## Descrizione evento e opzioni  {#event-description-options}

Le seguenti opzioni sono utilizzate da o visualizzabili in Marketo. Gli altri campi risiedono solo in WebEx.

* **Descrizione** - Immettete una descrizione. Questo sarà visibile ma non modificabile in Marketo.
* **Sondaggio** post-evento - Al momento, Marketo non è in grado di acquisire le informazioni in un sondaggio post-evento WebEx.
* **URL** di destinazione - (facoltativo) Potete immettere l&#39;URL di una pagina di destinazione Marketo da usare come URL di destinazione da visualizzare al termine della sessione.

![](assets/image2015-5-28-13-3a48-3a49.png)

## Partecipanti e registrazione {#attendees-registration}

Controllerete l’elenco di inviti, il modulo di registrazione e altre e-mail mediante un evento Marketo. Altre funzionalità non saranno supportate da Marketo, tra cui:

* **Numero massimo di utenti registrati** - Attualmente **non** supportato tramite l&#39;integrazione Marketo-WebEx.  L&#39;approvazione manuale degli utenti registrati è disponibile utilizzando lo stato In attesa di approvazione a Marketo.

* **ID registrazione richiesto** - Attualmente supportato con l&#39;integrazione Marketo-WebEx. Potete utilizzare Marketo per inviare l&#39;e-mail di conferma dell&#39;evento. Quando la persona si registra, riceve un URL univoco che utilizza per entrare nell’evento.

   >[!TIP]
   >
   >Per compilare il messaggio e-mail di conferma con questo URL univoco, utilizzate il seguente token nel messaggio e-mail: `{{member.webinar url}}`. Quando l&#39;URL di conferma viene inviato, questo token viene automaticamente risolto nell&#39;URL di conferma univoco della persona.
   >
   >Impostate l&#39;e-mail di conferma su **Operativo** per assicurare che le persone che si sono registrate e che potrebbero essere annullate la sottoscrizione continuino a ricevere le informazioni di conferma.

* **Password** registrazione - (facoltativo) Attualmente non supportata tramite l&#39;integrazione Marketo-WebEx.
* **Regole** di approvazione: al momento non supportato con l&#39;integrazione di Marketo-WebEx. Tuttavia, puoi utilizzare campagne intelligenti in Marketo per controllare le approvazioni.

![](assets/image2015-5-28-14-3a4-3a41.png)

### Presentatori e pannelli {#presenters-panelists}

Le informazioni configurate in questa sezione non vengono trasmesse a Marketo.

### Messaggi e-mail {#email-messages}

Utilizzerete Marketo per inviare e-mail ai vostri utenti registrati, e-mail di conferma, ecc. Non è necessario configurare nulla in questa sezione. Disattiva (deseleziona) le opzioni del messaggio e-mail in WebEx.

![](assets/image2015-5-28-14-3a9-3a14.png)

>[!NOTE]
>
>L&#39;integrazione di Marketo-WebEx non supporta l&#39;invio di e-mail di conferma da WebEx. La conferma deve essere inviata tramite Marketo. Dopo aver pianificato l’evento, accertatevi di copiare le informazioni sull’evento nell’e-mail di conferma di Marketo e impostare l’e-mail come **Operativa**.

Ora siamo pronti a saltare a Marketo!

1. Selezionate l’evento che avete creato. Aprite il menu a discesa Azioni **** evento. Scegliete Impostazioni **evento.**

   ![](assets/image2015-5-14-16-3a7-3a31.png)

   >[!NOTE]
   >
   >Il tipo di canale dell&#39;evento selezionato deve essere **webinar**.

1. In Partner **** evento, selezionare **WebEx**.

   ![](assets/image2015-1-30-13-3a58-3a2.png)

1. In **Accesso**, scegli il tuo login WebEx.

   ![](assets/image2015-5-18-12-3a2-3a26.png)

1. In **Evento**, scegliete l&#39;evento WebEx appena creato. Quindi, selezionate una pagina di backup facoltativa e fate clic su **Salva**.

   ![](assets/image2015-5-14-16-3a15-3a55.png)

1. Selezionare una pagina di backup opzionale per l&#39;evento WebEx. Scegliete dall’elenco a discesa delle pagine di destinazione Marketo approvate o immettete l’URL di una pagina di destinazione non Marketo.

   >[!TIP]
   >
   >Impostate una pagina di backup per indirizzare un membro a una pagina specifica se fa clic sull&#39;URL dell&#39;evento personalizzato prima dell&#39;ora di inizio dell&#39;evento.

   >[!NOTE]
   >
   >I campi inviati da Marketo sono: Nome, Cognome, Indirizzo E-Mail.

   ![](assets/webex.png)

   >[!CAUTION]
   >
   >Evitate di utilizzare programmi e-mail nidificati per inviare le e-mail di conferma. Utilizzate invece la campagna intelligente del programma dell&#39;evento, come mostrato sopra.

   >[!TIP]
   >
   >La visualizzazione dei dati in Marketo può richiedere fino a 48 ore. Se dopo aver aspettato troppo tempo non viene visualizzato nulla, selezionate **Aggiorna dal provider** webinar dal menu Azioni evento nella scheda **Riepilogo** dell’evento.

Dolce! L&#39;evento WebEx ora è sincronizzato con l&#39;evento Marketo.  Le persone che si iscrivono al webinar vengono inviate al provider del webinar tramite il passaggio Modifica stato programma quando il nuovo stato è impostato su &quot;Registrato&quot;. Nessun altro stato farà passare la persona. Inoltre, accertatevi che Modifica stato programma passi il passaggio 1 e Invia flusso e-mail il passaggio 2.

## Visualizzazione della pianificazione  {#viewing-the-schedule}

Nella vista [Pianificazione](http://docs.marketo.com/display/docs/program+schedule+view)programma, fate clic sulla voce del calendario relativa all&#39;evento. Potete visualizzare la pianificazione sul lato destro dello schermo!

![](assets/image2015-5-14-16-3a21-3a41.png)

>[!NOTE]
>
>Per modificare la pianificazione dell&#39;evento, dovrete modificare il webinar su WebEx.
