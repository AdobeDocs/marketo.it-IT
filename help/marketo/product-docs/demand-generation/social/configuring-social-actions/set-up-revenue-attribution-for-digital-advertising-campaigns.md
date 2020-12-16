---
unique-page-id: 10098812
description: Imposta l'attribuzione delle entrate per le campagne pubblicitarie digitali - Marketo Docs - Documentazione del prodotto
title: Impostazione dell'attribuzione delle entrate per le campagne pubblicitarie digitali
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---


# Impostazione dell&#39;attribuzione delle entrate per le campagne pubblicitarie digitali {#set-up-revenue-attribution-for-digital-advertising-campaigns}

Ecco come impostare l&#39;attribuzione dei ricavi per canali e campagne pubblicitarie digitali. Una volta configurato, puoi eseguire l&#39;attribuzione dei ricavi &quot;first-touch&quot; e &quot;multi-touch&quot; per gli annunci digitali come in altri programmi Marketo.

Dopo aver configurato il primo programma di annunci in Marketo, puoi duplicarlo e aggiornarlo per altri canali. Ad esempio, duplica un programma LinkedIn in un programma Facebook.

Con programmi separati, puoi quindi tenere traccia del numero di conversioni da ciascuna di esse e visualizzare i tuoi programmi in Program Analyzer, Opportunity Influence Analyzer e altre funzionalità di Marketing Analytics.

>[!PREREQUISITES]
>
>* Impostare un tag canale con valori di stato e successo del programma (ad esempio, Digital Advertising o Social Paid e PPC)
>* Creare o modificare un modulo per passare una stringa di query con la persona
>* Assicurati di avere accesso ad alcune funzionalità di analisi del ciclo dei ricavi per segnalare i canali e le campagne di annunci

>



## Creare un programma predefinito {#create-a-default-program}

A differenza di alcuni programmi (come l&#39;e-mail) che possono essere eseguiti periodicamente per un periodo di tempo specifico, i programmi predefiniti sono sempre attivati.

1. Vai a Attività **** di marketing.

   ![](assets/login-marketing-activities-5.png)

1. Fate clic su **Nuovo** e selezionate **Nuovo programma**.

   ![](assets/image2016-3-14-15-52-0.png)

1. Se avete già un programma in funzione, potete [clonarlo](../../../../product-docs/core-marketo-concepts/programs/working-with-programs/clone-a-program.md).

   >[!TIP]
   >
   >Ogni volta che si duplica un programma, assicurarsi di sostituire i nomi nei campi delle stringhe di query degli elenchi smart.

1. Posizionare il nuovo programma in una cartella specifica della campagna, dopo aver impostato il programma iniziale.

   >[!NOTE]
   >
   >**Esempio**
   >
   >
   >Una stringa di query passata attraverso l’URL aiuta Marketo a sapere su quale campagna pubblicitaria qualcuno ha fatto clic quando è diventato una persona in Marketo.
   >
   >
   >È possibile creare una metodologia di stringa di query che includa tutte le variabili da misurare. Marketo utilizza queste variabili per aggiungere persone ai diversi programmi.
   >
   >
   >Ad esempio, potete utilizzare il tipo di canale Canale__Canale__Area. Può essere simile a: SP_FB_NewGuide_US. **Nota**: le abbreviazioni consentono di risparmiare spazio.
   >
   >
   >In alternativa, impostatela come Channel_Adsource_AssetName_Region_UniqueIdNumber. Può essere simile a: Social-Paid_Facebook_NewGuide_NA_123.

## Creare una campagna intelligente per i nuovi nomi {#create-a-smart-campaign-for-new-names}

1. Nella campagna smart, create un elenco smart che contenga due attivatori e due filtri, come mostrato.

   ![](assets/image2016-3-23-13-3a59-3a24.png)

   >[!NOTE]
   >
   >La stringa di query utilizzata nelle due attivazioni e nel filtro Nome **** programma acquisito è univoca. Le stringhe di query visualizzate qui sono solo ad esempio. Se hai clonato il campo, sostituisci semplicemente questi campi.

1. Crea un passaggio di flusso per modificare l&#39;attributo in **Acquisition Program** e impostare New Value (Nuovo valore) sul valore definito per le campagne social a pagamento.

   ![](assets/image2016-3-14-14-3a58-3a6.png)

1. Pianificare e attivare la campagna.

## Creazione di una campagna intelligente per il successo dello stato/del programma {#create-a-smart-campaign-for-status-program-success}

È necessaria una seconda campagna intelligente per modificare lo stato delle persone, in modo che possano raggiungere il successo del programma e essere incluse nei calcoli di attribuzione delle entrate.

1. Nell&#39;attivatore **Modulo** di compilazione, immettere il nome del programma nella stringa di query. Se state clonando il programma, sostituite il nome della vecchia stringa di query con il nuovo.

   ![](assets/image2016-3-23-14-3a7-3a20.png)

1. Crea passaggi di flusso per cambiare lo stato in uno associato al successo del programma.

   ![](assets/image2016-3-14-15-3a9-3a29.png)

   >[!NOTE]
   >
   >Nell&#39;esempio riportato sopra, **Convertito, **ma questo dipende dai valori di stato/successo.

1. Pianificare e attivare la campagna.

## Crea annuncio {#create-your-ad}

Dopo aver configurato il programma e le campagne, crea il nuovo annuncio.

1. Vai al canale; Ad esempio, LinkedIn o Facebook.
1. Crea un nuovo annuncio.
1. Selezionate una pagina di destinazione Marketo come destinazione per l’azione Invito all’interno della campagna.
1. Aggiungete la stringa di query all’URL.

   >[!NOTE]
   >
   >**Esempio**
   >
   >
   >Ecco come aggiungere tutte le informazioni configurate in un URL effettivo. Gli elementi sono separati da una e commerciale (&amp;):
   >
   >
   >[www.marketo.com?**source**=Social-Paid&amp;**comment**=Social-Paid_Facebook_NewGuide_NA&amp;**camp**=abc&amp;**kk=**xyz](http://www.marketo.com?source=Social-Paid&amp;comment=Social-Paid_Facebook_NewGUide_NA&amp;camp=abc&amp;kk+xyz)
   >
   >    
   >    
   >    * **source** è l’Origine Persona utilizzata come identificatore del canale
   >    * **comment** è l&#39;identificatore univoco creato per ciascun programma
   >    * **camp** è la campagna su Facebook, LinkedIn o Google
   >    * **kk** è la parola chiave o il nome della risorsa da acquisire

   >    
   >    
   >**Questi quattro termini devono essere tutti in lettere minuscole e l’URL non può contenere spazi per acquisire tali informazioni.**

## Best practice {#best-practices}

Utilizzate un singolo tag canale per rappresentare tutta la pubblicità digitale, oppure più tag canale se desiderate confronti più granulari rispetto agli altri canali di marketing (ad esempio, Social-Paid, Search-Paid, Display, Retargeting).

Quindi, configurate programmi diversi per ogni visualizzazione di reporting necessaria. Usate un ID comune come parametro nell’URL (ad esempio BC) nella stringa di query se avete 10 aree che avviano una &quot;Grande campagna&quot; insieme e desiderate poter visualizzare i risultati tra le diverse aree.

Se vuoi creare un rapporto su ogni regione e sui risultati collettivi della Campagna Grande, crea 11 programmi: uno per ogni regione e uno per la Campagna Grande. Ogni programma fa riferimento solo ai caratteri pertinenti della stringa di query (ad esempio BC).

Esiste una sovrapposizione intenzionale nel numero di persone tra i programmi della Grande Campagna e quelli della regione, per cui non si desidera segnalare il totale delle persone in tutti gli 11 programmi, in quanto alcune persone si trovano sia nella Grande Campagna che in uno dei programmi della regione.
