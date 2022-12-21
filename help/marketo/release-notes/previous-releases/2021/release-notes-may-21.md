---
description: Note sulla versione - Maggio 2021 - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione - Maggio 2021
exl-id: e3de60a2-17bd-4760-848e-6e931ad85b3c
source-git-commit: 115b6e97978778a1d1e13478adf6fee625aa5257
workflow-type: tm+mt
source-wordcount: '1446'
ht-degree: 0%

---

# Note sulla versione: Maggio 2021 {#release-notes-may-21}

Le seguenti funzionalità sono incluse nella versione del 21 maggio. Per informazioni sulla disponibilità delle funzioni, consulta la tua edizione Marketo .

>[!AVAILABILITY]
>
>Caratteristiche indicate da una stella (![](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

**_Versioni trimestrali_**

Le seguenti funzionalità verranno rilasciate il **7 maggio 2021**.

## Esperienze basate su account {#Account-based-eaperiences}

* **Elenchi smart account (disponibilità generale)** ![](assets/yellow-star.png): Identifica e qualifica in modo dinamico gli account con gli attributi desiderati dell’account e della persona per eseguire il targeting in campagne di marketing cross-channel e invia avvisi tempestivi alle vendite per chiudere le offerte più rapidamente. Questa nuova funzionalità consente una solida automazione delle strategie di marketing basate su account. Gli elenchi smart account sono disponibili per i clienti con Gestione account di Target che fanno parte dell’esperienza utente di nuova generazione.

## Esperienza utente di nuova generazione {#next-generation-user-experience}

Con l’anteprima di ricerca globale, gli addetti al marketing possono vedere rapidamente dove esiste una risorsa condivisa nella loro istanza. Le schede del browser visualizzano il percorso per migliorare la navigazione in Marketing Activities o Design Studio. Per perfezionare i criteri di ricerca, sono disponibili altri filtri ad albero e filtri di ricerca globali. È stata ripristinata la funzionalità di trascinamento all’interno della struttura, che consente di spostare cartelle e risorse in modo rapido ed efficiente nelle aree dell’app principale. Le icone appena aggiornate (conformi agli standard di accessibilità di Adobe) e i badge di stato consentono agli addetti al marketing di distinguere rapidamente e facilmente tra cartelle e risorse nella struttura e di identificare lo stato di programmi e risorse.

## Automazione delle esperienze {#experience-automation}

* **Esegui i passaggi del flusso di campagna**: Semplifica i flussi di lavoro per la creazione di campagne e migliora le prestazioni delle campagne con un nuovo passaggio di flusso per le campagne avanzate. Crea e salva campagne modello centralizzate per attività ripetitive nell’area di lavoro, ad esempio la normalizzazione del codice del paese, da chiamare ed eseguire da qualsiasi campagna avanzata tramite il nuovo passaggio di flusso &quot;Esegui campagna&quot;. Le campagne collegate vengono eseguite nell’ordine indicato e assicurano il completamento dell’attività prima di passare alla fase di flusso successiva. Modifica rapidamente il flusso in una sola campagna centralizzata per aggiornare ogni campagna avanzata che lo utilizza per semplificare la gestione dei dati, il punteggio lead e i flussi di lavoro di indirizzamento.

## Orchestrazione tra canali {#cross-channel-orchestration}

* **Campi di dati sensibili in Forms**: Le informazioni personali (PII) dei clienti Protect non vengono visualizzate nei moduli Adobe Marketo Engage definendo i campi di dati come sensibili e limitando la precompilazione dei moduli per tali campi. Ogni volta che un visitatore visualizza un modulo sulla pagina di destinazione, i campi definiti sensibili non presentano dati precompilati.

* **Blocca invio modulo spam**: Protect il tuo database Adobe Marketo Engage da dati spazzatura che possono causare avvisi non validi alle vendite, attivare backlog della campagna e creare attività indesiderate. Il nuovo meccanismo di convalida rifiuta l’invio di moduli non validi e interrompe gli attacchi di bot. I dati sono più puliti e le campagne di marketing vengono eseguite come previsto, riducendo al minimo il rischio di inviare lead non qualificati alle vendite.

* **Avviso di approvazione del programma e-mail**: Impedisci l’invio di e-mail errate quando le nuove modifiche sono state apportate a un programma approvato in precedenza.  L’avviso funge da guardrail quando un addetto al marketing applica modifiche a un’e-mail già approvata, ma poi dimentica di approvare le modifiche più recenti e invia l’e-mail a un pubblico di grandi dimensioni senza contenuto, contenuto errato o contenuto obsoleto.

* **Attività bot e-mail con filtro**: Impedisci avvisi di vendita non intenzionali e rapporti e-mail inesatti tramite la nuova funzionalità di filtro delle attività bot delle e-mail. Identifica e filtra aperture e clic che possono essere associati a bot di e-mail che ispezionano i collegamenti che portano a falsi attivatori e avvisi di vendita o a rapporti errati.

## Miglioramenti API {#api-enhancements}

Diversi aggiornamenti critici delle API Bulk e Lead, tra cui la possibilità di esportare dati di oggetti personalizzati in blocco, associare l’azienda al lead in blocco, la capacità di filtrare l’estrazione di attività in blocco in base a un attributo principale e la possibilità di creare e aggiornare l’appartenenza al programma.

* **Programmi evento nidificati**: In Adobe Marketo Engage è possibile creare, clonare o spostare programmi evento sotto altri tipi di programmi. Questa funzionalità è ora consentita nell’API delle risorse.

* **API del programma di eliminazione ottimizzata**: Consente alle applicazioni integrate di eliminare i programmi contenenti ulteriori tipi di risorse senza richiedere agli utenti di farlo manualmente da Adobe Marketo Engage.

* **Iscrizione al programma**: Gli addetti al marketing possono eseguire query su tutti i record dei membri del programma per un programma selezionato in base a criteri diversi, ad esempio lo stato dei membri del programma. Condividi queste informazioni con un’applicazione esterna, uno strumento di business intelligence o Adobe Experience Cloud per migliorare la segmentazione e creare un coinvolgimento più mirato.

* **Estrazione oggetti personalizzati in blocco**: L’esportazione di dati in blocco integra le funzionalità di importazione di cui gli analisti di dati stanno già fruendo in Adobe Marketo Engage. Ora è possibile estrarre in massa i dati archiviati nel primo livello Adobe Marketo Engage Custom Objects, caricarli in un&#39;altra applicazione, in un data warehouse o in un altro strumento BI (Business Intelligence) per ottenere migliori informazioni sui dati nell&#39;istanza Adobe Marketo Engage.  Lo spostamento di dati in massa di oggetti personalizzati è bidirezionale e può essere pianificato in un momento conveniente.

* **API metadati campi personalizzati**: Risparmia tempo automatizzando la creazione di campi personalizzati durante la configurazione delle integrazioni Adobe Marketo Engage con un’applicazione di terze parti. Questa automazione è particolarmente utile per i clienti con più istanze di Adobe Marketo Engage che sono ora in grado di semplificare la creazione di campi personalizzati che richiedevano un lavoro manuale in ogni istanza. Semplifica la creazione di campi personalizzati e risparmia tempo su questa attività che richiede risorse.

* **API di estrazione attività in blocco**: Acquisisci il controllo sulla quantità e sul tipo di dati durante l’esecuzione di estrazioni in massa. Filtra punti di dati non necessari e controlla il numero di chiamate API necessarie per estrarre dati di attività in blocco.  Ad esempio, seleziona e-mail aperte, visita una pagina web o modifica il punteggio del lead e lascia indietro altre modifiche del valore che non desideri analizzare. Semplifica il processo per ridurre il numero di chiamate API e di pulizia dei dati.

* **API lead**: Identifica i lead in Adobe Marketo Engage a cui è associato un Adobe ECID (ID Experience Cloud).  I clienti Adobe Marketo Engage possono creare un elenco di lead da una campagna selezionata e utilizzare gli ECID (ID Experience Cloud) per creare rapporti in Adobe Analytics per tale elenco specifico. L&#39;integrazione tra Adobe Marketo Engage e Adobe Experience Cloud offre opportunità illimitate per segmentazione, targeting e reporting.

* **API di importazione in blocco di lead**: Controlla l’importazione in blocco dei lead e le risorse necessarie. Questo miglioramento crea un’associazione tra lead e società durante il processo di importazione in serie di lead. Aumenta l’efficienza e l’utilizzo dei dati e diminuisce l’utilizzo delle chiamate API.

* **Integrazione basata su API web per i clienti Microsoft Dynamics Online**: L’API Web di MS Dynamics è stata introdotta con il protocollo REST versione 8.0 e implementa OData (Open Data Protocol) v4. OData è uno standard OASIS (Organizzazione per la promozione di standard informativi strutturati) per la costruzione e il consumo di servizi RESTful rispetto ai dati ricchi. I clienti Adobe Marketo Engage che richiedono l’integrazione con Microsoft Dynamics utilizzando questo metodo stanno attualmente effettuando la migrazione a una connessione basata su API Web da SOAP (Simple Object Access Protocol).

## Ambiente dati di marketing {#marketing-data-environment}

* **Esportazione XLSX**: Abbiamo aggiornato le funzionalità di esportazione in tutto il prodotto per supportare XLSX al posto di XLS. Ciò significa che in qualsiasi punto del prodotto in cui è attualmente supportata l’esportazione XLS, questa opzione verrà sostituita con un’opzione per l’esportazione in XLSX. Questa modifica influenzerà i nomi dei file per tutte le esportazioni Excel di report e altri dati da Adobe Marketo Engage.

* **Ricerca per ID lead**: Accedi rapidamente alla ricerca di record lead da parte di Adobe Marketo Engage lead ID nel database lead o nell’elenco statico. Nella finestra Ricerca rapida digitare `[id]` con il numero corrispondente, vengono visualizzate le informazioni sul lead. Gli utenti possono esaminare rapidamente i dettagli relativi a lead, aziende o opportunità.

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Integrazione con LinkedIn Lead Gen Forms (Beta)**: Ottieni una visibilità profonda nella spesa e nel ROI del tuo canale LinkedIn con la soluzione di attribuzione Bizible Premium. Grazie all’integrazione più recente con Forms leader di LinkedIn, Bizible offre informazioni approfondite sui moduli inviati all’interno della piattaforma LinkedIn. Queste compilazioni vengono confrontate con i lead provenienti dall’istanza CRM (Customer Relationship Management) o Adobe Marketo Engage in modo che siano idonee all’attribuzione e possano essere monitorate rispetto agli altri engagement di marketing.

## Annunci {#announcements}

* **Piattaforme di sostituzione dei documenti di prodotto Marketo**: Siamo lieti di annunciare che i documenti sui prodotti Marketo sono entrati a far parte di Adobe Experience League venerdì 7 maggio. Sarà comunque possibile utilizzare l’URL: docs.marketo.com e se hai degli articoli esistenti con segnalibro, verrai reindirizzato. Tutti i documenti sui prodotti sono disponibili sulla nuova piattaforma, con miglioramenti pianificati per la fine dell&#39;anno.

* **Amministrazione utente semplificata e single sign-on con tecnologia Adobe Identity System**: A partire da luglio 2021, i nuovi clienti Adobe Marketo Engage saranno caricati utilizzando le credenziali utente Adobe. La migrazione degli attuali clienti al sistema di identità integrato non avverrà prima della metà del 2022 e non sarà necessaria alcuna azione da parte del cliente fino a nuovo avviso. Il single sign-on consente agli amministratori IT/di sicurezza di gestire più istanze di prodotti Adobe Marketo Engage insieme ad altre soluzioni Experience Cloud e di configurare SSO (Shared Services Organization) tramite una console comune. Gli amministratori possono gestire facilmente i gruppi di utenti e le adesioni degli utenti tramite un Admin Console comune.

**_Webinar sulla versione del prodotto_**

[Webinar sul rilascio del Marketo Engage di maggio 2021](https://engage.marketo.com/May_21_Release_webinar_RegistrationPage.html)
