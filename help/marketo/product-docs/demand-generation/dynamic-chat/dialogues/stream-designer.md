---
description: Stream Designer - Documenti Marketo - Documentazione del prodotto
title: Stream Designer
exl-id: aa44c7a5-f81b-4029-a1a4-5439bea83847
source-git-commit: 3883f31e59e4ba2dccf53961068fea7d5f805192
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Progettazione flussi {#stream-designer}

Ci sono _molti_ combinazioni di flussi che è possibile creare. Questo articolo contiene un esempio in cui l’addetto al marketing chiede al visitatore del sito se ha delle domande sul prodotto. Se sì, il visitatore può pianificare un appuntamento. In caso contrario, al visitatore viene offerta la possibilità di partecipare a una mailing list per la corrispondenza futura. L&#39;obiettivo è pianificare un appuntamento o raccogliere l&#39;e-mail del visitatore.

## Schede di Stream Designer {#stream-designer-cards}

Il designer del flusso contiene più schede che è possibile aggiungere per modellare la conversazione di chat.

<table>
 <tr>
  <td><strong>Messaggio</strong></td>
  <td>Utilizzare quando si desidera eseguire un'istruzione senza alcuna risposta necessaria (ad esempio: "Ciao! Tutti gli articoli sono 25% off oggi con codice SAVE25").
</td>
 </tr>
 <tr>
  <td><strong>Domanda</strong></td>
  <td>Utilizzare quando si desidera porre una domanda a scelta multipla, di cui fornire le risposte disponibili (ad esempio: A che tipo di veicolo ti interessa? Risposte = SUV, compatto, camion, ecc.).</td>
 </tr>
 <tr>
  <td><strong>Documento</strong></td>
  <td>Consente di incorporare i documenti PDF nelle finestre di dialogo e di tenere traccia dell’attività di coinvolgimento dei visitatori nei documenti (quante pagine sono state visualizzate, se il documento è stato scaricato e/o eventuali termini di ricerca utilizzati).</td>
 </tr>
 <tr>
  <td><strong>Acquisizione delle informazioni</strong></td>
  <td>Utilizza quando desideri raccogliere informazioni. I tre campi tra cui scegliere sono Indirizzo e-mail, Numero di telefono e Testo (che consente al visitatore di scrivere il proprio messaggio).</td>
 </tr>
 <tr>
  <td><strong>Pianificatore appuntamenti</strong></td>
  <td>Fornisce al visitatore un calendario delle date disponibili per pianificare un follow-up. La disponibilità del calendario riflette <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing">l'agente successivo in linea</a>.</td>
 </tr>
 <tr>
  <td><strong>Obiettivo</strong></td>
  <td>Questa è l'unica carta che i visitatori non vedranno. Sta a te determinare a quale punto un obiettivo viene raggiunto all'interno della chat specifica (es: se la raccolta dell'e-mail del visitatore è l'obiettivo, posiziona la scheda Obiettivo subito dopo l'acquisizione delle informazioni nello streaming).</td>
 </tr>
</table>

## Creare un flusso {#create-a-stream}

1. Dopo [crea la finestra di dialogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}, fai clic sul pulsante **Progettazione flussi** scheda .

   ![](assets/create-a-stream-1.png)

1. Trascinare la scheda Domanda.

   ![](assets/create-a-stream-2.png)

1. Sotto Chatbot Response, indica come ti piacerebbe.

   ![](assets/create-a-stream-3.png)

   >[!NOTE]
   >
   >Poke è impostato su on per impostazione predefinita, che visualizza la domanda di apertura accanto all&#39;icona della chat senza che il visitatore debba fare clic su di esso per vederlo.

1. Immetti le risposte utente e fai clic su **Salva**.

   ![](assets/create-a-stream-4.png)

1. Per &quot;Sì&quot; vogliamo pianificare un appuntamento, quindi sotto questa opzione trascina sulla scheda Scheduler Appointment.

   ![](assets/create-a-stream-5.png)

1. Nella colonna a destra, fai clic su **Salva**.

   ![](assets/create-a-stream-6.png)

1. Poiché si tratta di un obiettivo, trascina la scheda Obiettivo sotto l’Utilità di pianificazione degli appuntamenti.

   ![](assets/create-a-stream-7.png)

1. Denomina l&#39;obiettivo (o sceglierne uno esistente) e fai clic su **Salva**.

   ![](assets/create-a-stream-8.png)

1. Per &quot;No&quot; vogliamo vedere se si uniranno alla mailing list, quindi sotto quell&#39;opzione trascina su un&#39;altra scheda Domanda.

   ![](assets/create-a-stream-9.png)

1. Immetti la risposta e aggiungi le scelte di risposta per il visitatore. Fai clic su **Salva** al termine.

   ![](assets/create-a-stream-10.png)

   >[!NOTE]
   >
   >Per aggiungere altre risposte, fai clic su **Aggiungi risposta**.

1. Sotto la risposta &quot;Sì&quot;, trascina sulla scheda Info Capture per raccogliere l&#39;e-mail del visitatore.

   ![](assets/create-a-stream-11.png)

1. Fai clic sul pulsante **Tipo** a discesa e seleziona **E-mail**.

   ![](assets/create-a-stream-12.png)

1. Inserisci un messaggio chatbot e un segnaposto. Assicurati che l&#39;attributo sia mappato sul campo appropriato in Marketo e fai clic su **Salva**.

   ![](assets/create-a-stream-13.png)

   <table>
    <tr>
     <td><strong>Tipo</strong></td>
     <td>Tipo di informazioni da acquisire: Telefono, Testo, E-Mail.</td>
    </tr>
    <tr>
     <td><strong>Messaggio del chatbot</strong></td>
     <td>Il messaggio visualizzato dal visitatore richiede l’immissione delle informazioni.</td>
    </tr>
    <tr>
     <td><strong>Segnaposto</strong></td>
     <td>Testo di esempio che aiuta il visitatore a vedere cosa immettere.</td>
    </tr>
    <tr>
     <td><strong>Mappa risposta all'attributo</strong></td>
     <td>Consente di sincronizzare la risposta del visitatore al campo corrispondente nel record Persona nell’abbonamento Marketo.</td>
    </tr>
   </table>

1. Poiché la raccolta delle e-mail è un obiettivo, trascina la scheda Obiettivo sotto Info Capture (Acquisizione informazioni).

   ![](assets/create-a-stream-14.png)

1. Denomina l&#39;obiettivo (o sceglierne uno esistente) e fai clic su **Salva**.

   ![](assets/create-a-stream-15.png)

1. Ricordatevi di aggiungere una risposta se dicono &quot;No&quot;. Trascina una scheda Messaggio sotto quell’opzione.

   ![](assets/create-a-stream-16.png)

1. Inserisci il messaggio e fai clic su **Salva**.

   ![](assets/create-a-stream-17.png)

1. Seleziona la **Anteprima** per visualizzare l’anteprima della finestra di dialogo.

   ![](assets/create-a-stream-18.png)

1. Quando sei pronto per attivare la finestra di dialogo, fai clic su **Pubblica**.

   ![](assets/create-a-stream-19.png)

>[!NOTE]
>
>Prima di fare clic su Pubblica, ricorda di avere [ha inserito gli URL di destinazione](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md#target){target=&quot;_blank&quot;}.

>[!MORELIKETHIS]
>
>* [Creare una finestra di dialogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}
>* [Criteri del pubblico](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md){target=&quot;_blank&quot;}
>* [Rapporti](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target=&quot;_blank&quot;}

