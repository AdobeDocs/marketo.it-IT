---
unique-page-id: 2949865
description: Creare un evento con Adobe Connect - Documentazione Marketo - Documentazione del prodotto
title: Creare un evento con Adobe Connect
exl-id: 196b1640-9cfd-4485-9bc4-e907d3ac1f16
source-git-commit: d81a4a3caa12c5ec642afadf9328b3825bde6fed
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Creare un evento con Adobe Connect {#create-an-event-with-adobe-connect}

La sincronizzazione con Adobe Connect ti consente di gestire la registrazione e la partecipazione al webinar all’interno di Marketo, in modo da evitare che il coinvolgimento venga rimosso.

>[!PREREQUISITES]
>
>* [Collegamento Adobe Connect e Marketo](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [Creare un nuovo programma evento](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)


In primo luogo, assicurati di aver creato la riunione o il seminario in Adobe Connect. Se hai bisogno di aiuto, consulta la sezione [Guida utente di Adobe Connect](https://help.adobe.com/en_US/connect/9.0/using/index.html).

Le riunioni e i seminari creati in Adobe Connect devono essere creati nella cartella specificata al momento dell&#39;immissione delle credenziali in Marketo. Dopo aver creato la riunione o il seminario, prendere nota di tutte le informazioni logistiche rilevanti (come il numero di telefono), da utilizzare nel file di conferma e-mail e ICS.

>[!CAUTION]
>
>In qualità di host dell’evento, assicurati di partecipare dall’app e **not** tramite il collegamento inviato ai partecipanti.

>[!NOTE]
>
>Al momento non è supportato Adobe Connect On-Site.

1. Nella home di un nuovo evento, seleziona **Azioni evento** e quindi **Impostazioni evento**.

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >Se non vedi **Impostazioni evento** nel menu a discesa , assicurati che il canale dell’evento abbia **Evento con Webinar** selezionato in &quot;Si applica a&quot;.

1. Sotto **Partner evento**, seleziona **Adobe Connect**.

   ![](assets/event-settings-adobe-connect.png)

1. Seleziona la tua **Login** ID e seleziona il tuo **Evento**.

   ![](assets/event-settings-select-event-adobe-connect.png)

1. Fai clic su **Salva**.

   ![](assets/event-settings-overview.png)

   Bello! L’evento Adobe Connect viene ora sincronizzato con l’evento Marketo.

   >[!NOTE]
   >
   >I campi inviati da Marketo sono: Nome, Cognome, Indirizzo E-Mail.

   >[!TIP]
   >
   >Per inserire l’URL univoco della persona in un’e-mail, utilizza questo token: `{{member.webinar url}}`. Quando l’e-mail viene inviata, questo token risolve automaticamente l’URL di conferma univoco della persona da Adobe Connect.
   >
   >Imposta l’e-mail di conferma su **Operativo** per garantire che le persone che si registrano e possono essere cancellate ricevano comunque le informazioni di conferma.

   Le persone che si iscrivono al tuo webinar riceveranno un push al tuo provider tramite il passaggio Cambia lo stato del programma quando il nuovo stato è impostato su &quot;Registrato&quot;. Nessun altro stato invierà la persona. Inoltre, assicurati di fare il passaggio di flusso Modifica stato programma n. 1 e Invia passaggio di flusso e-mail n. 2.

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >Evita di utilizzare programmi e-mail nidificati per inviare le e-mail di conferma. Utilizza invece la campagna intelligente del programma dell’evento, come illustrato in precedenza.

   >[!TIP]
   >
   >La visualizzazione dei dati in Marketo può richiedere fino a 48 ore. Se dopo aver aspettato così a lungo non vedi ancora nulla, seleziona **Aggiorna da Webinar Provider** dal menu Azioni evento nella scheda Riepilogo dell’evento.

   >[!MORELIKETHIS]
   >
   >* [Aggiungere Adobe Connect as a LaunchPoint Service](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   >* [Modificare un canale evento](/help/marketo/product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)

