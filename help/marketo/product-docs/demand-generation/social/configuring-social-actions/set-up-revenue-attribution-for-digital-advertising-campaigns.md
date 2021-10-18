---
unique-page-id: 10098812
description: Impostare l’attribuzione dei ricavi per le campagne pubblicitarie digitali - Marketo Docs - Documentazione del prodotto
title: Imposta l’attribuzione dei ricavi per le campagne pubblicitarie digitali
exl-id: 7fb16c5f-7e76-429b-8b01-b5a1dd898158
source-git-commit: 41d8762203786bac9aea03ac978daa0549ac8e93
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 0%

---

# Imposta l’attribuzione dei ricavi per le campagne pubblicitarie digitali {#set-up-revenue-attribution-for-digital-advertising-campaigns}

Ecco come impostare l’attribuzione dei ricavi per canali e campagne pubblicitarie digitali. Dopo aver impostato questa opzione, puoi eseguire l’attribuzione dei ricavi di primo e multi-tocco per gli annunci digitali come in altri programmi Marketo.

Dopo aver configurato il tuo primo programma di annunci in Marketo, puoi clonarlo e aggiornarlo per altri canali. Ad esempio, clonare un programma LinkedIn su un programma Facebook.

Con programmi separati, puoi quindi tenere traccia del numero di conversioni da ciascuna di esse e visualizzare i programmi in Program Analyzer, Opportunity Influence Analyzer e altre funzionalità di Marketo Analytics.

>[!PREREQUISITES]
>
>* Imposta un tag canale con i valori di stato e il successo del programma (ad esempio, pubblicità digitale o Social Paid e PPC)
>* Creare o modificare un modulo per passare una stringa di interrogazione con la persona
>* Assicurati di avere accesso ad alcune funzionalità di Revenue Cycle Analytics per generare rapporti sui canali e le campagne pubblicitarie


## Creare un programma predefinito {#create-a-default-program}

A differenza di alcuni programmi (ad esempio e-mail) che possono essere eseguiti periodicamente per un periodo di tempo specifico, i programmi predefiniti sono sempre attivi.

1. Vai a **Attività di marketing**.

   ![](assets/login-marketing-activities-5.png)

1. Fai clic su **Nuovo** e seleziona **Nuovo programma**.

   ![](assets/image2016-3-14-15-52-0.png)

1. Se disponi già di un programma, puoi [clonare](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/clone-a-program.md).

   >[!TIP]
   >
   >Ogni volta che cloni un programma, assicurati di sostituire i nomi nei campi stringa query degli elenchi avanzati.

1. Posiziona il nuovo programma in una cartella specifica della campagna, dopo aver impostato il programma iniziale.

   >[!NOTE]
   >
   >**Esempio**
   >
   >Una stringa di query passata attraverso l’URL consente a Marketo di sapere su quale campagna pubblicitaria qualcuno ha fatto clic quando è diventato una persona in Marketo.
   >
   >È possibile creare una metodologia della stringa di query che includa tutte le variabili che si desidera misurare. Marketo utilizza queste variabili per aggiungere persone ai diversi programmi.
   >
   >Ad esempio, puoi utilizzare il tipo di canale Canale__Canale__Risorsa__Regione. Potrebbe essere simile a: SP_FB_NewGuide_US. **Nota**: le abbreviazioni consentono di risparmiare spazio.
   >
   >Oppure, impostalo come Channel_Adsource_AssetName_Region_UniqueIdNumber. Potrebbe essere simile a: Social-Paid_Facebook_NewGuide_NA_123.

## Creare una campagna avanzata per i nuovi nomi {#create-a-smart-campaign-for-new-names}

1. Nella campagna avanzata, crea un elenco avanzato contenente due attivatori e due filtri, come mostrato.

   ![](assets/image2016-3-23-13-3a59-3a24.png)

   >[!NOTE]
   >
   >La stringa di query utilizzata nei due trigger e nella **Programma che ha acquisito il nome** filtro è univoco. Le stringhe di query visualizzate qui sono solo ad esempio. Se hai clonato il campo, sostituisci semplicemente questi campi.

1. Crea un passaggio di flusso per modificare l&#39;attributo in **Programma di acquisizione** e imposta il nuovo valore sul valore definito per le campagne social a pagamento.

   ![](assets/image2016-3-14-14-3a58-3a6.png)

1. Pianifica e attiva la campagna.

## Creare una campagna avanzata per il successo di stato/programma {#create-a-smart-campaign-for-status-program-success}

È necessaria una seconda campagna intelligente per modificare lo stato delle persone, in modo che possano raggiungere il successo del programma e essere incluse nei calcoli di attribuzione dei ricavi.

1. In **Riempie il modulo** attivare, immettere il nome del programma nella stringa query. Se stai clonando il programma, sostituisci il nome della vecchia stringa di query con quello nuovo.

   ![](assets/image2016-3-23-14-3a7-3a20.png)

1. Crea passaggi di flusso per modificare lo stato in uno associato al successo del programma.

   ![](assets/image2016-3-14-15-3a9-3a29.png)

   >[!NOTE]
   >
   >L’esempio precedente mostra **Convertito**, ma dipende dai valori di stato/successo.

1. Pianifica e attiva la campagna.

## Crea l&#39;annuncio {#create-your-ad}

Dopo aver configurato il programma e le campagne, crea il nuovo annuncio.

1. Vai al canale; Ad esempio, LinkedIn o Facebook.
1. Crea un nuovo annuncio.
1. Seleziona una pagina di destinazione Marketo come destinazione per l’invito all’azione nella campagna.
1. Aggiungi la stringa di query all’URL.

   >[!NOTE]
   >
   >**Esempio**
   >
   >Ecco come aggiungere tutte le informazioni impostate in un URL effettivo. Gli elementi sono separati da una e commerciale (&amp;):
   >
   >`www.marketo.com?**source**=Social-Paid&**comment**=Social-Paid_Facebook_NewGuide_NA&**camp**=abc&**kk=**xyz`
   >
   >* **source** è l&#39;origine persona utilizzata come identificatore del canale
   >* **commento** è l&#39;identificatore univoco creato per ciascun programma
   >* **accampamento** è la campagna in Facebook, LinkedIn o Google
   >* **kk** è la parola chiave o il nome della risorsa che desideri acquisire

   >
   >**Questi quattro termini devono essere tutti in minuscolo e non ci possono essere spazi nell&#39;URL per acquisire queste informazioni.**

## Best practice {#best-practices}

Utilizza un singolo tag di canale per rappresentare tutta la pubblicità digitale, oppure utilizza più tag di canale se desideri confronti più granulari rispetto agli altri canali di marketing (ad esempio, Social-Paid, Search-Paid, Display, Retargeting).

Quindi, imposta programmi diversi per ogni visualizzazione di reporting necessaria. Utilizza un ID comune come parametro nell’URL (ad esempio BC) nella stringa query se disponi di 10 aree che lanciano una &quot;Campagna grande&quot; insieme e vuoi essere in grado di visualizzare i risultati tra aree geografiche.

Se desideri creare rapporti su ogni regione e sui risultati collettivi della Campagna Grande, crea 11 programmi, uno per ogni regione e uno per la Campagna Grande. Ogni programma fa riferimento solo ai caratteri pertinenti della stringa di interrogazione (come BC).

Vi è una sovrapposizione intenzionale nel conteggio delle persone tra i programmi Big Campaign e i programmi regionali, quindi non vorrai creare rapporti sul numero totale di persone in tutti gli 11 programmi, in quanto alcune persone sono sia nella Big Campaign che in uno dei programmi regionali.
