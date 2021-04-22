---
unique-page-id: 2949839
description: Controllare le persone nell'evento dal Tablet PC - Marketo Docs - Documentazione del prodotto
title: Controllare le persone nell'evento dal Tablet PC
exl-id: b48f5f95-8e36-441f-a785-1651f42f9f60
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# Controllare le persone nell&#39;evento dal Tablet {#check-people-into-your-event-from-your-tablet}

Quando le persone si presentano al tuo evento, puoi trovare le loro informazioni sull’app. Dopo il check-in, vengono promossi allo stato Partecipante al momento della sincronizzazione con Marketo.

L’app funziona allo stesso modo sia su iPad che su Android, tranne che per differenze di layout e progettazione minori.

>[!PREREQUISITES]
>
>* Crea un evento in Marketo e popolalo con persone invitate e registrate.
>* Scarica l&#39;app per tablet per [Android](https://play.google.com/store/apps/details?id=com.marketo.eventcheckin&amp;hl=en) o [iOS](https://itunes.apple.com/us/app/marketo-events/id522766637?mt=8)


## Accedi agli ospiti registrati {#check-in-registered-guests}

1. Tocca l’icona dell’app sull’iPad o sul tablet Android.

1. Tocca **Login** per avviare l&#39;app Marketo Event.

   ![](assets/1.jpg)

1. Immetti il nome utente e la password Marketo e fai clic su **Login**.

   >[!NOTE]
   >
   >Per visualizzare le persone nell’app, devi disporre di un ruolo con accesso al database.

1. Selezionare un **Evento**.

   ![](assets/2.jpg)

   >[!TIP]
   >
   >Vengono visualizzati solo i programmi evento (ad eccezione dei webinar) pianificati una settimana prima e una settimana dopo la data odierna.

1. Nella schermata Home, cerca gli ospiti registrati. Per trovare una persona nell’elenco, puoi:

   * Scorri per trovare un nome
   * Immettere un nome nel campo di ricerca
   * Passa a una lettera iniziale specifica del cognome toccandola sul lato destro dell’elenco

   >[!NOTE]
   >
   >Il processo è lo stesso su iPad e Android, ma gli schermi sono diversi e gli elementi possono trovarsi in posizioni diverse. Questo articolo presenta l’interfaccia iPad. Confronta la schermata Android in questa sezione per riferimento.

   **iPad**

   ![](assets/image2016-4-15-11-3a55-3a11.png)

   **Android**

   ![](assets/image2016-4-15-14-3a50-3a19.png)

1. Toccare il nome selezionato e sul record della persona, toccare **Check-in**.

   ![](assets/img-0068-35-hands.png)

L&#39;ospite ora ha uno stato Partecipante e riceve un segno di spunta. Il record della persona viene aggiornato al momento della sincronizzazione con Marketo. Il contatore rosso sul pulsante Sincronizza viene incrementato per mostrare il numero di check-in dall&#39;ultima sincronizzazione con Marketo. Il pulsante Sincronizza ha un aspetto diverso ed è in una posizione diversa per iPad e Android:

**iPad**

![](assets/image2016-4-12-14-3a25-3a13.png)

**Android**

![](assets/image2016-4-15-14-3a58-3a6.png)

>[!TIP]
>
>Se una persona è invitata ma non è registrata, è possibile cercare il nome facendo clic su **Cerca sul server**, appena sotto la casella Ricerca. Lo stato Invitato cambia in **Partecipato** per l&#39;evento.

## Crea una nuova persona sul Tablet {#create-a-new-person-on-the-tablet}

Puoi aggiungere manualmente gli ospiti che non sono persone esistenti nel database Marketo. Verranno automaticamente archiviate e aggiunte al database al momento della sincronizzazione con Marketo.

1. Fare clic su **Aggiungi**.

   **iPad**

   ![](assets/image2016-4-15-11-3a58-3a51.png)

   **Android**

   ![](assets/image2016-4-15-15-3a2-3a38.png)

1. Compila tutti i campi di informazioni di base possibili e tocca **Fine**.

   ![](assets/image2016-4-15-11-3a33-3a59.png)

   >[!NOTE]
   >
   >È possibile utilizzare solo i campi esistenti. Non puoi crearne di personalizzati.

   >[!CAUTION]
   >
   >Controlla l&#39;indirizzo e-mail. È possibile correggere altri campi in un secondo momento, ma l’indirizzo e-mail è il metodo principale per contattare l’ospite.

La nuova persona viene registrata come ha effettuato l&#39;accesso all&#39;evento e verrà aggiunta al database Marketo con stato Attended quando si esegue la sincronizzazione con Marketo.

## Invertire un Check-In {#reverse-a-check-in}

Se hai selezionato una persona per errore _prima di eseguire la sincronizzazione con Marketo_, puoi invertire lo stato Partecipante.

1. Toccare il nome nell’elenco e nel record della persona toccare **Annulla**.

   ![](assets/image2016-4-15-11-3a38-3a31.png)

   Tutto fisso!

## Modificare un record di persona al momento del check-in {#edit-a-person-record-at-check-in}

Puoi aggiungere e modificare le informazioni sugli ospiti, direttamente all&#39;evento!

1. Toccare il nome nell&#39;elenco delle persone e toccare **Modifica**.

   ![](assets/image2016-4-15-11-3a43-3a46.png)

1. Modifica e aggiungi informazioni ai campi, quindi tocca **Fine**.

   ![](assets/image2016-4-15-11-3a50-3a18.png)

   >[!NOTE]
   >
   >In Android, il pulsante **Fine** può essere nascosto. Scorri verso il basso per trovarlo.

Le informazioni vengono aggiornate al momento della sincronizzazione dell’app con Marketo.

## Sincronizza l&#39;app con Marketo {#sync-the-app-with-marketo}

L’app Marketo Events funziona in modo indipendente finché non sincronizzi nuovamente l’attività al database Marketo. È consigliabile eseguire la sincronizzazione il prima possibile dopo l’ultimo check-in. Il tablet deve essere connesso a Internet.

>[!CAUTION]
>
>Dopo la sincronizzazione, non puoi annullare un check-in dall&#39;app.

1. Sul tablet, apri l’app e accedi all’evento.

1. Tocca **Sincronizza**.

   L&#39;evento viene aggiornato con nuovi check-in nel database Marketo. Il contatore rosso sul pulsante Sincronizza si cancella finché non si verifica l&#39;inserimento di un altro utente.

   Per motivi di sicurezza, dopo aver completato la sincronizzazione dovresti chiudere l’app Marketo Events.

## Utilizzo di Accesso Internet limitato {#working-with-limited-internet-access}

Alcuni luoghi hanno un accesso a Internet scarso. È necessaria una buona connessione a:

* Scaricare e installare l’app
* Accedere
* Selezionare un evento
* Sincronizza l’app con Marketo

Se sei preoccupato dell&#39;accesso a Internet nel luogo in cui ti trovi, puoi accedere all&#39;app Marketo Events e selezionare l&#39;evento in anticipo, in una posizione con forte accesso a Internet. In questo modo, puoi comunque utilizzare l’app offline. Quindi, quando si riprende una connessione Internet, sincronizzarsi immediatamente al database Marketo.

>[!TIP]
>
>Se non disponi di una connessione Internet, puoi comunque creare una nuova persona per il check-in. Si riconcilierà con la persona esistente quando sincronizzerai l’app.

>[!NOTE]
>
>L’app ti disconnette automaticamente dopo otto ore di inattività.
