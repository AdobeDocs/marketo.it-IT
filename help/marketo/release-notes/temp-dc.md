---
description: Note sulla versione corrente di Dynamic Chat - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione di Dynamic Chat
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
source-git-commit: 7fbfdc6d34d2f1174e921464d64689b0c5687914
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 2%

---

# Note sulla versione del Dynamic Chat TEMP {#dynamic-chat-release}

## Versione di settembre/ottobre 2024 {#august-release}

### Analisi avanzata delle chat in tempo reale {#enhanced-live-chat-analytics}

Sono stati apportati diversi miglioramenti alla dashboard di Analytics, tra cui:

* Numero totale di chat in diretta richieste: numero di visitatori richiesti per una &quot;chat con agente&quot;

* Totale chat in diretta connessa: numero di visitatori connessi rispetto al totale richiesto per una &quot;chat con agente&quot;

* Totale richieste di chat in diretta non effettuate: numero di visitatori non assistiti rispetto al totale richiesto per una &quot;chat con agente&quot;

* Lunghezza media chat in minuti: analizza la &quot;lunghezza media della chat&quot; tra i visitatori e i tuoi agenti

* Tempo medio di risposta agente in secondi: analizza il &quot;tempo medio impiegato&quot; dagli agenti per rispondere alle domande e risposte live chat

* Dashboard giornaliera: richieste chat in diretta connesse correttamente, richieste chat in diretta non soddisfatte, ordina e filtra le attività chat in diretta recenti

SCHERMATA

### Punteggio conversazione {#conversation-scoring}

Quantifica i lead in base alla qualità della loro interazione con la chat e utilizza tale metrica come attivatore/filtro nelle campagne intelligenti di Marketo Engage. Utilizza il nuovo attributo _punteggio conversazione_ per le seguenti attività:

* Coinvolto con una finestra di dialogo
* Coinvolto in un flusso di conversazione
* Coinvolto con un agente

**Aspetti da considerare:**

* Il valore del punteggio sarà compreso tra 0, 1, 2, 3 (il valore predefinito è null)

* Una volta completata o eliminata la conversazione, nell’attività salva il valore di punteggio e pubblica che non può essere modificato????? (cosa significa questa frase)

* Impostazione punteggio:

   * Nella casella in entrata dell’agente: durante una chat live, l’agente è in grado di aggiornare o impostare un punteggio per la conversazione, che viene memorizzato nell’attività di conversazione

   * Nella finestra di progettazione del flusso, nella scheda dell’obiettivo l’utente è in grado di aggiornare o impostare un punteggio per la conversazione

SCHERMATA

SCHERMATA

SCHERMATA

### Nuova logica di creazione del lead {#new-lead-creation-logic}

Se un lead compila un modulo con l&#39;e-mail `abc@test.com` e viene cookie come xyz, quindi compila lo stesso modulo con l&#39;e-mail `def@test.com`, viene creato un nuovo lead, ma il cookie xyz viene associato al nuovo lead e rimosso dal lead `abc@test.com`.

Da quel momento, `abc@test.com` sarà un lead senza cookie. LEAD ANONIMO??

Pertanto, quando un visitatore con cookie abc arriva a una pagina e fornisce un ID e-mail come `abc@p.com`:

TABELLA

### Tempo di caricamento del flusso di conversazione ottimizzato {#optimized-conversation-flow-load-time}

Per migliorare l’esperienza utente, ora viene visualizzato un caricatore shimmer invece di uno spazio vuoto durante il caricamento del flusso di conversazione. CONVERSAZIONE O CONVERSAZIONE???

**Prima**

GIF

**Dopo**

GIF

### Opzione per ereditare il carattere {#option-to-inherit-font}

Ora puoi abilitare il chatbot per ereditare direttamente il font dalla pagina web in cui è ospitato, anziché gestire il font del brand in Dynamic Chat. Quando abiliti questa opzione, il chatbot assumerà il font definito sul tag `<body>` della pagina.

SCHERMATA

### Integrazione Demandbase con Dynamic Chat {#demandbase-integration-with-dynamic-chat}

Gli utenti di Demandbase sono in grado di portare la propria licenza di Demandbase e attivare l&#39;integrazione. Utilizza gli attributi persona Demandbase per il targeting delle finestre di dialogo, il branding condizionale e il routing personalizzato.

La risoluzione di questi valori di attributo rispetto a un lead viene eseguita in tempo reale e viene memorizzata nel rispettivo profilo di lead.
