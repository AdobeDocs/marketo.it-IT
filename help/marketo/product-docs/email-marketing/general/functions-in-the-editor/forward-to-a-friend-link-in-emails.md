---
unique-page-id: 1900581
description: Inoltrare a un amico Link nelle e-mail - Documentazione di Marketo - Documentazione del prodotto
title: Inoltra a un collegamento amico nelle e-mail
exl-id: 7addac65-4207-419f-845c-d6b2d08d299c
feature: Email Editor
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 0%

---

# Inoltra a un collegamento amico nelle e-mail {#forward-to-a-friend-link-in-emails}

L’aggiunta del collegamento &quot;Inoltra all’amico&quot; alle e-mail consente di tenere traccia delle persone che hanno ricevuto un’e-mail inoltrata tramite questo collegamento e di aggiungerle automaticamente come nuova persona se non sono già presenti nel database.

Ad esempio, supponiamo che Keith utilizzi il collegamento &#39;Inoltra all&#39;amico&#39; per inoltrare l&#39;e-mail a una persona sconosciuta, Mark. Mark viene aggiunto automaticamente come nuova persona, gli viene assegnato un cookie personale e una qualsiasi delle sue attività e-mail e web è collegata a lui. Tuttavia, se Keith usa il pulsante di inoltro nel suo client e-mail, Mark viene erroneamente ricattato come Keith e la sua attività viene registrata come Keith.

## Aggiungere il collegamento a un modello e-mail {#add-the-link-to-an-email-template}

1. Passare a **[!UICONTROL Design Studio]**.

   ![](assets/one-8.png)

1. Trova e seleziona il modello e-mail a cui desideri aggiungere il collegamento. Fai clic su **[!UICONTROL Edit Draft]**.

   ![](assets/two-7.png)

1. Incolla il seguente codice HTML dove vuoi che appaia il collegamento &#39;Inoltra all&#39;amico&#39; (se hai bisogno di aiuto con questa parte, contatta il tuo sviluppatore web):

   `<a href="{{system.forwardToFriendLink}}">Forward to Friend</a>`

   ![](assets/three-7.png)

   >[!TIP]
   >
   >
   >Puoi aggiungere al collegamento uno stile che ne faciliti l’aspetto. Ad esempio:
   >
   >`<a href="{{system.forwardToFriendLink}}" style="font-family:arial, sans-serif; padding:10px; position:absolute; right:0px;">Forward to Friend</a>`

   >[!CAUTION]
   >
   >Non è consigliabile utilizzare lo stile **position:relative** nel modello di messaggio di posta elettronica. Potrebbe causare problemi nella posizione e visualizzazione della casella &#39;Inoltra a amico&#39;.

1. Fare clic su **[!UICONTROL Preview Draft]** per verificare che l&#39;aspetto del modello sia quello desiderato.

   ![](assets/four-5.png)

   >[!NOTE]
   >
   >Ricordati di approvare la bozza del modello per applicare le modifiche.

   Ora tutte le e-mail che utilizzano quel modello avranno il collegamento &quot;Inoltra a amico&quot;. Quando il destinatario dell’e-mail fa clic su di essa, viene visualizzata una versione web dell’e-mail con la casella &quot;Inoltra a un amico&quot;:

   ![](assets/f2afbox.png)

## Aggiungere il collegamento a una singola e-mail {#add-the-link-to-an-individual-email}

Puoi anche aggiungere il collegamento &quot;Inoltra all’amico&quot; direttamente in un’e-mail.

1. Apri l’e-mail in cui desideri includere il collegamento e fai doppio clic nell’area modificabile.

   ![](assets/five-4.png)

1. Posizionare il cursore nel punto in cui si desidera visualizzare il collegamento e fare clic sul pulsante **Inserisci token**.

   ![](assets/six-2.png)

1. Selezionare il token **`{{system.forwardToFriendLink}}`**.

   ![](assets/seven-1.png)

   >[!NOTE]
   >
   >Questo token è l’URL della versione web dell’e-mail con una casella &quot;Inoltra all’amico&quot;.

1. Scrivi il testo da visualizzare sul collegamento, ad esempio &quot;Inoltra a un amico&quot;.

   ![](assets/seven-1.png)

1. Tagliare il token **`{{system.forwardToFriendLink}}`** utilizzando Ctrl+X (Windows) o Comando+X (Mac). Evidenziare &quot;Inoltra a un amico&quot; e fare clic sul pulsante **Inserisci/Modifica collegamento**.

   ![](assets/eight-1.png)

1. Incollare il token **`{{system.forwardToFriendLink}}`** nella casella **URL** utilizzando Ctrl/Comando+V, quindi fare clic su **[!UICONTROL Insert]**.

   ![](assets/nine.png)

1. Salva la modifica e visualizza l’anteprima del nuovo collegamento.

   ![](assets/ten-1.png)

   >[!NOTE]
   >
   >Per impostazione predefinita, i nuovi utenti che vengono aggiunti tramite la ricezione di un’e-mail di inoltro a un amico non sono iscritti alle e-mail di marketing.

## Visualizza attività di inoltro {#view-forwarding-activity}

Puoi vedere chi ha inoltrato e ricevuto le e-mail nel registro attività della persona.

1. Passare a **[!UICONTROL Database]**.

   ![](assets/db.png)

1. Fai doppio clic sulla persona per la quale desideri visualizzare l’attività.

   ![](assets/fourteen.png)

1. Passa alla scheda **[!UICONTROL Activity Log]**. Fare doppio clic su **[!UICONTROL Received Forward to Friend Email]** o **[!UICONTROL Sent Forward to Friend Email]** per visualizzare i dettagli.

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >**Definizione**
   >
   >Per Ricevuto Inoltra a e-mail amico, l’ID persona è la persona che ha inoltrato l’e-mail.
   >
   >Per Inoltra a e-mail amico, l’ID persona è la persona che ha ricevuto l’e-mail.

   ![](assets/sixteen.png)

1. Per visualizzare una persona per ID, copia e incolla **ID persona** alla fine dell&#39;URL (l&#39;inizio dell&#39;URL dipenderà dall&#39;istanza di Marketo):

   `...marketo.com/Database/loadPersonDetail?personId=`

   >[!NOTE]
   >
   >In una patch successiva, sarà possibile fare clic su **[!UICONTROL Person ID]** e collegarsi direttamente alla persona.

   ![](assets/seventeen.png)

   >[!NOTE]
   >
   >Se l&#39;amico che riceve l&#39;inoltro è una persona sconosciuta, viene creato un nuovo utente con &#39;Inoltra all&#39;amico&#39; contrassegnato come **Source** dell&#39;utente.
   >Se l&#39;e-mail è una risorsa locale di un programma, il programma viene contrassegnato come **Programma di acquisizione** della persona.

## Attivare o filtrare tramite attività di inoltro {#trigger-or-filter-using-forwarding-activity}

Puoi utilizzare sei trigger o filtri per attivare le azioni di flusso o filtrare le persone in base all’attività &quot;Inoltra a un amico&quot; inviata e ricevuta.

Nell’elenco smart di una campagna, se cerchi &quot;inoltra&quot; troverai i trigger e i filtri disponibili.

![](assets/nineteen.png)

## Inoltra test ad amico {#test-forward-to-friend}

Per verificare &quot;Inoltra ad amico&quot;, invia un&#39;e-mail con il collegamento di inoltro. Assicurati di inviarlo tramite il passaggio di flusso **Invia e-mail**, *non* tramite **Invia e-mail di prova**.
