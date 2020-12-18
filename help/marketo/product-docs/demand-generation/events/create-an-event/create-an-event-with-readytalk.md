---
unique-page-id: 2949870
description: Creazione di un evento con ReadyTalk - Marketo Docs - Documentazione prodotto
title: Creazione di un evento con ReadyTalk
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---


# Creazione di un evento con ReadyTalk {#create-an-event-with-readytalk}

>[!PREREQUISITES]
>
>* [Aggiungi ReadyTalk come servizio LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-readytalk-as-a-launchpoint-service.md)
>* [Creare un nuovo programma evento](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Impostare le azioni di flusso [appropriate](http://docs.marketo.com/display/DOCS/Flow+Actions)per tenere traccia del coinvolgimento


Configurate innanzitutto l&#39;evento nel centro conferenze ReadyTalk. Se hai bisogno di aiuto, consulta il Centro risorse [ReadyTalk.](https://www.readytalk.com/resources/readytalk)  Quando scegliete il tipo di registrazione, selezionate  **preregistratevi prima della riunione**. Se selezionate *registratevi al momento della riunione*, Marketo **non** acquisirà uno stato Registrato per le persone e lo stato sarà solo per le persone che partecipano *dopo* il webinar si conclude.

Lasciare **avvisare l&#39;utente di nuove registrazioni via e-mail** non selezionata.

![](assets/image2015-5-28-21-3a18-3a39.png)

Se utilizzi ReadyTalk per inviare e-mail di conferma, dovrai anche aggiungere una descrizione. Al termine, salvate l’evento in ReadyTalk.

>[!NOTE]
>
>Per pianificare un evento assistito da un operatore, fate clic sul collegamento **Richiedi servizi evento** situato sul lato sinistro della schermata iniziale del Centro conferenze per pianificare un evento con il nostro team eventi.

Ora è possibile collegare l’evento a Marketo.

1. Selezionate l&#39;evento, quindi fate clic su **Azioni evento** e infine su **Impostazioni evento.**

   ![](assets/image2015-5-18-12-3a46-3a47.png)

   >[!NOTE]
   >
   >Il tipo di canale dell&#39;evento selezionato deve essere **webinar.**

1. In **Partner evento,** selezionare **ReadyTalk**.

   ![](assets/image2015-5-18-12-3a47-3a59.png)

1. In **Login,** selezionare il login di ReadyTalk.

   ![](assets/image2015-5-18-12-3a48-3a48.png)

1. In **Evento**, selezionare l&#39;evento da collegare, quindi fare clic su **Salva**.

   ![](assets/image2015-5-18-12-3a51-3a35.png)

   Bello! L&#39;evento è ora sincronizzato.

   >[!NOTE]
   >
   >I campi inviati da Marketo sono: Nome, Cognome, Indirizzo E-Mail.

   >[!TIP]
   >
   >Per compilare il messaggio e-mail di conferma con questo URL univoco, utilizzate il seguente token nel messaggio e-mail: `{{member.webinar url}}`. Quando l&#39;URL di conferma viene inviato, questo token viene automaticamente risolto nell&#39;URL di conferma univoco della persona.
   >
   >Impostate l&#39;e-mail di conferma su Operativo per fare in modo che le persone che si sono registrate, che potrebbero non essere sottoscritte, ricevano le informazioni di conferma.

   ![](assets/readytalk.png)

   >[!CAUTION]
   >
   >Evitate di utilizzare programmi e-mail nidificati per inviare le e-mail di conferma. Utilizzate invece la campagna intelligente del programma dell&#39;evento, come mostrato sopra.

   >[!TIP]
   >
   >La visualizzazione dei dati in Marketo può richiedere fino a 48 ore. Se dopo aver aspettato troppo a lungo non viene visualizzato nulla, selezionate **Aggiorna da provider webinar** dal menu Azioni evento nella scheda **Riepilogo** dell&#39;evento.

## Visualizzazione della pianificazione {#viewing-the-schedule}

Nella [vista programmazione programma](http://docs.marketo.com/display/docs/program+schedule+view), fare clic sulla voce del calendario relativa all&#39;evento. Potete visualizzare la pianificazione sul lato destro dello schermo!

![](assets/image2015-5-18-12-9-58.png)

Le persone che si iscrivono al webinar vengono inviate al provider del webinar tramite il passaggio Modifica stato programma quando il nuovo stato è impostato su &quot;Registrato&quot;. Nessun altro stato farà passare la persona. Inoltre, accertatevi che Modifica stato programma passi il passaggio 1 e Invia flusso e-mail il passaggio 2.
