---
unique-page-id: 2949839
description: Visitare la pagina dedicata all'evento dal Tablet PC - Documentazione di Marketo - Documentazione del prodotto
title: Controllare l'evento dal Tablet PC
exl-id: b48f5f95-8e36-441f-a785-1651f42f9f60
feature: Mobile Marketing
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---

# Controllare l&#39;evento dal Tablet PC {#check-people-into-your-event-from-your-tablet}

Quando le persone si presentano al tuo evento, puoi trovare le loro informazioni nell’app. Dopo il check-in, vengono promossi allo stato Partecipazione durante la sincronizzazione con Marketo.

>[!IMPORTANT]
>
>Il 2 ottobre 2023 Adobe ha rimosso l’app Marketo Events da tutti gli app store. Se l&#39;app è già installata sul tuo tablet/dispositivo mobile, puoi continuare a utilizzarla per il momento. Una volta migrata l’istanza Marketo Engage ad Adobe Identity per l’autenticazione di Marketo, non potrai più accedere all’app. [Ulteriori informazioni](https://nation.marketo.com/t5/product-discussions/marketo-events-app-and-marketo-moments-app-end-of-life/m-p/340712/highlight/true#M193869){target="_blank"}.

L&#39;app funziona allo stesso modo sia su [!DNL iPad] che su [!DNL Android], ad eccezione di lievi differenze di layout e progettazione.

>[!PREREQUISITES]
>
>* Crea un evento in Marketo e popolalo con persone invitate e registrate.

## Check-in Ospiti registrati {#check-in-registered-guests}

1. Tocca l&#39;icona dell&#39;app sul tablet [!DNL iPad] o [!DNL Android].

1. Tocca **[!UICONTROL Login]** per avviare l&#39;app Marketo Event.

   ![](assets/1.jpg)

1. Immettere il nome utente e la password di Marketo e fare clic su **[!UICONTROL Login]**.

   >[!NOTE]
   >
   >Per visualizzare le persone nell’app, devi disporre di un ruolo con accesso al database.

1. Selezionare un **[!UICONTROL Event]**.

   ![](assets/2.jpg)

   >[!TIP]
   >
   >Vengono visualizzati solo i programmi evento (ad eccezione dei webinar) programmati una settimana prima e una settimana dopo la data odierna.

1. Nella schermata iniziale, sfogliare per trovare gli ospiti registrati. Per trovare una persona nell’elenco, puoi:

   * Scorri per trovare un nome
   * Immetti un nome nel campo di ricerca
   * Passa a una lettera iniziale specifica del cognome toccandola sul lato destro dell’elenco

   >[!NOTE]
   >
   >Il processo è lo stesso in [!DNL iPad] e [!DNL Android], ma le schermate sono diverse e gli elementi potrebbero trovarsi in posizioni diverse. Questo articolo presenta l&#39;interfaccia [!DNL iPad]. Confrontare la schermata [!DNL Android] in questa sezione per riferimento.

   **[!DNL iPad]**

   ![](assets/image2016-4-15-11-3a55-3a11.png)

   **[!DNL Android]**

   ![](assets/image2016-4-15-14-3a50-3a19.png)

1. Toccare il nome selezionato e nel record della persona toccare **[!UICONTROL Check-in]**.

   ![](assets/img-0068-35-hands.png)

L&#39;ospite ora è in stato Partecipato e riceve un segno di spunta. Il record della persona viene aggiornato quando si esegue la sincronizzazione con Marketo. Il contatore rosso sul pulsante Sincronizza viene incrementato per mostrare il numero di check-in dall&#39;ultima sincronizzazione con Marketo. Il pulsante di sincronizzazione ha un aspetto diverso e si trova in una posizione diversa per [!DNL iPad] e [!DNL Android]:

**[!DNL iPad]**

![](assets/image2016-4-12-14-3a25-3a13.png)

**[!DNL Android]**

![](assets/image2016-4-15-14-3a58-3a6.png)

>[!TIP]
>
>Se una persona è stata invitata ma non si è registrata, è possibile cercare il nome facendo clic su **[!UICONTROL Search on Server]**, immediatamente sotto la casella Cerca. Lo stato Invitato cambia in **[!UICONTROL Attended]** per l&#39;evento.

## Creare una nuova persona sul tablet {#create-a-new-person-on-the-tablet}

Puoi aggiungere manualmente gli ospiti che non sono persone esistenti nel database di Marketo. Verranno automaticamente archiviati e aggiunti al database durante la sincronizzazione con Marketo.

1. Fai clic su **[!UICONTROL Add]**.

   **[!DNL iPad]**

   ![](assets/image2016-4-15-11-3a58-3a51.png)

   **[!DNL Android]**

   ![](assets/image2016-4-15-15-3a2-3a38.png)

1. Completa il maggior numero possibile di campi delle informazioni di base e tocca **[!UICONTROL Done]**.

   ![](assets/image2016-4-15-11-3a33-3a59.png)

   >[!NOTE]
   >
   >Puoi utilizzare solo i campi esistenti. Non puoi crearne di personalizzati.

   >[!CAUTION]
   >
   >Controlla nuovamente l’indirizzo e-mail. Altri campi possono essere corretti in un secondo momento, ma l’indirizzo e-mail è il metodo principale per contattare l’ospite.

La nuova persona è registrata come archiviata nell&#39;evento e verrà aggiunta al database di Marketo con stato Partecipazione durante la sincronizzazione con Marketo.

## Inverti check-in {#reverse-a-check-in}

Se una persona è stata archiviata per errore, _prima della sincronizzazione con Marketo_, è possibile invertire lo stato [!UICONTROL Attended].

1. Toccare il nome nell&#39;elenco e nel record persona toccare **[!UICONTROL Undo]**.

   ![](assets/image2016-4-15-11-3a38-3a31.png)

   Tutto risolto!

## Modificare un record persona al momento del check-in {#edit-a-person-record-at-check-in}

Puoi aggiungere e modificare le informazioni dei visitatori direttamente all’evento.

1. Toccare il nome nell&#39;elenco delle persone e toccare **[!UICONTROL Edit]**.

   ![](assets/image2016-4-15-11-3a43-3a46.png)

1. Modifica e aggiungi informazioni ai campi, quindi tocca **[!UICONTROL Done]**.

   ![](assets/image2016-4-15-11-3a50-3a18.png)

   >[!NOTE]
   >
   >In [!DNL Android], il pulsante **[!UICONTROL Done]** potrebbe essere nascosto. Scorri verso il basso per trovarlo.

Le informazioni verranno aggiornate al momento della sincronizzazione dell&#39;app con Marketo.

## Sincronizzare l’app con Marketo {#sync-the-app-with-marketo}

L’app Marketo Events funziona in modo indipendente finché non sincronizzi nuovamente l’attività con il database di Marketo. È consigliabile eseguire la sincronizzazione il prima possibile dopo l&#39;ultimo check-in. Il tablet deve essere connesso a Internet.

>[!CAUTION]
>
>Dopo la sincronizzazione, non è possibile annullare un check-in dall&#39;app.

1. Sul tablet, apri l’app e passa all’evento.

1. Toccare **[!UICONTROL Sync]**.

   L’evento viene aggiornato con le nuove archiviazioni nel database di Marketo. Il contatore rosso sul pulsante Sincronizza si cancella finché non si archivia un altro utente.

   Per motivi di sicurezza, devi uscire dall’app Marketo Events al termine della sincronizzazione.

## Utilizzo dell&#39;accesso limitato a Internet {#working-with-limited-internet-access}

Alcuni luoghi hanno uno scarso accesso a Internet. È necessaria una buona connessione a:

* Scaricare e installare l’app
* Accedi
* Seleziona un evento
* Sincronizzare l’app con Marketo

Se sei preoccupato dell&#39;accesso a Internet, puoi accedere all&#39;app Marketo Events e selezionare l&#39;evento in anticipo, in una posizione con un forte accesso a Internet. In questo modo, puoi comunque utilizzare l’app offline. Quindi, quando si riprende una connessione Internet, eseguire immediatamente la sincronizzazione con il database di Marketo.

>[!TIP]
>
>Se non si dispone di una connessione a Internet, è comunque possibile creare una nuova persona per l&#39;archiviazione. Si riconcilierà con la persona esistente quando sincronizzerai l&#39;app.

>[!NOTE]
>
>L’app ti disconnette automaticamente dopo otto ore di inattività.
