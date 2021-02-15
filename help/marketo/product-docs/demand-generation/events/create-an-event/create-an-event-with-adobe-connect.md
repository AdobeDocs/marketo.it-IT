---
unique-page-id: 2949865
description: Creazione di un evento con  Adobe Connect - Marketo Docs - Documentazione prodotto
title: Creare un evento con  Adobe Connect
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---


# Creare un evento con  Adobe Connect {#create-an-event-with-adobe-connect}

La sincronizzazione con  Adobe Connect consente di gestire la registrazione e la partecipazione al webinar all&#39;interno di Marketo, il che assicura che il coinvolgimento non venga interrotto.

>[!PREREQUISITES]
>
>* [Collegamento  Adobe Connect e Marketo](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [Creare un nuovo programma evento](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)


Innanzitutto, accertatevi di aver creato la riunione o il seminario in  Adobe Connect. Per assistenza, consultare la [ Guida utente di Adobe Connect](https://help.adobe.com/en_US/connect/9.0/using/index.html). Le riunioni e i seminari creati in  Adobe Connect devono essere creati nella cartella specificata al momento dell&#39;immissione delle credenziali in Marketo. Dopo aver creato la riunione o il seminario, prendete nota di tutte le informazioni logistiche rilevanti (come il numero di telefono), da utilizzare nel file di conferma e-mail e ICS.

>[!NOTE]
>
>Al momento **non** supporta  Adobe Connect On-Site.

1. A casa di un nuovo evento, selezionare **Azioni evento**, quindi **Impostazioni evento**.

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >Se nel menu a discesa non viene visualizzato **Impostazioni evento**, assicurarsi che il canale dell&#39;evento sia selezionato in &quot;Applicabile a&quot;.****

1. In **Partner evento**, selezionare **Adobe Connect**.

   ![](assets/event-settings-adobe-connect.png)

1. Selezionare l&#39;ID **Login** e selezionare l&#39;ID **Evento**.

   ![](assets/event-settings-select-event-adobe-connect.png)

1. Fare clic su **Salva**.

   ![](assets/event-settings-overview.png)

   Bello! L&#39;evento Adobe Connect  ora è sincronizzato con l&#39;evento Marketo.

   >[!NOTE]
   >
   >I campi inviati da Marketo sono: Nome, Cognome, Indirizzo E-Mail.

   >[!TIP]
   >
   >Per inserire l’URL univoco della persona in un messaggio e-mail, utilizzate questo token: `{{member.webinar url}}`. Quando l’e-mail viene inviata, questo token risolve automaticamente l’URL di conferma univoco della persona da  Adobe Connect.
   >
   >Impostate l&#39;e-mail di conferma su **Operativo** per assicurare che le persone che si sono registrate e che potrebbero essere annullate la sottoscrizione continuino a ricevere le informazioni di conferma.

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >Evitate di utilizzare programmi e-mail nidificati per inviare le e-mail di conferma. Utilizzate invece la campagna intelligente del programma dell&#39;evento, come mostrato sopra.

   >[!TIP]
   >
   >La visualizzazione dei dati in Marketo può richiedere fino a 48 ore. Se dopo aver aspettato per un periodo di tempo tale da non visualizzare nulla, selezionate **Aggiorna da provider webinar** dal menu Azioni evento nella scheda Riepilogo dell&#39;evento.

   >[!MORELIKETHIS]
   >
   > * [Aggiungere  Adobe Connect come servizio LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   > * [Modifica di un canale evento](/help/marketo/product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)


Le persone che si iscrivono al webinar vengono inviate al provider del webinar tramite il passaggio Modifica stato programma quando il nuovo stato è impostato su &quot;Registrato&quot;. Nessun altro stato farà passare la persona. Inoltre, accertatevi che Modifica stato programma passi il passaggio 1 e Invia flusso e-mail il passaggio 2.
