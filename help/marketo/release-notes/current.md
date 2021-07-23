---
description: Note sulla versione corrente - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione corrente
source-git-commit: c98e265e0a4548821ffb291b4f4918f3c49f458d
workflow-type: tm+mt
source-wordcount: '1067'
ht-degree: 0%

---

# Note sulla versione: Agosto 2021 {#release-notes-aug-21}

Le seguenti funzionalità sono incluse nella versione del 21 agosto. Per informazioni sulla disponibilità delle funzioni, consultare la versione Marketo Engage.

>[!AVAILABILITY]
>
>Le caratteristiche indicate da una stella (![](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il tuo rappresentante del Marketo Engage Adobe.

**_Versioni trimestrali_**

Le seguenti funzionalità saranno rilasciate il **20 agosto 2021**.

## Integrazione Adobe Experience Platform {#adobe-experience-platform-integration}

* **Connettore Adobe Experience Platform nativo per la condivisione di tipi di pubblico su Marketo Engage**: Abilita l’orchestrazione di campagne multicanale nel Marketo Engage per i segmenti di pubblico creati in Adobe Experience Cloud tramite connettore di destinazione nativo. Il connettore utilizza indirizzi e-mail per far corrispondere i profili Adobe Experience Platform ai profili lead del Marketo Engage, consentendo una condivisione dei segmenti altamente accurata tra le applicazioni. Gli elenchi di Marketi Engage statici vengono creati automaticamente e consentono agli addetti al marketing di raggiungere il pubblico target con messaggi altamente personalizzati o di avviare flussi di lavoro. Attiva i tipi di pubblico sfruttando il proprio contesto di account e opportunità e dati più completi e in tempo reale, ad Experience Platform.

* **Autenticazione utente Marketo Engage tramite Adobe Identity**: A partire da settembre 2021, i nuovi utenti del Marketo Engage con pacchetti Enterprise verranno caricati utilizzando le credenziali utente Adobe ID. La migrazione degli attuali utenti al sistema di identità integrato non avverrà prima della metà del 2022 e non sarà necessaria alcuna azione fino a nuovo avviso. L’autenticazione utente di Adobe Identity consente agli amministratori IT/Security di gestire più istanze di prodotti di Marketo Engage insieme ad altre soluzioni di Experience Cloud, nonché di configurare SSO tramite una console comune. Gli amministratori possono gestire facilmente i gruppi di utenti e le adesioni degli utenti in un’unica posizione.

## Automazione delle esperienze {#experience-automation}

* **Nidificazione** campagna eseguibile: Le campagne eseguibili possono ora chiamare anche altre campagne eseguibili che consentono di nidificarle fino a tre livelli di profondità. Ciò consente un ulteriore consolidamento dei flussi operativi comuni e migliora la gestione di Smart Campaign.

* **Pagina** singola azione di flusso in dettagli persona: Esegui azioni di flusso come l’invio di e-mail, la modifica del proprietario della persona o qualsiasi altra azione di campagna intelligente su singoli utenti dalla pagina dei dettagli della persona utilizzando il menu delle azioni di flusso senza passare alla visualizzazione della griglia del database.

* **Esportazione** attività personalizzate: L’esportazione dei metadati supporta ora tutti gli oggetti e i rispettivi metadati che possono essere utilizzati per condividere, analizzare e progettare il modello di dati di abbonamento.

## Miglioramenti API {#api-enhancements}

* **API** metadati campi personalizzati: Creazione e gestione semplificata dei campi personalizzati nel Marketo Engage per le integrazioni dei partner. Crea automaticamente nuovi campi su un oggetto lead e apporta aggiornamenti ai campi in più istanze di Marketi Engage immediatamente e simultaneamente.

* **Filtro** avanzato: Diverse API ora supportano più filtri, ad esempio l’aggiunta di un filtro per l’intervallo di date alle risorse e ai campi dei membri del programma per e-mail. Ora puoi estrarre solo i dati che sono stati aggiornati in un determinato intervallo di tempo per le seguenti API..
   * Ottieni membri programma
   * Ottieni e-mail
   * Estrazione attività in blocco

* **API** per l’invio di moduli: Quando un indirizzo e-mail viene duplicato in due o più record Lead, aggiorniamo l’ultimo record &quot;aggiornato&quot; invece di saltare del tutto. È simile all’API Forms 2.0.

* **API** e-mail: Recupera risorse e-mail campione o sfida.

**_Rilascio in tutto il trimestre_**

Le seguenti caratteristiche sono su un ciclo non trimestrale e saranno rilasciate durante i prossimi mesi.

## Approfondimenti vendite {#sales-insight}

![(stella)](assets/yellow-star.png)

* **Maggiore visibilità nelle attività Lead, Contatto, Account e Opportunità per gli utenti** CRM Salesforce: Il coinvolgimento con i potenziali clienti durante i lunghi cicli di vendita è più informato a causa di un maggior numero di record di coinvolgimento in Sales Insight. Le schede Momenti interessanti, attività web, e-mail e punteggio mostrano fino a 400 attività tra gli oggetti Lead, Contatto, Account e Opportunità.

## Sales Connect {#sales-connect}

![(stella)](assets/yellow-star.png)

* **Limitazione connessione e-mail (GA)**: Migliora il recapito dei messaggi e-mail e ridimensiona le comunicazioni di vendita personalizzate con la limitazione della connessione e-mail per Sales Connect. Questa nuova tecnologia gestisce automaticamente i tempi di invio delle e-mail per creare esperienze senza soluzione di continuità per gli utenti di Exchange e Gmail. Diminuisci o elimina l’utilizzo di applicazioni di invio in blocco di e-mail di terze parti e invia con sicurezza tutte le tue e-mail da Sales Connect.

* **Approfondimenti** attività di vendita migliorati: Acquisisci e attiva un coinvolgimento personalizzato in base alle attività precedenti del tuo team di vendita. È possibile utilizzare nuovi attributi quali il collegamento di registrazione delle chiamate di vendita, il nome della campagna di vendita e l’oggetto dell’e-mail di vendita negli elenchi smart del Marketo Engage.  Queste attività possono essere esportate e segnalate tramite l’API REST di Marketo Engage o l’esportazione in blocco e sono disponibili su filtri e trigger come vincoli aggiuntivi per gli elenchi avanzati.

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Integrazione** Bizible LinkedIn Lead Gen Forms: Gli addetti al marketing possono ora eseguire l’attribuzione dei ricavi sulle conversioni che si verificano quando LinkedIn acquisisce i moduli compilati tramite le unità pubblicitarie Forms lead Gen. Queste informazioni possono quindi essere utilizzate per ottimizzare le prestazioni del modulo e gli investimenti sui mezzi a pagamento. linkedIn Lead Gen Forms è una delle offerte a pagamento di LinkedIn in più rapida crescita e questa nuova funzionalità è inclusa nell’integrazione di LinkedIn Ads con Bizible. 
 
* **Dashboard** Velocity migliorato: Abbiamo aggiunto una nuova metrica di velocità e un filtro del dashboard per approfondimenti più approfonditi. Questo dashboard viene utilizzato dagli esperti di marketing per comprendere la velocità di lead e opportunità, in base allo stadio, e l’efficienza delle diverse forme di coinvolgimento nel marketing e nelle vendite.

* **Nuovo dashboard** del Percorso Cascata coorte: Questo consente agli esperti di marketing di visualizzare la progressione di una coorte selezionata attraverso un set classico di fasi &quot;cascata della domanda&quot;, fornendo una rapida comprensione dei tassi di conversione e della causalità della conversione implicita per fase su base graduale.

## Integrazione Bizible con Adobe Experience Cloud {#bizible-integration-with-adobe-experience-cloud}

Questa sezione include nuove funzioni per gli utenti Bizible che hanno completato la migrazione a Adobe Identity Management System (IMS). Se hai eseguito la migrazione, visualizzerai il tuo nuovo Adobe ID in Impostazioni Bizible nella scheda Adobe ID . La migrazione di tutti gli account è prevista per la fine del 2021.

* **Integrazione Bizible con Adobe Privacy Service**  (disponibile a settembre 2021): L’integrazione di Bizible con Adobe Privacy Service centralizza la conformità alle normative fondamentali sulla privacy dei dati (come il RGPD) nelle applicazioni Adobe Experience Cloud. Ora puoi sfruttare questo servizio e gestire centralmente tutte le richieste di privacy in modo che le richieste di modifica provenienti da Bizible e da altri prodotti Adobe si riflettano tra le applicazioni.

* **Bizible su Adobe Unified Shell**: L’adozione di Adobe Unified Shell da parte di Bizible offre agli utenti nuove funzionalità che verranno visualizzate nella barra di intestazione dell’applicazione Bizible e includono un migliore accesso alle risorse di supporto e al passaggio alle applicazioni. La shell unificata di Adobe consente di creare un’esperienza coerente tra Bizible e altre applicazioni Adobe Experience Cloud.

* **Proprietà e gestione** del dominio Bizible: Gli utenti Bizible possono utilizzare Adobe Admin Console per gestire i domini che desiderano che Bizible tenga traccia. Questo consente di eseguire il self-service in un processo manuale precedente e fornisce un’esperienza coerente nella gestione della proprietà e del tracciamento dei domini nelle applicazioni Adobe Experience Cloud.

## Annunci {#announcements}

* **Aggiornamento delle impostazioni** ID universale della sottoscrizione: Per supportare la prossima integrazione di Marketo Engage e identità Adobe per gli utenti esistenti, tutte le sottoscrizioni di Marketo Engage saranno unificate nell’abilitazione del supporto di Universal ID.
