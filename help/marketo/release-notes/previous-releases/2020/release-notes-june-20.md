---
unique-page-id: 37357276
description: Note sulla versione -20 giugno - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Giugno '20
exl-id: ffc39c9f-8c0c-45af-8ee6-f58971e230b9
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '1031'
ht-degree: 0%

---

# Note sulla versione: giugno 2020 {#release-notes-june}

Le seguenti funzioni sono incluse nella versione di giugno 2020. Verifica la disponibilità delle funzioni nella tua edizione di Marketo.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da un asterisco (![](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

**_Versioni trimestrali_** Le seguenti funzionalità verranno rilasciate il **5 giugno 2020**.

## Marketo Engage core {#core-marketo-engage}

* **[Predictive Audiences](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=en#predictive-audiences)** ![(star)](assets/yellow-star.png): i nuovi filtri per elenchi avanzati e campagne intelligenti basati su Adobe Sensei ti consentono di creare segmenti di pubblico basati sull’intelligenza artificiale per programmi di marketing di e-mail, eventi e webinar. Utilizza l’intelligenza artificiale per segmentare il pubblico in base alla probabilità di lead per registrarti a un evento, partecipare a un evento o annullare l’abbonamento. Crea tipi di pubblico simili in base a programmi passati per replicare in modo efficiente i successi precedenti. Raggiungi gli obiettivi di conversione con il tracciamento predittivo degli obiettivi e ottieni consigli su come perfezionare i segmenti di pubblico per i programmi evento.
* **Incremento e-mail in batch** ![(stella)](assets/yellow-star.png): è stata migliorata la funzionalità di e-mail marketing, che consente di inviare fino a 3 milioni di e-mail in batch all&#39;ora. Abbiamo riprogettato l’elaborazione delle campagne batch e dei rapporti e-mail per migliorare le prestazioni dei programmi e-mail e delle campagne e-mail batch. Ciò consente di ridurre il lead time di invio e di migliorare il tempo di completamento. La configurazione degli invii di e-mail normalmente non comporta complessità aggiuntive. Questo miglioramento è disponibile come componente aggiuntivo di prodotto che include anche un pacchetto di lancio dei servizi di consegna, strumenti di consegna e-mail e più indirizzi IP dedicati.
* **[Integrazione del pubblico con Adobe Experience Cloud (AEC)](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**: nuova integrazione Adobe Experience Cloud (AEC) che consente di sincronizzare elenchi statici di lead noti da Marketo Engage con più applicazioni AEC per migliorare i programmi esistenti, sbloccare nuovi casi d&#39;uso e orchestrare campagne multicanale. Questa integrazione include Adobe Analytics, Adobe Target, Adobe Experience Manager, Adobe Audience Manager e Adobe Advertising Cloud.
* **[Campi personalizzati del membro del programma](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)**: acquisire e utilizzare campi personalizzati su un membro del programma. Utilizza questi nuovi campi nei Marketo Engage Form, visualizzali nell’elenco dei membri di un programma, sfruttali nei filtri e nei trigger dell’elenco avanzato e includili in una nuova Azione di flusso di Smart Campaign per una maggiore automazione e una personalizzazione più granulare. Questi possono anche essere importati ed esportati tramite l’interfaccia utente e le API. Miglioramento della funzionalità per campi e oggetti dati personalizzati.
* **Descrivi membro del programma**: recupera i metadati dei membri del programma, consentendo di importare ed esportare i dati del campo personalizzato dei membri del programma tramite API REST. Miglioramento della nostra API.
* **[Crea attività in [!DNL Microsoft Dynamics]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)**: crea attività per le vendite in [!DNL Microsoft Dynamics] utilizzando una nuova azione di flusso basata sul comportamento del cliente acquisito in Marketo Engage. Miglioramento dell&#39;integrazione nativa di [!DNL Microsoft Dynamics] CRM.
* **Ottieni modulo utilizzato dall&#39;endpoint API per risorse di elenco**: recupera un elenco di risorse che dipendono da un modulo. Miglioramento della nostra API.
* **Imposta preintestazione e-mail tramite API**: abilita la traduzione e la localizzazione automatiche dei campi di preintestazione e-mail. Miglioramento della nostra API.
* **Memorizzazione in cache di immagini e file**: è in corso l&#39;aumento della stabilità del server Marketo Engage distribuendo le risorse di immagini e file da una cache di 60 secondi.

## Account-Based Marketing {#account-based-marketing}

![(stella)](assets/yellow-star.png)

* **Individuazione nuovo account generalmente disponibile**

   * La nuova funzione di individuazione account è un miglioramento della funzionalità di profilazione account che consente di individuare nuovi account target per la strategia ABM in base al modello di profilo cliente ideale basato sull’intelligenza artificiale. Visualizza, seleziona e importa nuovi account consigliati, insieme ai relativi indicatori di dati di idoneità e intento basati sull’intelligenza artificiale.

<br> 

**_Rilascio nel corso del trimestre_**

Le seguenti funzioni sono in un ciclo non trimestrale e verranno rilasciate nei prossimi mesi.

## [!DNL Bizible] {#bizible}

![(stella)](assets/yellow-star.png)

* **Integrazione dei programmi Marketo Engage**: estrarre i dati del programma direttamente da Marketo Engage per creare punti di contatto lungo il percorso di attribuzione in [!DNL Bizible] per accreditare in modo appropriato i programmi di e-mail e coinvolgimento. Miglioramento dell&#39;integrazione con Marketo Engage.
* **Integrazione delle attività di Marketo Engage (BETA)**: inserisci i dati delle attività di Marketo Engage direttamente in [!DNL Bizible] per creare punti di contatto nel percorso di clienti e in tutti i modelli di attribuzione. Alcuni esempi includono modifiche del punteggio di lead, momenti di interesse, clic su e-mail o altre attività personalizzate. Miglioramento dell&#39;integrazione con Marketo Engage.
* Integrazione degli attributi del cliente B2B **[!DNL Bizible](BETA)**: si tratta di un&#39;integrazione Adobe Experience Cloud con Adobe Analytics che consente di inserire dati Bizible selezionati direttamente in Adobe Analytics per un&#39;analisi più approfondita. Alcuni esempi includono il traffico del sito basato sull&#39;account e l&#39;analisi dei contenuti per nome della società, attributi dell&#39;account, opportunità di gestione delle relazioni con i clienti e singoli utenti di alto valore come definito da [!DNL Bizible] ricavi attribuiti e fase funnel.
* **[!DNL Bizible]Filtri di individuazione e miglioramenti**: Analizza i tuoi dati con filtri per canali, sottocanale, campagne e segmenti nelle dashboard. Maggiore visibilità dei dati con un maggior numero di attributi di espansione. Questo è un miglioramento alle nostre Discover Boards.
* **Sincronizzazione attività per[!DNL Microsoft Dynamics]**: attribuisci le interazioni di vendita inserendo [!DNL Microsoft Dynamics] attività di gestione delle relazioni con i clienti nel percorso di punti di contatto e tieni traccia di eventi quali chiamate, appuntamenti o attività associate ai tuoi lead o contatti. Miglioramento dell&#39;integrazione CRM di [!DNL Microsoft Dynamics].

## [!DNL Sales Insight] {#sales-insight}

![(stella)](assets/yellow-star.png)

* **[Dashboard approfondimenti per Salesforce CRM](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)**: stiamo riprogettando la funzionalità [!DNL Sales Insight] con una nuova visibilità dei prossimi eventi di marketing e campagne per consentire ai venditori di rendere i consigli più rilevanti per i clienti e i potenziali clienti in base alle loro esigenze e ai loro interessi. I venditori possono inoltre visualizzare le attività di contatto e account entro la timeline e accedere facilmente a ulteriori dettagli sull&#39;attività. Ulteriori dettagli su come aggiornare il pacchetto [qui](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md).

<br> 

## Annunci {#announcements}

* **Aggiornamento RTP ITP 2.1+**: a causa delle modifiche ai criteri dei cookie per [!DNL Safari], la possibilità dei cookie RTP di tenere traccia degli utenti tra sessioni sullo stesso dominio sarà limitata da ITP a 1 o 7 giorni in base alla versione del browser e del browser utilizzati dal visitatore. Per questo, stiamo implementando un nuovo servizio web per consentire l’impostazione dei cookie RTP con un’intestazione Set-Cookie tramite risposta HTTP. Ulteriori informazioni sono disponibili [qui](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603).

* **Modifiche all&#39;infrastruttura delle campagne batch**: i servizi delle campagne batch verranno aggiornati per il resto dell&#39;anno. Si tratterà di un aggiornamento senza soluzione di continuità che non influirà sulle campagne batch in corso e non comporterà un cambiamento di comportamento. Non è richiesta alcuna azione. Trova ulteriori dettagli in questo [Post nazione](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374).

## Funzionalità deprecate {#deprecations}

* **[Associa lead Munchkin](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: a partire dalla versione 159 di [!DNL Munchkin] JS, quando viene richiamato il metodo Associa lead verrà registrato un avviso di elementi obsoleti nella console del browser, a indicare che la funzionalità verrà rimossa in una versione futura.  La pianificazione completa degli elementi obsoleti verrà annunciata in un secondo momento.

**_Webinar sulla versione del prodotto_** [Guarda la registrazione](https://engage.marketo.com/June-Release-2020-On-Demand.html) del nostro webinar sulle innovazioni della versione del prodotto di giugno 20.
