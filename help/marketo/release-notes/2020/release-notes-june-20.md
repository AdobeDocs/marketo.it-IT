---
unique-page-id: 37357276
description: Note sulla versione - Giugno 20 - Marketo Docs - Documentazione prodotto
title: Note sulla versione - Giugno 20
translation-type: tm+mt
source-git-commit: b33f5ed707a1377daad51191cc6dd9f093138258
workflow-type: tm+mt
source-wordcount: '1073'
ht-degree: 0%

---


# Note sulla versione: Giugno 20 {#release-notes-june}

Le seguenti funzionalità sono incluse nella release di giugno 20. Per informazioni sulla disponibilità delle funzionalità, consulta la versione di Marketo.

>[!AVAILABILITY]
>
>Le caratteristiche indicate da una stella ( ![(star)](assets/star-yellow.svg)) possono essere aggiunte a pagamento. Per ulteriori informazioni, contattate il rappresentante del Marketo Engage.

**_Rilasci_** trimestraliLe seguenti funzionalità verranno rilasciate il 5  **giugno 2020**.

## Marketo Engage di base {#core-marketo-engage}

* **[Predictive Audiences](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=en#predictive-audiences)** ![(star)](assets/star-yellow.svg): I nuovi filtri Elenco avanzato e Campagna intelligente basati su  Adobe Sensei consentono di creare segmenti di pubblico dotati di tecnologia AI per i programmi di marketing e-mail, eventi e webinar. Utilizzate l&#39;API per segmentare il pubblico in base alla probabilità principale di registrarsi a un evento, partecipare a un evento o annullare la sottoscrizione. Crea tipi di pubblico simili in base ai programmi passati per replicare in modo efficiente il successo precedente. Raggiungete gli obiettivi di conversione con il tracciamento predittivo degli obiettivi e ottenete suggerimenti su come perfezionare i segmenti di pubblico per i programmi dell&#39;evento.
* **Incremento** ![ e-mail batch (stella)](assets/star-yellow.svg): È stata migliorata la nostra capacità di marketing e-mail che consente di inviare fino a 3 milioni di e-mail batch all&#39;ora. Abbiamo riprogettato la nostra elaborazione batch di campagne e report e-mail per migliorare le prestazioni dei programmi e-mail e delle campagne batch. Questo riduce i tempi di invio e migliora i tempi di completamento. Configurate le vostre e-mail come fareste normalmente, senza alcuna complessità aggiuntiva. Questo miglioramento è disponibile come componente aggiuntivo di prodotto che include anche un pacchetto di lancio di Servizi di consegna, strumenti di consegna e-mail e più indirizzi IP dedicati.
* **[Integrazione dell&#39;audience con Adobe Experience Cloud (AEC)](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**: Nuova integrazione Adobe Experience Cloud (AEC) che consente di sincronizzare elenchi statici di lead noti da Marketo Engage con più applicazioni AEC per migliorare i programmi esistenti, sbloccare nuovi casi di utilizzo e orchestrare campagne multicanale. Questa integrazione include  Adobe Analytics,  Adobe Target, Adobe Experience Manager, Adobe Audience Manager e Adobe Advertising Cloud.
* **[Campi](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)** personalizzati membri del programma: Acquisire e utilizzare campi personalizzati su un membro del programma. Utilizzate questi nuovi campi nei moduli di Marketo Engage, visualizzateli nell&#39;elenco dei membri di un programma, sfruttateli nei filtri e nelle attivazioni per l&#39;elenco avanzato e includeteli in una nuova azione di flusso delle campagne Smart Campaign per migliorare l&#39;automazione e la personalizzazione più granulare. Questi possono essere importati ed esportati anche tramite l’interfaccia utente e le API. Miglioramento della funzionalità di oggetti dati e campi personalizzati.
* **Descrivi membro** del programma: Recuperate i metadati dei membri del programma, per consentirvi di importare ed esportare i dati dei campi personalizzati dei membri del programma mediante l&#39;API REST. Miglioramento dell&#39;API.
* **[Crea attività in Microsoft Dynamics](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)**: Crea attività per le vendite all&#39;interno di Microsoft Dynamics utilizzando una nuova azione di flusso basata sul comportamento del cliente acquisito nel Marketo Engage. Miglioramento all&#39;integrazione nativa di Microsoft Dynamics CRM.
* **Ottieni modulo utilizzato dall&#39;endpoint** API della risorsa elenco: Recuperate un elenco di risorse dipendenti da un modulo. Miglioramento dell&#39;API.
* **Impostate l&#39;intestazione dell&#39;e-mail tramite API**: Abilitate la traduzione automatica e la localizzazione dei campi di intestazione e-mail. Miglioramento dell&#39;API.
* **Memorizzazione delle immagini e dei file nella cache**: Stiamo migliorando la stabilità del server di Marketo Engage distribuendo le risorse Immagine e File da una cache di 60 secondi.

## Marketing basato su account {#account-based-marketing}

![(stella)](assets/star-yellow.svg)

* **Nuova individuazione account disponibile in genere**

   * Il nuovo Account Discovery è un miglioramento alla nostra funzionalità di Account Profiling che ti permette di scoprire nuovi account target per la tua strategia ABM basati sul modello di profilo cliente ideale basato sull&#39;intelligenza artificiale. Visualizza, seleziona e importa i nuovi account consigliati, insieme ai relativi indicatori di dati di adattamento e intento basati su AI.

<br> 

**_Rilascio per tutto il trimestre_**

Le seguenti funzionalità sono su un ciclo non trimestrale e verranno rilasciate nei prossimi mesi.

## Bizible {#bizible}

![(stella)](assets/star-yellow.svg)

* **Integrazione** dei programmi di Marketo Engage: Estrarre i dati del programma direttamente dal Marketo Engage per creare punti di contatto lungo il percorso di attribuzione in Bizible e accreditare in modo appropriato e-mail e programmi di coinvolgimento. Miglioramento dell&#39;integrazione dei nostri Marketi Engage.
* **Integrazione attività Marketo Engage (BETA)**: Inserite i dati dell&#39;attività di Marketo Engage direttamente in Bizible per creare punti di contatto nel percorso cliente e in tutti i modelli di attribuzione. Alcuni esempi includono modifiche alla valutazione dei lead, momenti interessanti, clic su e-mail o qualsiasi attività personalizzata. Miglioramento dell&#39;integrazione dei nostri Marketi Engage.
* **Integrazione degli attributi del cliente B2B (Bizible B2B Customer Attributes Integration, BETA)**: Questa è un&#39;integrazione Adobe Experience Cloud con  Adobe Analytics che consente di portare alcuni dati Bizible direttamente in  Adobe Analytics per un&#39;analisi più approfondita. Alcuni esempi includono l&#39;analisi del traffico del sito e del contenuto basata su conto in base al nome della società, agli attributi del conto, alle opportunità CRM e agli individui di alto valore, come definiti dalle entrate e dallo stadio funnel attribuibili Bizible.
* **Filtri e miglioramenti** per la scoperta della bizible: Analizzare i dati con canali, canali secondari, campagne e filtri per segmenti attraverso le dashboard. Maggiore visibilità dei dati con più attributi di drill-down. Questo è un miglioramento per le nostre bacheche Discover.
* **Sincronizzazione attività per Microsoft Dynamics**: Attribuisci le interazioni di vendita inserendo le attività di Microsoft Dynamics CRM nel percorso dei punti di contatto e monitora eventi quali chiamate, appuntamenti o attività associate ai tuoi lead o contatti. Miglioramento all&#39;integrazione con Microsoft Dynamics CRM.

## Informazioni sulle vendite {#sales-insight}

![(stella)](assets/star-yellow.svg)

* **[Pannello Insights per Salesforce CRM](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)**: Stiamo ripensando la nostra Sales Insight funzionalità con una nuova visibilità sugli eventi di marketing e sulle campagne per offrire ai venditori la possibilità di rendere le raccomandazioni più rilevanti per i clienti e i potenziali clienti in base alle loro esigenze e ai loro interessi. I venditori possono inoltre visualizzare l&#39;attività Contatto e Account nella timeline e accedere facilmente ai dettagli dell&#39;attività aggiuntiva. Maggiori informazioni su come aggiornare il pacchetto [qui](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/configuration-for-existing-customers.md).

<br> 

## Annunci {#announcements}

* **Aggiornamento** ITP 2.1+ RTP: A causa delle modifiche ai criteri dei cookie per Safari, la capacità dei cookie RTP di monitorare gli utenti in più sessioni sullo stesso dominio sarà limitata da ITP a 1 o 7 giorni in base al browser e alla versione del browser utilizzati dal visitatore. Per rendere conto di ciò, stiamo implementando un nuovo servizio Web per consentire l&#39;impostazione dei cookie RTP con un&#39;intestazione Set-Cookie tramite la risposta HTTP. Ulteriori informazioni sono disponibili [qui](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603).

* **Modifiche** all&#39;infrastruttura delle campagne batch: Stiamo aggiornando i nostri servizi di campagna batch per tutto il resto dell&#39;anno. Si tratterà di un aggiornamento senza soluzione di continuità che non influirà sulle campagne batch in corso e non determinerà un cambiamento di comportamento. Non è richiesta alcuna azione. Per maggiori dettagli, vedere [Nation post](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374).

## Deprecazioni {#deprecations}

* **[Munchkin Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: A partire dalla versione 159 di Munchkin JS, quando viene richiamato il metodo Associate Lead, verrà registrato un avviso di obsolescenza nella console del browser, a indicare che la funzione verrà rimossa in una versione futura.  Il programma completo di obsolescenza verrà annunciato in una data successiva.

**_Webinar_** [sulla versione del prodottoGuardate la ](https://engage.marketo.com/June-Release-2020-On-Demand.html) registrazione del webinar sulle innovazioni nella release del prodotto di giugno 2006.
