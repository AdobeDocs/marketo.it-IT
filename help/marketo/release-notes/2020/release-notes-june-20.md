---
unique-page-id: 37357276
description: Note sulla versione - Giugno 20 - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione - Giugno 20
exl-id: ffc39c9f-8c0c-45af-8ee6-f58971e230b9
translation-type: tm+mt
source-git-commit: d44f5e6f3fb24a25678e4d15ee4c6361b658556b
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 0%

---

# Note sulla versione: Giugno 20 {#release-notes-june}

Le seguenti funzionalità sono incluse nella versione del 20 giugno. Per informazioni sulla disponibilità delle funzioni, consulta la tua edizione Marketo .

>[!AVAILABILITY]
>
>Le caratteristiche indicate da una stella (![](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

**_Versioni_** trimestraliLe seguenti funzionalità saranno rilasciate il 5  **giugno 2020**.

## Marketo Engage core {#core-marketo-engage}

* **[Predictive Audiences](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=en#predictive-audiences)** ![ (stella)](assets/yellow-star.png): I nuovi filtri per l’elenco avanzato e la campagna avanzata gestiti da Adobe Sensei consentono di creare segmenti di pubblico basati sull’intelligenza artificiale per i programmi di marketing relativi a e-mail, eventi e webinar. Utilizza l’intelligenza artificiale per segmentare il pubblico in base alla probabilità del lead di registrarsi a un evento, partecipare a un evento o annullare l’abbonamento. Crea tipi di pubblico lookalike basati su programmi passati per replicare in modo efficiente il successo precedente. Raggiungi gli obiettivi di conversione con il tracciamento predittivo degli obiettivi e ottieni consigli su come perfezionare i segmenti di pubblico per i programmi evento.
* **Incremento e-mail in batch** ![ (stella)](assets/yellow-star.png): Miglioramento della funzionalità di marketing e-mail che ti consente di inviare fino a 3 milioni di e-mail batch all’ora. Abbiamo riprogettato l’elaborazione di batch di campagne e report e-mail per migliorare le prestazioni dei programmi e-mail e delle campagne e-mail batch. Ciò comporta un lead time più breve per l’invio e tempi di completamento più lunghi. Imposta gli invii di posta elettronica come faresti normalmente, non c&#39;è complessità aggiuntiva. Questo miglioramento è disponibile come componente aggiuntivo di prodotto che include anche un pacchetto Launch per i servizi di consegna, strumenti di consegna e-mail e più indirizzi IP dedicati.
* **[Integrazione del pubblico con Adobe Experience Cloud (AEC)](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**: Nuova integrazione di Adobe Experience Cloud (AEC) che consente di sincronizzare elenchi statici di lead noti da Marketo Engage con più applicazioni AEC per migliorare i programmi esistenti, sbloccare nuovi casi d’uso e orchestrare campagne multicanale. Questa integrazione include Adobe Analytics, Adobe Target, Adobe Experience Manager, Adobe Audience Manager e Adobe Advertising Cloud.
* **[Campi](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)** personalizzati membri del programma: Acquisire e utilizzare campi personalizzati relativi a un membro del programma. Utilizza questi nuovi campi nei moduli di Marketo Engage, visualizzali nell’elenco dei membri di un programma, sfruttali nei filtri e nei trigger di elenchi avanzati e includili in una nuova azione di flusso di campagne avanzate per automazione avanzata e personalizzazione più granulare. Possono anche essere importate ed esportate tramite l’interfaccia utente e le API. Miglioramento della funzionalità per oggetti dati e campi personalizzati.
* **Descrivi membro** del programma: Recupera i metadati dei membri del programma, consentendoti di importare ed esportare i dati dei campi personalizzati dei membri del programma utilizzando l’API REST. Miglioramento dell’API.
* **[Crea attività in Microsoft Dynamics](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)**: Crea attività per le vendite all’interno di Microsoft Dynamics utilizzando una nuova azione Flusso basata sul comportamento dei clienti acquisito nel Marketo Engage. Miglioramento dell’integrazione nativa di Microsoft Dynamics CRM.
* **Ottieni Modulo Utilizzato Dall’Endpoint** API Della Risorsa Elenco: Recupera un elenco di risorse dipendenti da un modulo. Miglioramento dell’API.
* **Imposta l’intestazione dell’e-mail tramite API**: Abilita la traduzione automatica e la localizzazione dei campi di preintestazione e-mail. Miglioramento dell’API.
* **Memorizzazione in cache** di immagini e file: Stiamo migliorando la stabilità del server di Marketo Engage servendo le risorse Immagine e File da una cache di 60 secondi.

## Marketing basato su account {#account-based-marketing}

![(stella)](assets/yellow-star.png)

* **Disponibilità generale di un nuovo account Discovery**

   * Il nuovo Account Discovery è un miglioramento della funzionalità di profilazione dell&#39;account che consente di scoprire nuovi account target netti per la strategia ABM in base al modello di profilo cliente ideale basato sull&#39;intelligenza artificiale. Visualizza, seleziona e importa i nuovi account consigliati, insieme ai relativi indicatori di dati di adattamento e intento basati sull’intelligenza artificiale.

<br> 

**_Rilascio in tutto il trimestre_**

Le seguenti caratteristiche sono su un ciclo non trimestrale e saranno rilasciate durante i prossimi mesi.

## Bizible {#bizible}

![(stella)](assets/yellow-star.png)

* **Integrazione** dei programmi di Marketo Engage: Recupera i dati del programma direttamente dal Marketo Engage per creare punti di contatto lungo il percorso di attribuzione in Bizible per accreditare in modo appropriato i programmi e-mail e di coinvolgimento. Miglioramento dell’integrazione dei Marketi Engage.
* **Integrazione delle attività di Marketo Engage (BETA)**: Trasferisci i dati delle attività di Marketo Engage direttamente in Bizible per creare punti di contatto nel percorso di clienti e in tutti i modelli di attribuzione. Alcuni esempi includono modifiche al punteggio lead, momenti interessanti, clic su e-mail o attività personalizzate. Miglioramento dell’integrazione dei Marketi Engage.
* **Integrazione degli attributi del cliente (BETA)** Bizible B2B: Questa è un’integrazione di Adobe Experience Cloud con Adobe Analytics che ti consente di inserire direttamente dati Bizible in Adobe Analytics per un’analisi più approfondita. Gli esempi includono l&#39;analisi del traffico del sito basata sull&#39;account e del contenuto in base al nome dell&#39;azienda, agli attributi dell&#39;account, alle opportunità di gestione delle relazioni con i clienti e agli individui di alto valore, come definiti dalla fase Ricavo e Funnel attribuiti da Bizible.
* **Filtri e miglioramenti** di Discover Bizible: Analizza i dati con i filtri per canale, canale secondario, campagna e segmento tra le dashboard. Rafforzare la visibilità dei dati con attributi più drill-down. Questo è un miglioramento per i nostri Discover Boards.
* **Sincronizzazione delle attività per Microsoft Dynamics**: Attribuisci le interazioni di vendita inserendo le attività di Microsoft Dynamics CRM nel percorso dei punti di contatto e tiene traccia di eventi quali chiamate, appuntamenti o attività associate ai lead o ai contatti. Miglioramento dell’integrazione con Microsoft Dynamics CRM.

## Informazioni sulle vendite {#sales-insight}

![(stella)](assets/yellow-star.png)

* **[Dashboard approfondimenti per CRM](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)** Salesforce: Stiamo riimmaginando la nostra capacità di Sales Insight con una nuova visibilità nei prossimi eventi e campagne di marketing per dare ai venditori la possibilità di rendere i consigli più rilevanti per i clienti e i potenziali clienti in base alle loro esigenze e ai loro interessi. I venditori possono anche visualizzare l’attività Contatto e Account nella timeline e accedere facilmente ai dettagli di attività aggiuntivi. Ulteriori informazioni su come aggiornare il pacchetto [qui](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/configuration-for-existing-customers.md).

<br> 

## Annunci {#announcements}

* **Aggiornamento** ITP 2.1+ RTP: A causa di modifiche ai criteri dei cookie per Safari, la capacità dei cookie RTP di monitorare gli utenti attraverso sessioni sullo stesso dominio sarà limitata da ITP a 1 o 7 giorni in base al browser e alla versione del browser utilizzati dal visitatore. Per tenere conto di ciò, stiamo implementando un nuovo servizio web per consentire l’impostazione dei cookie RTP con un’intestazione Set-Cookie tramite risposta HTTP. Ulteriori informazioni sono disponibili [qui](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603).

* **Modifiche** all’infrastruttura di campagna in batch: Stiamo aggiornando i nostri servizi per le campagne batch durante il resto dell&#39;anno. Si tratta di un aggiornamento senza soluzione di continuità che non influirà sulle campagne batch in corso e non determinerà un cambiamento di comportamento. Non è richiesta alcuna azione. Ulteriori informazioni sono disponibili in questo [Post sulla nazione](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374).

## Elementi obsoleti {#deprecations}

* **[Capo](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)** associato Munchkin: A partire dalla versione 159 di Munchkin JS, quando si richiama il metodo Associa lead , nella console del browser viene visualizzato un avviso di obsolescenza, che indica che la funzione verrà rimossa in una versione futura.  La pianificazione completa della rimozione verrà annunciata in una data successiva.

**_Webinar sul rilascio del prodotto_** [Guarda la ](https://engage.marketo.com/June-Release-2020-On-Demand.html) registrazione del nostro webinar sulle innovazioni del rilascio del prodotto del 20 giugno.
