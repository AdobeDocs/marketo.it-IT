---
unique-page-id: 2949865
description: Creare un evento con Adobe Connect - Documentazione di Marketo - Documentazione del prodotto
title: Creare un evento con Adobe Connect
exl-id: 196b1640-9cfd-4485-9bc4-e907d3ac1f16
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Creare un evento con Adobe Connect {#create-an-event-with-adobe-connect}

La sincronizzazione con Adobe Connect consente di gestire la registrazione e la partecipazione ai webinar all’interno di Marketo, in modo da evitare che il coinvolgimento venga ignorato.

>[!PREREQUISITES]
>
>* [Collegare Adobe Connect e Marketo](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [Creare un nuovo programma evento](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)

Innanzitutto, assicurati di aver creato la riunione o il seminario in Adobe Connect. Se hai bisogno di aiuto, consulta [Guida utente di Adobe Connect](https://help.adobe.com/en_US/connect/9.0/using/index.html).

Le riunioni e i seminari creati in Adobe Connect devono essere creati nella cartella specificata al momento dell&#39;immissione delle credenziali in Marketo. Dopo aver creato la riunione o il seminario, prendere nota di tutte le informazioni logistiche pertinenti (ad esempio il numero di telefono) da utilizzare nell&#39;e-mail di conferma e nel file ICS.

>[!CAUTION]
>
>In qualità di host dell’evento, assicurati di partecipare dall’app e **non** tramite il collegamento inviato ai partecipanti.

>[!NOTE]
>
>Al momento Adobe Connect On-Site non è supportato.

1. Nella home di un nuovo evento, seleziona **Azioni evento**, e quindi **Impostazioni evento**.

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >Se non vedi **Impostazioni evento** nel menu a discesa, assicurati che il canale dell’evento abbia **Evento con webinar** selezionato in &quot;Si applica a&quot;.

1. Sotto **Partner evento**, seleziona **Adobe Connect**.

   ![](assets/event-settings-adobe-connect.png)

1. Seleziona il **Login** ID e seleziona il tuo **Evento**.

   ![](assets/event-settings-select-event-adobe-connect.png)

1. Clic **Salva**.

   ![](assets/event-settings-overview.png)

   Bello! L’evento Adobe Connect ora è sincronizzato con l’evento Marketo.

   >[!NOTE]
   >
   >I campi inviati da Marketo sono: Nome, Cognome, Indirizzo e-mail.

   >[!TIP]
   >
   >Per inserire l’URL univoco della persona in un’e-mail, utilizza questo token: `{{member.webinar url}}`. Quando l’e-mail viene inviata, questo token risolve automaticamente l’URL univoco di conferma della persona da Adobe Connect.
   >
   >Imposta l’e-mail di conferma su **Operativo** per garantire che le persone che si registrano e potrebbero annullare l’abbonamento ricevano comunque le informazioni di conferma.

   Le persone che si registrano al webinar verranno inviate al provider del webinar tramite il passaggio del flusso di stato del programma di modifica quando il nuovo stato è impostato su &quot;Registrato&quot;. Nessun altro stato spingerà la persona oltre. Inoltre, assicurati di #1 il passaggio di flusso Stato programma di modifica e il passaggio di flusso Invia e-mail #2.

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >Evita di utilizzare programmi e-mail nidificati per inviare le e-mail di conferma. Utilizza invece la campagna intelligente del programma dell’evento, come illustrato in precedenza.

   >[!TIP]
   >
   >La visualizzazione dei dati in Marketo può richiedere fino a 48 ore. Se dopo aver atteso a lungo non vedi ancora nulla, seleziona **Aggiorna dal provider del webinar** dal menu Azioni evento nella scheda Riepilogo dell’evento.

   >[!MORELIKETHIS]
   >
   >* [Aggiungere Adobe Connect as a LaunchPoint Service](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   >* [Modificare un canale eventi](/help/marketo/product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)
