---
description: Rivedi l’ambito dati di Marketo AI, i controlli di governance e le considerazioni PII in tutti i flussi di lavoro chiave, come l’importazione di lead, il controllo qualità del programma e la normalizzazione dei dati.
title: Scheda informativa di Marketo AI
badge: beta
source-git-commit: 5c127a9b84033f2baa3c6bce727472d4b58f5842
workflow-type: tm+mt
source-wordcount: '1454'
ht-degree: 0%

---

# Scheda informativa di Marketo AI {#data-information}

L’intelligenza artificiale di Marketo è una funzione nativa e dinamica di Adobe Marketo Engage che consente ai team delle operazioni di marketing di automatizzare determinati flussi di lavoro tramite interazione con il linguaggio naturale, tra cui importazione di lead, convalida del programma, normalizzazione dei dati, creazione di programmi, analisi dei lead, analisi e guida del prodotto. Marketo AI funziona all’interno dell’ambiente Marketo Engage esistente di un utente e utilizza l’infrastruttura gestita da Adobe per il ragionamento e l’orchestrazione dell’intelligenza artificiale.

**Ambiente utente:** Marketo AI funziona all&#39;interno di un ambiente Marketo Engage esistente e non introduce un nuovo percorso di condivisione da utente a utente.

**Ambito dati:** Il servizio elabora i dati di marketing B2B standard già presenti nell&#39;ambiente utente, inclusi i record dei lead, i dati del programma e l&#39;attività smart campaign.

**Servizi di intelligenza artificiale:** Marketo AI sfrutta un cablaggio preassemblato di intelligenza artificiale creato da Adobe e utilizza Azure OpenAI GPT-4.1 e Claude su AWS Bedrock per il ragionamento di intelligenza artificiale, con gli strumenti MCP di Marketo che supportano l&#39;esecuzione delle azioni del prodotto.

**Governance:** gli output generati dall&#39;intelligenza artificiale rimangono all&#39;interno dell&#39;ambiente dell&#39;utente e sono soggetti ai controlli di governance, residenza e conservazione esistenti.

**Trasparenza:** gli output generati dall&#39;intelligenza artificiale possono essere esaminati tramite la cronologia di conversazione e audit per supportare la supervisione degli utenti.

## Controlli di accesso e rollout

### Importa lead

**Funzione:** elabora i dati dei lead forniti dall&#39;utente per la mappatura, la normalizzazione, la deduplicazione e l&#39;importazione in Marketo Engage.

### Controllo di qualità del programma

**Funzione:** valuta i programmi Marketo in base alle regole organizzative definite dagli utenti in un file di markdown delle abilità, ad esempio gli standard di denominazione, lo stato di approvazione, la conformità e-mail e la logica di flusso.

### Crea programma da breve

**Funzione:** utilizza prompt in linguaggio naturale per generare strutture di programmi Marketo, incluse campagne avanzate, passaggi di flusso e segnaposto di contenuto, direttamente nell&#39;ambiente dell&#39;utente.

### Agenti chiamabili

**Funzione:** esegue azioni di IA attivate da azioni di flusso all&#39;interno dei passaggi di flusso di Smart Campaign per casi di utilizzo quali convalida, normalizzazione e rilevamento di bot.

### Indagine lead

**Funzione:** fornisce un&#39;analisi conversazionale del motivo per cui una persona è passata o meno a una fase cardine esaminando l&#39;esecuzione delle fasi del flusso e l&#39;appartenenza all&#39;elenco smart.

### Misurazione e analisi

**Funzione:** genera l&#39;analisi delle prestazioni di campagne e programmi, inclusi consigli e approfondimenti sulle cause principali.

### Conoscenza del prodotto

**Funzione:** fornisce best practice e indicazioni pratiche per Marketo attraverso un livello di conoscenza condiviso utilizzato nell&#39;esperienza dell&#39;agente.

## Casi di utilizzo

Oltre a quelli elencati, considera l’utilizzo di IA per Marketo per diagnosticare e risolvere problemi operativi complessi (errori di sincronizzazione CRM, errori del webhook, analisi della causa principale della consegna e-mail, incongruenze dei campi), condurre controlli di audit sul tuo account (recapito e-mail, conformità del centro abbonamenti, revisioni di campagne intelligenti, valutazioni del modello di punteggio) e accelerare la creazione del programma da resoconti e modelli (programmi di eventi, campagne e-mail multilingue, configurazioni del webinar). L’intelligenza artificiale di Marketo è progettata per fornire la classificazione dei lead assistiti dall’intelligenza artificiale e l’arricchimento dei dati su larga scala, l’analisi delle prestazioni con raccomandazioni per il monitoraggio e il debug guidato delle configurazioni tecniche, come gli script Velocity e i modelli di ciclo di vita.

## Disponibilità e stato di rollout

**Idoneità:** l&#39;abilitazione iniziale dell&#39;utente è limitata agli utenti Marketo Engage idonei che hanno accettato il rider Adobe Gen AI.

**Provisioning:** l&#39;accesso viene gestito tramite i controlli di abilitazione del prodotto esistenti e il provisioning dei flag di funzionalità all&#39;interno dell&#39;esperienza Marketo Engage.

**Rollout modello:** La distribuzione procede attraverso Alpha e Private Beta prima di ampliare l&#39;espansione di Public Beta.

**Ambito geografico:** La versione iniziale è destinata agli utenti globali di Marketo Engage, esclusa la Cina continentale.

**Ambito di settore:** L&#39;implementazione corrente non include funzionalità specifiche per il settore verticale per settori altamente regolamentati come l&#39;assistenza sanitaria, i servizi finanziari, la pubblica amministrazione o la difesa.

## Documentazione e supporto

**Documentazione:** la documentazione di Experience League è in espansione come parte della disponibilità generale.

**Modello di supporto:** L&#39;approccio di supporto corrente include l&#39;assunzione di feedback da parte degli utenti, le ore di ufficio e una community Experience League di Marketo AI.

**Monitoraggio dei servizi:** Adobe identifica l&#39;osservabilità, le dashboard di feedback e i meccanismi di valutazione della qualità come componenti importanti della maturità del lancio e del miglioramento continuo.

## Dati ed esclusioni fuori ambito

**Nessun nuovo dato di categoria speciale:** Marketo AI non introduce nuove elaborazioni per dati sanitari, finanziari, di posizione precisa, biometrici o di altre categorie speciali.

**Nessun nuovo percorso di condivisione:** Il servizio non crea un nuovo meccanismo di condivisione dei contenuti utente-utente.

**Output contenuti dall&#39;utente:** gli output generati dall&#39;intelligenza artificiale rimangono all&#39;interno dell&#39;ambiente Marketo Engage esistente dell&#39;utente sotto i controlli di governance esistenti.

**Esclusioni correnti:** Il rollout iniziale esclude la Cina continentale e non fornisce funzionalità specifiche per il settore verticale per i settori altamente regolamentati.

## Utilizzo di Azure OpenAI e Claude su AWS Bedrock

Questa sezione spiega come Azure OpenAI supporta i flussi di lavoro di IA per Marketo. Tutti i diagrammi o le descrizioni del flusso correlati devono essere letti insieme ai controlli qui descritti, incluse le limitazioni sull’ambito dei dati, la supervisione degli utenti e l’addestramento dei modelli.

**Finalità:** Azure OpenAI GPT-4.1 viene utilizzato per il ragionamento conversazionale e l&#39;orchestrazione dei flussi di lavoro basati su agenti.

**Ambito dati:** Gli input sono limitati ai dati di marketing B2B standard già presenti nell&#39;ambiente Marketo Engage dell&#39;utente e necessari per soddisfare il flusso di lavoro richiesto.

**Output di IA:** gli output di IA sono determinati dai prompt utente e dalla configurazione e le funzionalità di IA di Marketo non prendono decisioni autonomamente senza la configurazione utente.

**Formazione:** Adobe non utilizza i dati utente per addestrare o perfezionare i modelli Azure OpenAI per questo servizio.

**Sorveglianza utente:** gli output generati dall&#39;intelligenza artificiale rimangono visualizzabili in Marketo Engage attraverso le funzionalità di cronologia di conversazione e controllo.

## Conservazione e archiviazione dei dati

**Output contenuti dall&#39;utente:** Gli output generati dall&#39;intelligenza artificiale come elenchi di lead puliti, rapporti di controllo qualità, strutture di programma generate e dati normalizzati rimangono all&#39;interno dell&#39;ambiente Marketo Engage dell&#39;utente.

**Allineamento governance:** I dati di output rimangono soggetti ai controlli di governance, residenza e conservazione dei dati esistenti dell&#39;utente in Marketo Engage.

**Nessun nuovo archivio per più utenti:** Il servizio non introduce un percorso separato di condivisione dei dati da utente a utente.

## Percorsi di elaborazione e archiviazione dei dati

In questa sezione vengono riepilogati gli ambienti in cui opera Marketo AI e dove si verifica l’elaborazione. Se il documento include diagrammi regionali o elementi visivi dell’infrastruttura, tali materiali dovrebbero essere intesi come rappresentazioni di alto livello della posizione del servizio e del flusso di elaborazione, anziché come schemi esaustivi della rete.

**Ambiente applicazione:** Marketo AI funziona all&#39;interno dell&#39;ambiente Adobe Marketo Engage esistente dell&#39;utente.

**Elaborazione IA:** Marketo AI utilizza Azure OpenAI GPT-4.1 e Claude su AWS Bedrock per il ragionamento conversazionale e l&#39;orchestrazione delle attività.

**Percorso dati utente:** i dati utente e gli output generati dall&#39;intelligenza artificiale rimangono all&#39;interno dell&#39;ambiente Marketo Engage dell&#39;utente e sono soggetti ai controlli di residenza, governance e conservazione esistenti dell&#39;utente.

**Nessun archivio separato per più utenti:** Il servizio non introduce un livello separato di condivisione dati o archiviazione da utente a utente.

## Ambito dati per tipo di flusso di lavoro

I dati elaborati da Marketo AI sono determinati dal modello di utilizzo dell’utente e dal flusso di lavoro specifico richiamato. Non tutti i flussi di lavoro richiedono l’elaborazione di dati a livello di lead.

### Flussi di lavoro che sfruttano solo i metadati della campagna (nessuna informazione sui lead)

* Creazione di programmi da breve: genera strutture di programmi, campagne intelligenti, passaggi di flusso e segnaposto di contenuti da istruzioni in linguaggio naturale
* Clonazione e traduzione di e-mail: duplica e traduce il contenuto del HTML e-mail, le righe dell’oggetto e la copia di marketing nelle varianti di lingua
* Controllo delle campagne: esamina le configurazioni di campagne intelligenti, le definizioni di attivatori/filtri, la logica di flusso e le convenzioni di denominazione.
* Convalida del controllo qualità del programma: valuta i programmi rispetto alle regole definite dall&#39;utente per la conformità, lo stato di approvazione e la completezza strutturale
* Valutazione dell’architettura di programmi e centri di abbonamento — analizza la logica della campagna e la struttura del programma
* Conoscenza del prodotto e best practice: fornisce a Marketo le risposte alle procedure da un livello di conoscenza condiviso

### Flussi di lavoro che sfruttano i record a livello di lead (campi di contatto B2B standard)

* Analisi e risoluzione dei problemi dei lead: esamina i valori dei campi dei lead individuali forniti dall&#39;utente, la cronologia delle attività e la progressione del ciclo di vita per diagnosticare il motivo per cui un lead ha raggiunto o meno lo stato MQL o è idoneo per una campagna di marketing
* Importazione e normalizzazione dei lead: elabora i dati dei lead forniti dall&#39;utente, inclusi nomi, indirizzi e-mail, numeri di telefono e campi aziendali per la mappatura, la pulizia e la deduplicazione
* Classificazione e arricchimento dei lead: valuta i record dei lead in base a una logica di punteggio o classificazione definita dall’utente (ad esempio, lead validi e spam per l’integrità del database, utenti tipo per scopi di personalizzazione, lead aziendali con lead di e-mail aziendali e clienti potenziali)
* Controlli della qualità dei dati e del recapito messaggi: analizza i dati del coinvolgimento a livello di lead, i pattern di mancato recapito e i record duplicati per identificare i problemi di integrità del database
* Analisi delle prestazioni di Campaign: emergono modelli di coinvolgimento dei lead, dati di conversione e composizione del pubblico per supportare l’analisi delle prestazioni

### Minimizzazione dei dati in base alla progettazione

* In tutti i casi, i dati inviati al modello di IA sono limitati a quanto necessario per soddisfare la specifica richiesta dell’utente all’interno di tale flusso di lavoro
* Marketo AI segue le autorizzazioni Marketo Engage esistenti dell’utente e non fornisce l’accesso a record, campi o programmi oltre a quelli che l’utente dispone dell’autorizzazione per visualizzare tramite l’interfaccia utente del prodotto
* Gli utenti che desiderano limitare l’elaborazione dei dati dei lead possono limitare l’accesso ai flussi di lavoro investigativi dello strumento attraverso i controlli esistenti di autorizzazione e ruolo di Marketo Engage, mantenendo al contempo il pieno accesso alle funzionalità di intelligenza artificiale strutturali e amministrative

### Nessuna esposizione incrementale dei dati

L’intelligenza artificiale funziona come acceleratore sulle autorizzazioni utente esistenti, non come percorso di escalation. Inoltre, un utente che non può visualizzare determinati campi, programmi o partizioni lead nell’interfaccia utente di Marketo Engage non può visualizzare tali dati tramite IA per Marketo. Il servizio non ignora le regole di partizione, le autorizzazioni a livello di campo o le restrizioni dell’area di lavoro.
