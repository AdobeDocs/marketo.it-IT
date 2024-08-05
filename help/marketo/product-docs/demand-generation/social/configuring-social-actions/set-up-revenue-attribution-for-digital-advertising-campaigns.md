---
unique-page-id: 10098812
description: Configurare l’attribuzione dei ricavi per le campagne Digital Advertising - Documenti Marketo - Documentazione del prodotto
title: Impostare l’attribuzione dei ricavi per le campagne Digital Advertising
exl-id: 7fb16c5f-7e76-429b-8b01-b5a1dd898158
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '853'
ht-degree: 0%

---

# Impostare l’attribuzione dei ricavi per le campagne Digital Advertising {#set-up-revenue-attribution-for-digital-advertising-campaigns}

Ecco come impostare l’attribuzione dei ricavi per i canali e le campagne pubblicitarie digitali. Dopo averlo configurato, puoi eseguire l’attribuzione dei ricavi di primo contatto e multi-contatto per gli annunci digitali esattamente come in altri programmi Marketo.

>[!IMPORTANT]
>
>Il 31 luglio 2024 è iniziato il processo di rimozione di questa funzione. Non è più possibile creare nuove risorse. Le risorse esistenti continueranno a funzionare fino al 31 gennaio 2025. [Ulteriori informazioni](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

Dopo aver configurato il primo programma pubblicitario in Marketo, puoi clonarlo e aggiornarlo per altri canali. Ad esempio, clonare un programma LinkedIn in un programma Facebook.

Con i programmi separati, puoi quindi tenere traccia del numero di conversioni da ciascuno e visualizzare i programmi in Analizzatore di programmi, Analizzatore di influenza opportunità e altre funzioni di Marketo Analytics.

>[!PREREQUISITES]
>
>* Impostare un tag di canale con i valori di stato e il successo del programma (ad esempio, Digital Advertising o Social Paid e PPC)
>* Creare o modificare un modulo per trasmettere una stringa di query all’utente
>* Assicurati di avere accesso ad alcune funzionalità di analisi del ciclo di fatturato per creare rapporti sui canali e sulle campagne pubblicitarie

## Creare un programma predefinito {#create-a-default-program}

A differenza di alcuni programmi (come le e-mail) che possono essere eseguiti periodicamente per un periodo di tempo specifico, i programmi predefiniti sono sempre attivi.

1. Vai a **Attività di marketing**.

   ![](assets/login-marketing-activities-5.png)

1. Fai clic su **Nuovo** e seleziona **Nuovo programma**.

   ![](assets/image2016-3-14-15-52-0.png)

1. Se disponi già di un programma, puoi [clonarlo](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/clone-a-program.md).

   >[!TIP]
   >
   >Ogni volta che si clona un programma, assicurarsi di sostituire i nomi nei campi stringa query degli elenchi smart.

1. Posiziona il nuovo programma in una cartella di campagna specifica, dopo aver impostato il programma iniziale.

   >[!NOTE]
   >
   >**Esempio**
   >
   >Una stringa di query trasmessa tramite l’URL consente a Marketo di sapere su quale campagna pubblicitaria ha fatto clic un utente quando è diventato una persona in Marketo.
   >
   >Puoi creare una metodologia di stringa di query che includa tutte le variabili che desideri misurare. Marketo utilizza queste variabili per aggiungere persone ai diversi programmi.
   >
   >Ad esempio, puoi utilizzare Channel type_Channel__Asset__Region. Potrebbe essere simile al seguente: SP_FB_NewGuide_US. **Nota**: le abbreviazioni consentono di risparmiare spazio.
   >
   >In alternativa, impostalo come Channel_Adsource_AssetName_Region_UniqueIdNumber. Potrebbe essere simile al seguente: Social-Paid_Facebook_NewGuide_NA_123.

## Creare una campagna avanzata con nuovi nomi {#create-a-smart-campaign-for-new-names}

1. Nella campagna avanzata, crea un elenco avanzato contenente due trigger e due filtri, come mostrato.

   ![](assets/image2016-3-23-13-3a59-3a24.png)

   >[!NOTE]
   >
   >La stringa di query utilizzata nei due trigger e nel filtro **Programma che ha acquisito il nome** è univoca. Le stringhe di query mostrate di seguito sono solo a titolo di esempio. Se hai clonato il campo, sostituisci semplicemente questi campi.

1. Creare un passaggio di flusso per modificare l&#39;attributo in **Programma di acquisizione** e impostare il nuovo valore sul valore definito per le campagne social a pagamento.

   ![](assets/image2016-3-14-14-3a58-3a6.png)

1. Pianifica e attiva la campagna.

## Creare una campagna avanzata per stato/successo del programma {#create-a-smart-campaign-for-status-program-success}

È necessaria una seconda campagna intelligente per modificare lo stato delle persone, in modo che possano raggiungere il successo del programma ed essere incluse nei calcoli di attribuzione dei ricavi.

1. Nel trigger **Compila modulo**, immettere il nome del programma nella stringa di query. Se si sta clonando il programma, è sufficiente sostituire il nome della stringa di query precedente con quello nuovo.

   ![](assets/image2016-3-23-14-3a7-3a20.png)

1. Crea i passaggi del flusso per cambiare lo stato in uno associato al successo del programma.

   ![](assets/image2016-3-14-15-3a9-3a29.png)

   >[!NOTE]
   >
   >L&#39;esempio precedente mostra **Convertito**, ma questo dipende dai valori di stato/successo.

1. Pianifica e attiva la campagna.

## Creare l’annuncio {#create-your-ad}

Dopo aver configurato il programma e le campagne, crea il nuovo annuncio.

1. Vai al canale, ad esempio LinkedIn o Facebook.
1. Crea un nuovo annuncio.
1. Seleziona una pagina di destinazione di Marketo come destinazione per l’invito all’azione nella campagna.
1. Aggiungi la stringa di query all’URL.

   >[!NOTE]
   >
   >**Esempio**
   >
   >Ecco come aggiungere tutte le informazioni impostate in un URL effettivo. Gli elementi sono separati da una e commerciale (&amp;):
   >
   >`www.marketo.com?**source**=Social-Paid&**comment**=Social-Paid_Facebook_NewGuide_NA&**camp**=abc&**kk=**xyz`
   >
   >* **source** è il Source della persona utilizzato come identificatore di canale
   >* **commento** è l&#39;identificatore univoco creato per ogni programma
   >* **camp** è la campagna in Facebook, LinkedIn o Google
   >* **kk** è la parola chiave o il nome della risorsa da acquisire
   >
   >**Questi quattro termini devono essere tutti minuscoli e non possono essere presenti spazi nell&#39;URL per l&#39;acquisizione di queste informazioni.**

## Best practice {#best-practices}

Utilizza un singolo tag canale per rappresentare tutto Digital Advertising oppure, se desideri confronti più granulari rispetto agli altri canali di marketing (ad esempio Social-Paid, Search-Paid, Display, Retargeting), utilizza più tag canale.

Quindi, imposta diversi programmi per ogni visualizzazione di reporting necessaria. Utilizza un ID comune come parametro nell’URL (BC, ad esempio) nella stringa di query se disponi di 10 aree che avviano insieme una &quot;Grande campagna&quot; e desideri visualizzare i risultati tra aree diverse.

Se desideri creare rapporti su ciascuna regione e sui risultati collettivi della Grande Campagna, crea 11 programmi, uno per ogni regione e uno per la Grande Campagna. Ogni programma fa riferimento solo ai caratteri pertinenti della stringa query (ad esempio BC).

C’è una sovrapposizione intenzionale nel conteggio delle persone tra la Grande Campagna e i programmi dell’area, pertanto non vorresti generare rapporti sul numero totale di persone per tutti gli 11 programmi, poiché alcune persone sono incluse sia nella Grande Campagna che in uno dei programmi dell’area.
