---
description: Note sulla versione corrente di Dynamic Chat - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione di Dynamic Chat
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
source-git-commit: 342d52439a21668a3bf94e5149710b20e4ddb83f
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 3%

---

# Note sulla versione del Dynamic Chat TEMP {#dynamic-chat-release}

## Versione di settembre/ottobre 2024 {#august-release}

### Analisi avanzata della chat in diretta {#enhanced-live-chat-analytics}

Sono stati apportati diversi miglioramenti alla dashboard di Analytics, tra cui:

* Numero totale di chat in diretta richieste: numero di visitatori richiesti per una &quot;chat con agente&quot;

* Totale chat in diretta connessa: numero di visitatori connessi rispetto al totale richiesto per una &quot;Chat con agente&quot;

* Totale richieste di chat in diretta non effettuate: numero di visitatori non assistiti rispetto al totale richiesto per una &quot;chat con agente&quot;

* Lunghezza media chat in minuti: analizza la &quot;lunghezza media della chat&quot; tra i visitatori e i tuoi agenti

* Tempo medio di risposta dell&#39;agente in secondi: analizza il &quot;tempo medio impiegato&quot; dagli agenti per rispondere alle domande e risposte live chat

* Dashboard giornaliera: richieste chat in diretta connesse correttamente, richieste chat in diretta non soddisfatte, ordina e filtra le attività chat in diretta recenti

SCHERMATA

### Punteggio conversazione

Quantifica i lead in base alla qualità della loro interazione con la chat e utilizza tale metrica come attivatore/filtro nelle campagne intelligenti di Marketo Engage. Utilizza il nuovo attributo _punteggio conversazione_ per le seguenti attività:

* Coinvolto con una finestra di dialogo
* Coinvolto in un flusso di conversazione
* Coinvolto con un agente

**Aspetti da considerare:**

* Il valore del punteggio sarà compreso tra 0, 1, 2, 3 (il valore predefinito è null)

* Una volta completata o eliminata la conversazione, nell’attività salva il valore di punteggio e pubblica che non può essere modificato???????????????????????????????? (cosa significa)

* Impostazione punteggio:

   * Nella casella in entrata dell’agente: durante una chat live, l’agente è in grado di aggiornare o impostare un punteggio per la conversazione, che viene memorizzato nell’attività di conversazione

   * Nella finestra di progettazione del flusso, nella scheda dell’obiettivo l’utente è in grado di aggiornare o impostare un punteggio per la conversazione

SCHERMATA

SCHERMATA

SCHERMATA

### Nuova logica di creazione lead {#new-lead-creation-logic}

Se un lead compila un modulo con l&#39;e-mail `abc@test.com` e viene cookie come xyz, quindi compila lo stesso modulo con l&#39;e-mail `def@test.com`, viene creato un nuovo lead, ma il cookie xyz viene associato al nuovo lead e rimosso dal lead `abc@test.com`.

Da quel momento, `abc@test.com` sarà un lead senza cookie. ANON LEAD??

Pertanto, quando un visitatore con cookie abc arriva a una pagina e fornisce un ID e-mail come `abc@p.com`:

TABELLA
