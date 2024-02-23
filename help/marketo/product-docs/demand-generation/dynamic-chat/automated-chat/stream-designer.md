---
description: Progettazione flussi - Documentazione di Marketo - Documentazione del prodotto
title: Designer flusso
feature: Dynamic Chat
exl-id: 310b1dff-dd93-48a6-85c2-64c58494ce48
source-git-commit: f5f93a993d5b13c1fda0b31172393eff0bc65fd4
workflow-type: tm+mt
source-wordcount: '1108'
ht-degree: 1%

---

# Designer flusso {#stream-designer}

Ci sono _molti_ combinazioni di flusso possibili. Questo articolo contiene un esempio in cui l’addetto al marketing chiede al visitatore del sito se ha domande sul prodotto. In caso affermativo, il visitatore può pianificare un appuntamento. In caso negativo, il visitatore ha la possibilità di iscriversi a una mailing list per la corrispondenza futura. Viene anche offerto loro un PDF gratuito. L’obiettivo finale è pianificare un appuntamento o raccogliere l’e-mail del visitatore.

>[!PREREQUISITES]
>
>Prima di poter utilizzare la scheda Documento, è necessario [configurarlo](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-pdf-embed-api.md){target="_blank"} nel tuo account di Adobe.

## Schede di Stream Designer {#stream-designer-cards}

Progettazione flussi contiene più schede che è possibile aggiungere per modellare la conversazione chat.

<table>
 <tr>
  <td style="width:25%"><strong>Messaggio</strong></td>
  <td>Da utilizzare quando si desidera effettuare una dichiarazione senza bisogno di risposta (ad esempio: "Ciao! Tutti gli articoli hanno il 25% di sconto oggi con il codice SAVE25").
</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Domanda</strong></td>
  <td>Da utilizzare quando si desidera porre una domanda a scelta multipla, di cui si forniscono le risposte disponibili (ad esempio: Quale tipo di veicolo si è interessati? Risposte = SUV, Compatto, Camion, ecc.).</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Documento</strong></td>
  <td>Consente di incorporare documenti PDF nelle finestre di dialogo e di tenere traccia dell’attività di coinvolgimento dei visitatori nei documenti (quante pagine sono state visualizzate, se il documento è stato scaricato e/o qualsiasi termine di ricerca utilizzato).</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Acquisizione delle informazioni</strong></td>
  <td>Utilizzare quando si desidera raccogliere informazioni (ad esempio, nome, indirizzo e-mail, qualifica, ecc.). Dopo aver scelto il campo a cui attribuire la risposta, puoi scegliere se consentire al visitatore di digitare il testo nella risposta o selezionare le opzioni da un elenco a discesa che hai determinato (suggerimento: quest’ultimo può essere utile per la pulizia del database). Puoi anche scegliere di sovrascrivere i dati attualmente elencati con la relativa risposta, oppure puoi saltare completamente la domanda se disponi già di un valore per essi.</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Prenotazione riunione</strong></td>
  <td>Fornisce al visitatore un calendario delle date disponibili per pianificare una riunione. Scegli la disponibilità del calendario tramite round robin, un agente specifico o utilizzando regole personalizzate. Clic <b>Aggiungi attributo</b> se desideri acquisire il nome o l’indirizzo e-mail dell’agente e assegnarlo al record persona del visitatore della chat per eseguire query future (suggerimento: creare un <a href="/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md" target="_blank">campo personalizzato</a> per mappare le informazioni dell’agente su in modo da non sovrascrivere un campo di Marketo Engage standard).</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Obiettivo</strong></td>
  <td>Questa è l'unica carta che i visitatori non vedranno. Sta a te determinare a quale punto un obiettivo viene raggiunto all’interno della chat specifica (ad esempio, se l’obiettivo è la raccolta dell’e-mail del visitatore, inserisci la scheda Obiettivo immediatamente dopo Info Capture nel flusso).</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Azione</strong></td>
  <td>Simile ai campi nascosti di un modulo, con la scheda delle azioni è possibile compilare qualsiasi attributo del lead o dell’azienda (che presenta un <a href="/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md#string">tipo di dati string</a>) con valori impliciti che si desidera acquisire in base a un record lead. Puoi aggiungere la scheda delle azioni in qualsiasi punto della conversazione e aggiornare i rispettivi attributi con un valore o token nativi che popolano automaticamente il rispettivo valore.</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Chat live</strong></td>
  <td>Utilizza la scheda chat in diretta quando desideri che i visitatori chattino con un agente in diretta.
  <li>La scheda chat live deve essere l'ultima scheda del ramo.</li>
  <li>I visitatori verranno indirizzati a un agente non appena raggiungono questa scheda nel flusso, pertanto si consiglia di anteporre a questa scheda una scheda con le domande che chiedono ai visitatori se desiderano chattare con un agente live.</li></td>
 </tr>
</table>

## Icone di Stream Designer {#stream-designer-icons}

In alto a destra in Progettazione flussi sono visualizzate alcune icone. Ecco cosa fanno.

<table>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-1.png"></td>
  <td>Ingrandisce, creando schede più grandi</td>
 </tr>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-2.png"></td>
  <td>Esegue lo zoom indietro, creando schede più piccole</td>
 </tr>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-3.png"></td>
  <td>Apre una finestra per il test della chat (premere lo stesso pulsante per chiudere)</td>
 </tr>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-4.png"></td>
  <td>Consente di cercare tipi di schede o contenuti all’interno del flusso</td>
 </tr>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-5.png"></td>
  <td>Dispone tutte le schede nel flusso</td>
 </tr>
</table>

## Creare un flusso {#create-a-stream}

È possibile creare flussi per le finestre di dialogo o [Forms per conversazioni](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-overview.md){target="_blank"}. In questo esempio ne creeremo uno per un dialogo.

1. Dopo aver [ha creato il tuo dialogo](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-dialogue.md){target="_blank"}, fare clic su **[!UICONTROL Progettazione flussi]** scheda.

   ![](assets/stream-designer-6.png)

1. Trascina la [!UICONTROL Domanda] Card.

   ![](assets/stream-designer-7.png)

1. Sotto [!UICONTROL Risposta Chatbot], digita la tua domanda come desideri.

   ![](assets/stream-designer-8.png)

   >[!TIP]
   >
   >Puoi personalizzare l’esperienza per i visitatori della chat conosciuti utilizzando dei token (es: Hello `{{lead.leadFirstName:""}}`). Fai clic sull’icona della parentesi graffa a destra ed effettua la selezione. Aggiungi un valore predefinito tra i quoate se vuoi che i visitatori anonimi vedano qualcosa di generico (es: Hello `{{lead.leadFirstName:"there"}}`).

   >[!NOTE]
   >
   >Poke è impostato su on per impostazione predefinita, il che mostra la domanda di apertura accanto all’icona della chat senza che il visitatore debba fare clic su di essa per visualizzarla. Poke è disponibile solo sulla prima scheda della conversazione.

1. Inserisci le risposte utente e fai clic su **[!UICONTROL Salva]**.

   ![](assets/stream-designer-9.png)

   >[!NOTE]
   >
   >**[!UICONTROL Modifica valori memorizzati]** è un passaggio facoltativo per coloro che desiderano memorizzare nel database un valore diverso da quello visualizzato ai visitatori nel chatbot per gli attributi mappati nella scheda Domanda (ad esempio, il visitatore vede &quot;Ottimizzazione del motore di ricerca&quot; e il valore viene memorizzato come &quot;SEO&quot;).

1. Se si seleziona &quot;Sì&quot; si desidera pianificare un appuntamento, quindi trascinare l&#39;opzione nella scheda Programmazione appuntamenti.

   ![](assets/stream-designer-10.png)

1. Nella colonna a destra, fai clic su **[!UICONTROL Salva]**.

   ![](assets/stream-designer-11.png)

1. Poiché si tratta di un obiettivo, trascina [!UICONTROL Obiettivo] sotto l&#39;Utilità di pianificazione appuntamenti.

   ![](assets/stream-designer-12.png)

1. Assegna un nome all’obiettivo (o scegliine uno esistente) e fai clic su **[!UICONTROL Salva]**.

   ![](assets/stream-designer-13.png)

1. Per &quot;No&quot; vogliamo vedere se si uniranno alla mailing list, quindi sotto quell&#39;opzione trascinare su un altro [!UICONTROL Domanda] Card.

   ![](assets/stream-designer-14.png)

1. Inserisci la risposta e aggiungi le scelte di risposta per il visitatore. Clic **[!UICONTROL Salva]** al termine.

   ![](assets/stream-designer-15.png)

   >[!NOTE]
   >
   >Puoi aggiungere altre risposte facendo clic su **[!UICONTROL Aggiungi risposta]**.

1. Sotto la risposta &quot;Sì&quot;, trascina sulla scheda Info Capture per raccogliere l’e-mail del visitatore.

   ![](assets/stream-designer-16.png)

1. Fai clic su **[!UICONTROL Tipo]** a discesa e selezionare **[!UICONTROL E-mail]**.

   ![](assets/stream-designer-17.png)

1. Inserisci un messaggio chatbot e un segnaposto. Assicurati che l’attributo sia mappato al campo appropriato in Marketo e fai clic su **[!UICONTROL Salva]**.

   ![](assets/stream-designer-18.png)

   <table>
    <tr>
     <td style="width:30%"><strong>Tipo</strong></td>
     <td>Tipo di informazioni da acquisire: telefono, testo, e-mail.</td>
    </tr>
    <tr>
     <td style="width:30%"><strong>Messaggio del chatbot</strong></td>
     <td>Il messaggio visualizzato dal visitatore che gli chiede di fornire le informazioni.</td>
    </tr>
    <tr>
     <td style="width:30%"><strong>Placeholder</strong></td>
     <td>Testo di esempio che aiuta il visitatore a vedere cosa inserire.</td>
    </tr>
    <tr>
     <td style="width:30%"><strong>Mappa risposta su attributo</strong></td>
     <td>Consente di sincronizzare la risposta del visitatore al campo corrispondente nel record Persona nell’abbonamento Marketo.</td>
    </tr>
   </table>

1. Poiché la raccolta delle e-mail è un obiettivo, trascina [!UICONTROL Obiettivo] sotto Info Capture.

   ![](assets/stream-designer-19.png)

1. Assegna un nome all’obiettivo (o scegliine uno esistente) e fai clic su **[!UICONTROL Salva]**.

   ![](assets/stream-designer-20.png)

1. Ricordati di aggiungere una risposta se dicono &quot;No&quot;. Un&#39;opzione consiste nel trascinare una scheda Messaggio qui sotto e dire &quot;grazie comunque&quot;. In questo esempio, forniremo loro invece un documento di PDF gratuito.

   ![](assets/stream-designer-21.png)

1. In questo esempio verrà creato un nuovo documento. Assegna un nome, immetti l’URL del PDF che hai già ospitato e fai clic su **[!UICONTROL Salva]**.

   ![](assets/stream-designer-22.png)

1. Seleziona la **[!UICONTROL Anteprima]** attiva per visualizzare l’anteprima della finestra di dialogo.

   ![](assets/stream-designer-23.png)

1. Quando sei pronto ad attivare la tua finestra di dialogo, fai clic su **[!UICONTROL Pubblica]**.

   ![](assets/stream-designer-24.png)

>[!NOTE]
>
>Prima di fare clic [!UICONTROL Pubblica], ricorda di assicurarti di aver [ha inserito gli URL di destinazione](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/audience-criteria.md#target){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Creare una finestra di dialogo](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-dialogue.md){target="_blank"}
>* [Criteri di pubblico](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/audience-criteria.md){target="_blank"}
>* [API di incorporamento Adobe PDF](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-pdf-embed-api.md){target="_blank"}
