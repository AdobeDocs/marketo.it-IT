---
description: Note sulla versione - Maggio 2021 - Documentazione di Marketo - Documentazione del prodotto
title: Note sulla versione - Maggio 2021
exl-id: e3de60a2-17bd-4760-848e-6e931ad85b3c
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1446'
ht-degree: 0%

---

# Note sulla versione: maggio 2021 {#release-notes-may-21}

Le seguenti funzioni sono incluse nella versione di maggio 2021. Verifica la disponibilità delle funzioni nella tua edizione di Marketo.

>[!AVAILABILITY]
>
>Caratteristiche contrassegnate da una stella (![](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

**_Versioni trimestrali_**

Le seguenti funzioni verranno rilasciate il **7 maggio 2021**.

## Esperienze basate su account {#Account-based-eaperiences}

* **Elenchi avanzati account (disponibilità generale)** ![](assets/yellow-star.png): identifica e qualifica dinamicamente gli account con gli attributi di account e persona desiderati per eseguire il targeting nelle campagne di marketing cross-channel e invia avvisi tempestivi alle vendite per chiudere le offerte più rapidamente. Questa nuova funzionalità consente una solida automazione delle strategie di marketing basate sull’account. Gli elenchi avanzati account sono disponibili per i clienti con Target Account Management che hanno l’esperienza di utente di nuova generazione.

## Esperienza utente di nuova generazione {#next-generation-user-experience}

Con l’anteprima della ricerca globale, gli addetti al marketing possono vedere rapidamente dove esiste una risorsa condivisa nella loro istanza. Le schede del browser visualizzano la posizione per migliorare la navigazione in Marketing Activities o Design Studio. La struttura ad albero e i filtri di ricerca globali aggiuntivi consentono di perfezionare i criteri di ricerca. È stata ripristinata la funzionalità di trascinamento all’interno della struttura, che consente di spostare cartelle e risorse in modo rapido ed efficiente all’interno delle aree dell’app principale. Le icone appena aggiornate (che soddisfano gli standard di accessibilità di Adobe) e i badge di stato consentono agli addetti al marketing di distinguere rapidamente e facilmente cartelle e risorse nella struttura e di identificare lo stato di programmi e risorse.

## Automazione dell’esperienza {#experience-automation}

* **Eseguire i passaggi del flusso della campagna**: semplifica i flussi di lavoro per la creazione di campagne e migliora le prestazioni delle campagne, con un nuovo passaggio di flusso per le campagne intelligenti. Crea e salva campagne modello centralizzate per attività ripetitive nell’area di lavoro, come la normalizzazione del codice paese, da chiamare ed eseguire da qualsiasi campagna avanzata tramite il nuovo passaggio di flusso &quot;Esegui campagna&quot;. Le campagne collegate verranno eseguite nell’ordine designato e garantiranno il completamento dell’attività prima di passare al passaggio successivo del flusso. Modifica rapidamente il flusso in una sola campagna centralizzata per aggiornare ogni Smart Campaign che lo utilizza al fine di semplificare la gestione dei dati, il punteggio dei lead e l’indirizzamento dei flussi di lavoro.

## Orchestrazione cross-channel {#cross-channel-orchestration}

* **Campi dati sensibili in Forms**: le informazioni personali (PII) dei clienti Protect non vengono visualizzate nei moduli Adobe Marketo Engage definendo i campi dati come sensibili e limitando la precompilazione dei moduli per tali campi. Ogni volta che un visitatore visualizza un modulo nella pagina di destinazione, i campi definiti sensibili non mostrano alcun dato precompilato.

* **Blocca invio modulo spam**: esegui il Protect del database Adobe Marketo Engage da dati indesiderati che possono causare avvisi non validi alle vendite, attivare i backlog delle campagne e creare attività indesiderate. Il nuovo meccanismo di convalida rifiuta l’invio di moduli non validi e interrompe gli attacchi di bot. I dati sono più puliti e le campagne di marketing vengono eseguite come previsto, riducendo al minimo il rischio di inviare lead non qualificati per le vendite.

* **Avviso di approvazione del programma e-mail**: evita l’invio di e-mail errate quando vengono apportate nuove modifiche a un programma precedentemente approvato.  L’avviso funge da guardrail quando un addetto al marketing applica le modifiche a un’e-mail già approvata, ma poi dimentica di approvare le modifiche più recenti e invia l’e-mail a un pubblico ampio senza contenuto, contenuto errato o contenuto precedente.

* **Escludere l’attività Bots e-mail**: evita avvisi di vendita involontari e rapporti e-mail imprecisi tramite la nuova funzionalità di filtro delle attività dei bot e-mail. Identificare e filtrare le aperture e i clic che possono essere associati ai bot e-mail esaminando i collegamenti che portano a falsi attivatori e avvisi di vendita o a rapporti errati.

## Miglioramenti API {#api-enhancements}

Diversi aggiornamenti critici alle API Bulk e Lead, tra cui la possibilità di esportare dati di oggetti personalizzati in blocco, associare la società al lead in blocco, la possibilità di filtrare l’estrazione di attività in blocco in base a un attributo principale e la possibilità di creare e aggiornare l’iscrizione al programma.

* **Nidifica programmi evento**: in Adobe Marketo Engage è possibile creare, clonare o spostare programmi evento in altri tipi di programmi. Questa funzionalità è ora consentita nell’API delle risorse.

* **API del programma di eliminazione migliorata**: consente alle applicazioni integrate di eliminare i programmi contenenti ulteriori tipi di risorse, senza richiedere agli utenti di farlo manualmente da Adobe Marketo Engage.

* **Iscrizione al programma**: gli addetti al marketing possono eseguire query su tutti i record dei membri del programma per un programma selezionato in base a criteri diversi, ad esempio lo stato dei membri del programma. Condividi queste informazioni con un’applicazione esterna, uno strumento di business intelligence o Adobe Experience Cloud per migliorare la segmentazione e creare un coinvolgimento più mirato.

* **Estrazione oggetto personalizzato in blocco**: l’esportazione di dati in blocco integra le funzionalità di importazione già disponibili per gli analisti di dati in Adobe Marketo Engage. Ora possono estrarre in blocco i dati memorizzati negli oggetti personalizzati Adobe Marketo Engage di primo livello, caricarli in un’altra applicazione, data warehouse o strumento BI (Business Intelligence) per ottenere informazioni migliori sui dati nell’istanza Adobe Marketo Engage.  Lo spostamento in massa dei dati di un oggetto personalizzato è bidirezionale e può essere pianificato in un momento opportuno.

* **API metadati campi personalizzati**: risparmia tempo automatizzando la creazione di campi personalizzati durante la configurazione delle integrazioni Adobe Marketo Engage con un’applicazione di terze parti. Questa automazione offre vantaggi soprattutto ai clienti con più istanze di Adobe Marketo Engage, che ora possono semplificare la creazione di campi personalizzati che in passato richiedevano un lavoro manuale in ogni istanza. Semplifica la creazione di campi personalizzati e risparmia tempo su questa attività che consuma risorse.

* **API di estrazione attività in blocco**: acquisisci il controllo sulla quantità e sul tipo di dati durante l’esecuzione di estrazioni in blocco. Escludi i punti di dati non necessari e controlla il numero di chiamate API necessarie per estrarre in blocco i dati dell’attività.  Ad esempio, seleziona e-mail aperte, visita una pagina web o modifica nel punteggio del lead e lascia da parte altre modifiche di valore che non desideri analizzare. Semplifica il processo per ridurre il numero di chiamate API e la pulizia dei dati.

* **API lead**: identifica i lead in Adobe Marketo Engage a cui è associato l’Adobe ECID (ID Experience Cloud).  I clienti Adobe Marketo Engage possono creare un elenco di lead da una campagna selezionata e utilizzare gli ECID (ID Experience Cloud) per creare rapporti in Adobe Analytics per tale elenco specifico. L’integrazione tra Adobe Marketo Engage e Adobe Experience Cloud offre opportunità illimitate di segmentazione, targeting e reporting.

* **API di importazione lead in blocco**: controlla l’importazione di lead in blocco e le risorse necessarie. Questo miglioramento crea un’associazione tra lead e azienda durante il processo di importazione di lead in blocco. Aumenta l’efficienza e l’utilizzo dei dati, e riduci l’utilizzo in caso di chiamate API.

* **Integrazione basata su API Web per i clienti Microsoft Dynamics Online**: MS Dynamics Web API è stato introdotto con la versione 8.0 del protocollo REST e implementa OData (Open Data Protocol) v4. OData è uno standard OASIS (Organization for the Advancement of Structured Information Standards) per la creazione e l&#39;utilizzo di servizi RESTful su rich data. I clienti Adobe Marketo Engage che richiedono l’integrazione con Microsoft Dynamics utilizzando questo metodo sono attualmente in fase di migrazione alla connessione basata su API Web da SOAP (Simple Object Access Protocol).

## Ambiente dati di marketing {#marketing-data-environment}

* **Esportazione XLSX**: abbiamo aggiornato le funzionalità di esportazione in tutto il prodotto per supportare XLSX al posto di XLS. Ciò significa che in qualsiasi punto del prodotto in cui è attualmente supportata l’esportazione XLS, questa opzione verrà sostituita da un’opzione per l’esportazione in XLSX. Questa modifica influirà sui nomi dei file per tutte le esportazioni Excel di report e altri dati da Adobe Marketo Engage.

* **Ricerca per ID lead**: accesso rapido alla ricerca di record lead per ID lead Adobe Marketo Engage nel database lead o nell’elenco statico. Nella finestra Ricerca rapida digitare `[id]` con il numero corrispondente, verranno visualizzate le informazioni sul lead. Gli utenti possono rivedere rapidamente i dettagli di lead, società o opportunità.

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Integrazione con LinkedIn Lead Gen Forms (Beta)**: ottieni una visibilità approfondita sulla spesa del canale LinkedIn e sul ROI con la soluzione di attribuzione Bizible Premium. Grazie all’integrazione più recente con LinkedIn Lead Gen Forms, Bizible ottiene informazioni approfondite sui moduli inviati all’interno della piattaforma LinkedIn. Questi riempimenti di modulo vengono confrontati con i lead provenienti dalla tua istanza di CRM (Customer Relationship Management) o Adobe Marketo Engage in modo che siano idonei per l’attribuzione e possano essere tracciati rispetto agli altri impegni di marketing.

## Annunci {#announcements}

* **Piattaforme di switching per la documentazione sui prodotti Marketo**: siamo entusiasti di annunciare che la documentazione del prodotto Marketo è stata aggiunta ad Adobe Experience League a partire da venerdì 7 maggio. Potrai comunque utilizzare l’URL: docs.marketo.com e, se hai già degli articoli segnalibri, verrai reindirizzato. Tutti i documenti sui prodotti sono disponibili sulla nuova piattaforma, con miglioramenti pianificati per la fine dell’anno.

* **Amministrazione semplificata degli utenti e Single Sign-On con tecnologia Adobe Identity System**: a partire da luglio 2021, ai nuovi clienti Adobe Marketo Engage verrà effettuato l’onboarding utilizzando le credenziali utente Adobe. La migrazione dei clienti attuali al sistema di identità integrato non avverrà fino alla metà del 2022 e non è richiesta alcuna azione da parte del cliente fino a nuovo avviso. Il Single Sign-On consente agli amministratori IT/della sicurezza di gestire più istanze di prodotto Adobe Marketo Engage insieme ad altre soluzioni Experience Cloud e di configurare il SSO (Shared Services Organization) tramite una console comune. Gli amministratori possono gestire in modo semplice gruppi di utenti e adesioni utente tramite un Admin Console comune.

**_Webinar sulla versione del prodotto_**

[Webinar sulla versione del Marketo Engage di maggio 2021](https://engage.marketo.com/May_21_Release_webinar_RegistrationPage.html)
