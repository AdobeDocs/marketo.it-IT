---
unique-page-id: 37357276
description: Note sulla versione -20 giugno - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Giugno '20
exl-id: ffc39c9f-8c0c-45af-8ee6-f58971e230b9
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 0%

---

# Note sulla versione: giugno 2020 {#release-notes-june}

Le seguenti funzioni sono incluse nella versione di giugno 2020. Verifica la disponibilità delle funzioni nella tua edizione di Marketo.

>[!AVAILABILITY]
>
>Caratteristiche contrassegnate da una stella (![](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

**_Versioni trimestrali_** Le seguenti funzioni verranno rilasciate il **5 giugno 2020**.

## Marketo Engage core {#core-marketo-engage}

* **[Predictive Audiences](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=en#predictive-audiences)** ![(stella)](assets/yellow-star.png): i nuovi filtri per elenchi avanzati e campagne intelligenti basati su Adobe Sensei ti consentono di creare segmenti di pubblico basati sull’intelligenza artificiale per e-mail, eventi e programmi di marketing basati su webinar. Utilizza l’intelligenza artificiale per segmentare il pubblico in base alla probabilità di lead per registrarti a un evento, partecipare a un evento o annullare l’abbonamento. Crea tipi di pubblico simili in base a programmi passati per replicare in modo efficiente i successi precedenti. Raggiungi gli obiettivi di conversione con il tracciamento predittivo degli obiettivi e ottieni consigli su come perfezionare i segmenti di pubblico per i programmi evento.
* **Incremento e-mail in batch** ![(stella)](assets/yellow-star.png): miglioramento della funzionalità di e-mail marketing, che consente di inviare fino a 3 milioni di e-mail in batch all’ora. Abbiamo riprogettato l’elaborazione delle campagne batch e dei rapporti e-mail per migliorare le prestazioni dei programmi e-mail e delle campagne e-mail batch. Ciò consente di ridurre il lead time di invio e di migliorare il tempo di completamento. La configurazione degli invii di e-mail normalmente non comporta complessità aggiuntive. Questo miglioramento è disponibile come componente aggiuntivo di prodotto che include anche un pacchetto di lancio dei servizi di consegna, strumenti di consegna e-mail e più indirizzi IP dedicati.
* **[Integrazione del pubblico con Adobe Experience Cloud (AEC)](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**: nuova integrazione di Adobe Experience Cloud (AEC) che consente di sincronizzare elenchi statici di lead noti dal Marketo Engage con più applicazioni AEC per migliorare i programmi esistenti, sbloccare nuovi casi d’uso e orchestrare campagne multicanale. Questa integrazione include Adobe Analytics, Adobe Target, Adobe Experience Manager, Adobe Audience Manager e Adobe Advertising Cloud.
* **[Campi personalizzati del membro del programma](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)**: acquisisci e utilizza campi personalizzati su un membro del programma. Utilizza questi nuovi campi nei moduli di Marketo Engage, visualizzali nell’elenco dei membri di un programma, sfruttali nei filtri e nei trigger dell’elenco avanzato e includili in una nuova Azione di flusso di Smart Campaign per una maggiore automazione e una personalizzazione più granulare. Questi possono anche essere importati ed esportati tramite l’interfaccia utente e le API. Miglioramento della funzionalità per campi e oggetti dati personalizzati.
* **Descrivi membro programma**: recupera i metadati dei membri del programma, consentendo di importare ed esportare i dati dei campi personalizzati dei membri del programma tramite API REST. Miglioramento della nostra API.
* **[Crea attività in Microsoft Dynamics](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)**: crea attività per le vendite in Microsoft Dynamics utilizzando una nuova azione di flusso basata sul comportamento del cliente acquisito nel Marketo Engage. Miglioramento dell&#39;integrazione nativa di Microsoft Dynamics CRM.
* **Ottieni modulo utilizzato dall’endpoint API per risorse di elenco**: recupera un elenco di risorse che dipendono da un modulo. Miglioramento della nostra API.
* **Impostare la preintestazione e-mail tramite API**: abilita la traduzione e la localizzazione automatiche dei campi di preintestazione e-mail. Miglioramento della nostra API.
* **Memorizzazione in cache di immagini e file**: stiamo migliorando la stabilità del server di Marketo Engage distribuendo risorse di file e immagini da una cache di 60 secondi.

## Account-Based Marketing {#account-based-marketing}

![(stella)](assets/yellow-star.png)

* **Rilevamento di nuovi account generalmente disponibile**

   * La nuova funzione di individuazione account è un miglioramento della funzionalità di profilazione account che consente di individuare nuovi account target per la strategia ABM in base al modello di profilo cliente ideale basato sull’intelligenza artificiale. Visualizza, seleziona e importa nuovi account consigliati, insieme ai relativi indicatori di dati di idoneità e intento basati sull’intelligenza artificiale.

<br> 

**_Rilascio nel corso del trimestre_**

Le seguenti funzioni sono in un ciclo non trimestrale e verranno rilasciate nei prossimi mesi.

## Bizible {#bizible}

![(stella)](assets/yellow-star.png)

* **Integrazione dei programmi di Marketo Engage**: estrai i dati del programma direttamente dal Marketo Engage per creare punti di contatto lungo il percorso di attribuzione in Bizible, in modo da assegnare il giusto credito ai programmi di e-mail e coinvolgimento. Miglioramento dell’integrazione del Marketo Engage.
* **Integrazione delle attività di Marketo Engage (BETA)**: inserisci i dati delle attività di Marketo Engage direttamente in Bizible per creare punti di contatto nel percorso di clienti e in tutti i modelli di attribuzione. Alcuni esempi includono modifiche del punteggio di lead, momenti di interesse, clic su e-mail o altre attività personalizzate. Miglioramento dell’integrazione del Marketo Engage.
* **Integrazione di attributi cliente B2B (BETA) Bizible**: si tratta di un’integrazione di Adobe Experience Cloud con Adobe Analytics che consente di inserire dati specifici di Bizible direttamente in Adobe Analytics per un’analisi più approfondita. Alcuni esempi includono il traffico del sito basato sull’account e l’analisi dei contenuti per nome della società, attributi dell’account, opportunità di gestione delle relazioni con i clienti e singoli individui di alto valore come definito dalle entrate attribuite Bizible e dalla fase funnel.
* **Filtri e miglioramenti Bizible Discover**: analizza i dati con filtri di canale, sottocanale, campagna e segmento nelle dashboard. Maggiore visibilità dei dati con un maggior numero di attributi di espansione. Questo è un miglioramento alle nostre Discover Boards.
* **Sincronizzazione attività per Microsoft Dynamics**: attribuisci le interazioni di vendita inserendo le attività di Microsoft Dynamics CRM nel percorso dei punti di contatto e tieni traccia di eventi come chiamate, appuntamenti o attività associate ai lead o ai contatti. Miglioramento dell’integrazione con Microsoft Dynamics CRM.

## Insight sulle vendite {#sales-insight}

![(stella)](assets/yellow-star.png)

* **[Dashboard approfondimenti per Salesforce CRM](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)**: stiamo rinnovando la nostra funzionalità di approfondimento delle vendite con una nuova visibilità sui prossimi eventi e campagne di marketing per dare ai venditori la possibilità di rendere i consigli più rilevanti per i clienti e i potenziali clienti in base alle loro esigenze e ai loro interessi. I venditori possono inoltre visualizzare le attività di contatto e account entro la timeline e accedere facilmente a ulteriori dettagli sull&#39;attività. Ulteriori dettagli su come aggiornare il pacchetto [qui](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md).

<br> 

## Annunci {#announcements}

* **Aggiornamento RTP ITP 2.1+**: a causa delle modifiche alla policy sui cookie per Safari, la capacità dei cookie RTP di tenere traccia degli utenti tra sessioni diverse sullo stesso dominio sarà limitata da ITP a 1 o 7 giorni in base al browser e alla versione del browser utilizzati dal visitatore. Per questo, stiamo implementando un nuovo servizio web per consentire l’impostazione dei cookie RTP con un’intestazione Set-Cookie tramite risposta HTTP. Ulteriori informazioni sono disponibili [qui](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603).

* **Modifiche all’infrastruttura della campagna in batch**: stiamo aggiornando i servizi delle campagne batch nel resto dell’anno. Si tratterà di un aggiornamento senza soluzione di continuità che non influirà sulle campagne batch in corso e non comporterà un cambiamento di comportamento. Non è richiesta alcuna azione. Ulteriori dettagli in [Post nazionale](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374).

## Obsoleti {#deprecations}

* **[Lead associato Munchkin](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: a partire dalla versione 159 di Munchkin JS, quando viene richiamato il metodo Associate Lead, nella console del browser viene registrato un avviso di elementi obsoleti che indica che la funzione verrà rimossa in una versione futura.  La pianificazione completa degli elementi obsoleti verrà annunciata in un secondo momento.

**_Webinar sulla versione del prodotto_** [Guarda la registrazione](https://engage.marketo.com/June-Release-2020-On-Demand.html) del webinar sulle innovazioni del rilascio dei prodotti del 20 giugno.
