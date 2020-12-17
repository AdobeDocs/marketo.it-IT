---
unique-page-id: 1900581
description: Inoltro a un collegamento amico nelle e-mail - Documenti Marketo - Documentazione prodotto
title: Inoltra a un collegamento amico nelle e-mail
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 0%

---


# Inoltra a un collegamento amico nelle e-mail {#forward-to-a-friend-link-in-emails}

L&#39;aggiunta del collegamento &quot;Inoltra a amico&quot; alle e-mail consente di tenere traccia delle persone che hanno ricevuto un&#39;e-mail inoltrata tramite questo collegamento e di aggiungerle automaticamente come nuova persona, se non sono già presenti nel database.

Ad esempio, Keith utilizza il collegamento &quot;Inoltra all’amico&quot; per inoltrare l’e-mail a una persona sconosciuta, Mark. Mark viene aggiunto automaticamente come persona nuova, viene assegnato il proprio cookie e una qualsiasi delle sue attività e-mail e web è collegata a lui. Tuttavia, se Keith utilizza il pulsante di inoltro nel client di posta elettronica, Mark riceve un cookie non corretto come Keith e la sua attività viene registrata come Keith.

## Aggiungere il collegamento a un modello e-mail {#add-the-link-to-an-email-template}

1. Andate a **Design Studio**.

   ![](assets/one-8.png)

1. Individuate e selezionate il modello e-mail a cui desiderate aggiungere il collegamento. Fare clic su **Modifica bozza**.

   ![](assets/two-7.png)

1. Incollate il seguente codice HTML in cui desiderate visualizzare il collegamento &quot;Inoltra a amico&quot; (se avete bisogno di aiuto con questa parte, conferitelo allo sviluppatore Web):

   `<pre data-theme="Confluence"><a href="{{system.forwardToFriendLink}}">Forward to Friend</a></pre>`

   ![](assets/three-7.png)

   >[!TIP]
   >
   >
   >Puoi aggiungere lo stile al collegamento per renderlo più piacevole. Ad esempio:
   >
   >`<a href="{{system.forwardToFriendLink}}" style="font-family:arial, sans-serif; padding:10px; position:absolute; right:0px;">Forward to Friend</a>`

   >[!CAUTION]
   >
   >Non è consigliabile utilizzare lo stile **position:relative** nel modello e-mail. Può creare problemi con la posizione e la visualizzazione della casella &quot;Inoltra all&#39;amico&quot;.

1. Fare clic su **Anteprima bozza** per verificare che il modello sia nel modo desiderato.

   ![](assets/four-5.png)

   >[!NOTE]
   >
   >**Promemoria**
   >
   >Ricordate di approvare la bozza del modello per applicare le modifiche.

   Ora tutte le e-mail che utilizzano tale modello avranno il collegamento &quot;Inoltra all&#39;amico&quot;. Quando il destinatario dell&#39;e-mail fa clic su di esso, verrà indirizzato a una versione Web dell&#39;e-mail con la casella &quot;Inoltra a un amico&quot;:
   ![](assets/f2afbox.png)

## Aggiungere il collegamento a un&#39;e-mail singola {#add-the-link-to-an-individual-email}

Puoi anche aggiungere il collegamento &quot;Inoltra a amico&quot; direttamente in un&#39;e-mail.

1. Aprite il messaggio e-mail in cui desiderate includere il collegamento e fate doppio clic nell’area modificabile.

   ![](assets/five-4.png)

1. Posizionare il cursore nel punto in cui si desidera visualizzare il collegamento e fare clic sul pulsante **Inserisci token**.

   ![](assets/six-2.png)

1. Selezionare il token **`{{system.forwardToFriendLink}}`**.

   ![](assets/seven-1.png)

   >[!NOTE]
   >
   >Questo token è l’URL della versione Web dell’e-mail con la casella &quot;Inoltra all’amico&quot;.

1. Indicare il testo da visualizzare del collegamento (ad esempio, &quot;Inoltra a un amico&quot;).

   ![](assets/seven-1.png)

1. Tagliate il token **`{{system.forwardToFriendLink}}`** utilizzando Ctrl+X (Windows) o Cmd+X (Mac). Evidenziare &quot;Inoltra a un amico&quot; e fare clic sul pulsante **Inserisci/Modifica collegamento**.

   ![](assets/eight-1.png)

1. Incollate il token **`{{system.forwardToFriendLink}}`** nella casella **URL** utilizzando Ctrl/Cmd+V, quindi fate clic su** Inserisci**.

   ![](assets/nine.png)

1. Salva la modifica e visualizza in anteprima il nuovo collegamento!

   ![](assets/ten-1.png)

   >[!NOTE]
   >
   >Per impostazione predefinita, le nuove persone che vengono aggiunte ricevendo un messaggio e-mail di tipo &quot;Inoltra a un amico&quot; vengono annullate dalla sottoscrizione alle e-mail di marketing.

## Visualizza attività di inoltro {#view-forwarding-activity}

Puoi vedere chi ha inoltrato e ricevuto le e-mail nel log delle attività della persona.

1. Passare alla cartella **`Database`**.

   ![](assets/db.png)

1. Fate doppio clic sulla persona per la quale desiderate visualizzare l&#39;attività.

   ![](assets/fourteen.png)

1. Passate alla scheda **Activity Log**. Fare doppio clic su **Ricevuto e-mail a amico** o **Inviato a e-mail amico** per visualizzare i dettagli.

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >**Definizione**
   >
   >
   >Per E-mail ricevuta da un amico, l’ID persona è la persona che ha inoltrato l’e-mail.
   >
   >
   >Per Invia a e-mail amico, l’ID persona è la persona che ha ricevuto l’e-mail.

   ![](assets/sixteen.png)

1. Per visualizzare una persona per ID, copiate e incollate l&#39;** ID persona** alla fine dell&#39;URL (l&#39;inizio di tale URL dipende dall&#39;istanza di Marketo):

   `<pre data-theme="Confluence">...marketo.com/Database/loadPersonDetail?personId=</pre>`

   >[!NOTE]
   >
   >Facendo clic sull&#39; **ID persona** e collegandoci direttamente alla persona in una patch imminente.

   ![](assets/seventeen.png)

   >[!NOTE]
   >
   >Se l&#39;amico che riceve l&#39;inoltro è una persona sconosciuta, viene creata una nuova persona con &quot;Inoltra all&#39;amico&quot; contrassegnato come **Origine** della persona.\
   >Se l&#39;e-mail è una risorsa locale di un programma, il programma è contrassegnato come **Programma di acquisizione della persona**.

## Trigger o Filtro utilizzando l&#39;attività di inoltro {#trigger-or-filter-using-forwarding-activity}

Esistono sei attivatori/filtri che puoi usare per attivare azioni di flusso o filtrare le persone mediante l’attività &quot;Inoltra all’amico&quot; inviata e ricevuta.

Nell&#39;elenco smart della campagna, se cercate &quot;avanti&quot;, troverete le attivazioni e i filtri disponibili.

![](assets/nineteen.png)

## Test inoltrato all&#39;amico {#test-forward-to-friend}

Per testare ‘Inoltra all’amico’, inviatevi un’e-mail con il collegamento in avanti. Assicurarsi di inviarlo tramite il passaggio di flusso **Invia e-mail**, *not* tramite **Invia e-mail di prova**.
