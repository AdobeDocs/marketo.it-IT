---
description: Note sulla versione corrente di Dynamic Chat - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione di Dynamic Chat
feature: Release Information, Dynamic Chat
exl-id: 0447dc47-b9c5-42e1-8f66-73bf67c7871d
source-git-commit: 5dbc3add8acaae02f25c1f9b9ae39ecfc1aaf259
workflow-type: tm+mt
source-wordcount: '3408'
ht-degree: 2%

---

# Note sulla versione di Dynamic Chat {#dynamic-chat-release}

I rilasci di Adobe Dynamic Chat funzionano secondo un modello di distribuzione continua che consente un approccio più scalabile alla distribuzione delle funzioni. A volte ci sono più versioni in un mese, quindi controlla regolarmente per informazioni sempre aggiornate.

La pagina delle note sulla versione standard per Marketo Engage [ si trova qui](/help/marketo/release-notes/current.md){target="_blank"}.

## Versione di giugno 2025 {#june-2025-release}

**Data di rilascio: martedì 30 giugno 2025**

### Rinnovo della logica di routing {#routing-logic-revamp}

Abbiamo rinnovato la logica di indirizzamento della chat in tempo reale in Dynamic Chat per garantire un comportamento di coinvolgimento più intelligente e prevedibile per tutti i tipi di indirizzamento (Account, Personalizzato, Team e Round Robin). La nuova logica semplifica i flussi di routing e migliora la gestione di fallback quando gli agenti non sono disponibili.

#### Miglioramenti chiave nel comportamento di indirizzamento

* **Fino a due tentativi di coinvolgimento per sessione**

   * Il sistema tenterà di connettersi con un massimo di due agenti (al massimo), ma rigorosamente all’interno della regola di routing principale.

   * Se un agente è disponibile ma non risponde (ad esempio, rifiuta o salta la chat), il sistema tenterà di connettersi a un altro agente dello stesso pool.

   * La logica di fallback (come Round Robin) viene attivata solo se non vengono trovati agenti idonei durante la risoluzione iniziale, per non riprovare dopo un coinvolgimento fallito.

* **Comportamento Specifico Della Regola Di Indirizzamento**

##### —Indirizzamento account—

Se il dominio e-mail di un visitatore è mappato su un account noto, l’agente mappato ha sempre la priorità.

Se l’agente è disponibile, la chat viene indirizzata direttamente a loro.

Se l&#39;agente non è disponibile, il sistema:

* Non tenta un altro agente, anche se Round Robin è abilitato come fallback.

* Invece:

   * Mostra il calendario della riunione dell&#39;agente mappato (se attivato).
-oppure-
   * Torna a un messaggio predefinito (caso peggiore).

La regola di routing a livello di scheda (ad esempio Team, Personalizzato) viene considerata solo se l’Instradamento account non è idoneo (nessun dominio o agente corrispondente).

##### —Instradamento personalizzato/team—

Queste regole possono restituire più agenti idonei.

Se il primo agente disponibile non si attiva, il sistema tenterà un altro agente dallo stesso elenco.

Il fallback Round Robin non viene attivato solo perché un agente non risponde.

Se nessuno dei due agenti si impegna:

* Il sistema visualizza il calendario del primo agente provato (se attivato).
-oppure-
* Visualizza il messaggio di fallback predefinito.

##### —Stesura arrotondata robin—

Quando viene utilizzato come regola di instradamento principale, il sistema:

* Tenta di coinvolgere il primo agente disponibile dal pool round robin.

* Se il primo agente non risponde, tenta di nuovo con il migliore agente idoneo successivo.

Se Round Robin viene utilizzato come fallback, si attiva solo se non vengono risolti agenti dalla regola primaria.

##### Flusso di esperienza dei visitatori

Il sistema controlla se è applicabile l&#39;Instradamento conto.

* Se sì e l’agente è disponibile, si connette immediatamente.

* Se l&#39;agente non è idoneo o non disponibile, passa alla regola di routing a livello di scheda.

Viene valutata la regola di routing a livello di scheda (Personalizzato, Team, Round Robin).

* Gli agenti idonei vengono verificati per la disponibilità (autorizzazioni, stato).

* Il sistema coinvolge un agente e, se necessario, tenta un secondo agente dalla stessa regola.

* Se il coinvolgimento non ha esito positivo, viene applicata la logica di fallback:

   * Fallback del calendario (se attivato),
-oppure-
   * Messaggio predefinito.

Il fallback Round Robin viene considerato solo quando non vengono trovati agenti idonei dalla regola di routing principale, non quando i singoli agenti non rispondono.

##### Casi d’uso

<p>

_&#x200B;**Indirizzamento account**&#x200B;_

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Esempio</th>
    <th>Risultato</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideale</td>
    <td>Il dominio del visitatore è associato a un account; l’agente mappato ha una chat in tempo reale abilitata ed è disponibile</td>
    <td>La chat si connette direttamente all’agente mappato</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>L’agente mappato non è disponibile. Il fallback Round Robin è abilitato</td>
    <td>Il sistema seleziona un agente disponibile tramite Round Robin e li coinvolge </td>
  </tr>
  <tr>
    <td>Nessun agente di fallback</td>
    <td>L’agente mappato non è disponibile, nessun fallback Round Robin; la prenotazione della riunione è abilitata</td>
    <td>Il sistema mostra il calendario dell'agente mappato o visualizza un messaggio di fallback predefinito</td>
  </tr>
</tbody></table>

_&#x200B;**Routing personalizzato**&#x200B;_

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Esempio</th>
    <th>Risultato</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideale</td>
    <td>La logica personalizzata risolve un elenco di agenti; il primo agente è disponibile e accetta la chat.</td>
    <td>La chat si connette al primo agente.</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>La regola personalizzata non risolve alcun agente; il fallback Round Robin è abilitato.</td>
    <td>Il sistema seleziona un agente disponibile tramite Round Robin e li coinvolge.</td>
  </tr>
  <tr>
    <td>Nessun agente di fallback</td>
    <td>Due agenti sono stati risolti; nessuno dei due accetta la chat e il fallback è impostato sul calendario della riunione.</td>
    <td>Viene visualizzato il calendario dell'agente provato per primo oppure il messaggio di fallback predefinito.</td>
  </tr>
</tbody></table>

_&#x200B;**Indirizzamento team**&#x200B;_

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Esempio</th>
    <th>Risultato</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideale</td>
    <td>Il team include agenti con chat in tempo reale; il primo agente disponibile accetta la chat.</td>
    <td>La chat si connette a tale agente.</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>Nessun agente team disponibile e il fallback Round Robin è abilitato.</td>
    <td>Il sistema seleziona e si connette con un agente del pool Round Robin.</td>
  </tr>
  <tr>
    <td>Nessun agente di fallback</td>
    <td>Due agenti disponibili, ma nessuno dei due è coinvolto; il fallback del calendario è abilitato.</td>
    <td>Viene visualizzato il calendario del primo agente provato oppure viene attivato il messaggio di fallback.</td>
  </tr>
</tbody></table>

_&#x200B;**Routing Robin Round**&#x200B;_

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Esempio</th>
    <th>Risultato</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideale</td>
    <td>Round Robin pool ha più agenti; secondo agente accetta chat dopo primo non lo fa.</td>
    <td>La chat si connette al secondo agente.</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>Nessun agente disponibile nel pool Round Robin. Il calendario della riunione è abilitato.</td>
    <td>Il calendario viene visualizzato per il primo agente nell’elenco (se configurato), oppure viene visualizzato il messaggio di fallback.</td>
  </tr>
  <tr>
    <td>Nessun agente di fallback</td>
    <td>Nessun agente disponibile; il fallback è disabilitato.</td>
    <td>Al visitatore viene mostrato un messaggio di fallback statico.</td>
  </tr>
</tbody></table>

### Notifica Pulse {#pulse-notification}

Ogni volta che un visitatore richiede di connettersi con un agente, forniamo all’agente una notifica in-app tramite browser. Ma a volte, gli agenti perdono queste chat.

Con questa versione, l’agente live può ricevere una notifica e-mail, Slack, in-app e browser quando un nuovo visitatore è interessato alla chat.

1. Nella home page di Adobe Experience Cloud, fai clic sull&#39;icona Account e seleziona **Preferenze**.

   ![](assets/dynamic-chat-june-2025-release-1.png)

1. Scorri verso il basso fino a _Notifiche_ e seleziona il Dynamic Chat desiderato.

   ![](assets/dynamic-chat-june-2025-release-2.png)

>[!NOTE]
>
>Il contenuto di una notifica Pulse può essere lo stesso utilizzato per le notifiche in-app del browser.

## Versione di aprile/maggio 2025 {#apr-may-25-release}

### Suono notifica messaggio {#message-notification-sound}

Ora puoi abilitare un suono per il visitatore ogni volta che il chatbot viene attivato in una sessione. È possibile scegliere tra più suoni.

### Abilita messaggi Poke su dispositivi mobili {#enable-poke-messages-on-mobile}

&quot;Poke&quot;, che mostra la domanda di apertura accanto all’icona della chat senza che il visitatore debba fare clic su di essa per visualizzarla, è ora un’opzione da abilitare per i visitatori che utilizzano un dispositivo mobile.

### Aggiornamento di fallback predefinito {#default-fallback-update}

Per qualsiasi regola/team personalizzato come scheda di chat in diretta, se non sono disponibili agenti (o la chat non può connettersi), verrà eseguito il fallback su Round Robin per gli agenti disponibili (tutti coloro che sono disponibili in quel momento, indipendentemente dalla logica/regola di routing inserita nel flusso).

### Integrazione Demandbase {#demandbase-integration}

Gli utenti Demandbase possono utilizzare gli attributi persona Demandbase per il targeting delle finestre di dialogo, il branding condizionale e il routing personalizzato in Dynamic Chat.

## Versione di settembre/ottobre 2024 {#sep-oct-release}

### Analisi avanzata delle chat in tempo reale {#enhanced-live-chat-analytics}

Sono stati apportati diversi miglioramenti alla dashboard di Analytics, tra cui:

* Numero totale di chat in diretta richieste: numero di visitatori richiesti per una &quot;chat con agente&quot;

* Totale chat in diretta connessa: numero di visitatori connessi rispetto al totale richiesto per una &quot;chat con agente&quot;

* Totale richieste di chat in diretta non effettuate: numero di visitatori non assistiti rispetto al totale richiesto per una &quot;chat con agente&quot;

* Lunghezza media chat in minuti: analizza la &quot;lunghezza media della chat&quot; tra i visitatori e i tuoi agenti

* Tempo medio di risposta agente in secondi: analizza il &quot;tempo medio impiegato&quot; dagli agenti per rispondere alle domande e risposte live chat

* Dashboard giornaliera: richieste chat in diretta connesse correttamente, richieste chat in diretta non soddisfatte, ordina e filtra le attività chat in diretta recenti

![](assets/dynamic-chat-sep-oct-2024-release-1.png)

### Punteggio conversazione {#conversation-scoring}

Quantifica i lead in base alla qualità della loro interazione con la chat e utilizza tale metrica come attivatore/filtro in Marketo Engage Smart Campaigns. Utilizza il nuovo attributo _punteggio conversazione_ per le seguenti attività:

* Coinvolto con una finestra di dialogo
* Coinvolto in un flusso di conversazione
* Coinvolto con un agente

**Aspetti da considerare:**

* Il valore del punteggio sarà compreso tra 0, 1, 2, 3 (il valore predefinito è null)

* Quando la conversazione viene completata o eliminata, il valore del punteggio non può essere modificato

* Impostazione punteggio:

   * Nella casella in entrata dell’agente: durante una chat live, l’agente è in grado di aggiornare o impostare un punteggio per la conversazione, che viene memorizzato nell’attività di conversazione

   * Nella finestra di progettazione del flusso, nella scheda dell’obiettivo l’utente è in grado di aggiornare o impostare un punteggio per la conversazione

![](assets/dynamic-chat-sep-oct-2024-release-2.png)

![](assets/dynamic-chat-sep-oct-2024-release-3.png)

![](assets/dynamic-chat-sep-oct-2024-release-4.png)

### Nuova logica di creazione del lead {#new-lead-creation-logic}

Se un lead compila un modulo con l&#39;e-mail `abc@test.com` e viene cookie come xyz, quindi compila lo stesso modulo con l&#39;e-mail `def@test.com`, viene creato un nuovo record persona, ma il cookie xyz viene associato alla nuova persona e rimosso dalla persona `abc@test.com`.

Pertanto, quando un visitatore con cookie abc arriva a una pagina e fornisce un ID e-mail come `abc@test.com`:

<table><thead>
  <tr>
    <th>Visitor</th>
    <th>Cookie</th>
    <th>E-mail fornita</th>
    <th>Comportamento previsto</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Anonimo</td>
    <td>abc</td>
    <td>Non esiste nel database</td>
    <td>Crea una nuova persona</td>
  </tr>
  <tr>
    <td>Anonimo</td>
    <td>abc</td>
    <td>Esiste nel database</td>
    <td>Unisci persona</td>
  </tr>
  <tr>
    <td>Anonimo</td>
    <td>xyz</td>
    <td>Esiste nel database</td>
    <td>Unisci persona</td>
  </tr>
  <tr>
    <td>Persona nota</td>
    <td>abc</td>
    <td>Uguale alla persona esistente</td>
    <td>Aggiorna persona</td>
  </tr>
  <tr>
    <td>Persona nota</td>
    <td>abc</td>
    <td>Diverso da persona esistente</td>
    <td>Se esiste già una persona nota, trasferisci il cookie e risolvi tale profilo. Se non esiste alcuna persona con questa e-mail, crea un nuovo record persona e trasferisci il cookie</td>
  </tr>
  <tr>
    <td>Persona nota</td>
    <td>xyz</td>
    <td>Uguale alla persona esistente</td>
    <td>Aggiungi un nuovo cookie alla stessa persona</td>
  </tr>
  <tr>
    <td>Persona nota</td>
    <td>xyz</td>
    <td>Diverso da persona esistente</td>
    <td>questo scenario non è possibile se si tratta di un nuovo cookie di   predefinito considerato come nuovo profilo anonimo</td>
  </tr>
</tbody></table>

### Opzione per ereditare il carattere {#option-to-inherit-font}

Ora puoi abilitare il chatbot per ereditare direttamente il font dalla pagina web in cui è ospitato, anziché gestire il font del brand in Dynamic Chat. Quando abiliti questa opzione, il chatbot assumerà il font definito sul tag `<body>` della pagina.

![](assets/dynamic-chat-sep-oct-2024-release-5.png)

### Integrazione Demandbase con Dynamic Chat {#demandbase-integration-with-dynamic-chat}

Gli utenti di Demandbase sono in grado di portare la propria licenza di Demandbase e attivare l&#39;integrazione. Utilizza gli attributi persona Demandbase per il targeting delle finestre di dialogo, il branding condizionale e il routing personalizzato.

La risoluzione di questi valori di attributo nei confronti di una persona viene eseguita in tempo reale e viene memorizzata nel rispettivo profilo persona.

### Tempo di caricamento del flusso di conversazione ottimizzato {#optimized-conversation-flow-load-time}

Per migliorare l’esperienza utente, ora viene visualizzato un caricatore shimmer invece di uno spazio vuoto durante il caricamento del flusso conversazionale.

**Prima**

![](assets/dynamic-chat-sep-oct-2024-release-6.png)

**Dopo**

![](assets/dynamic-chat-sep-oct-2024-release-7.gif)

## Versione di agosto 2024 {#august-release}

**Data di rilascio: sabato 23 agosto 2024**

### Personalizzare la formattazione dei messaggi di conversazione {#custom-format-conversation-messages}

Le finestre di progettazione di flussi ora supportano [l&#39;inserimento di HTML](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#create-a-stream){target="_blank"} per personalizzare l&#39;aspetto delle conversazioni.

![](assets/dynamic-chat-aug-2024-release-1.png)

### Chatbot scorri verso il basso {#chatbot-scroll-to-bottom}

Nel chatbot è stata aggiunta un’icona per consentire ai visitatori web di passare direttamente all’ultimo messaggio. In questo modo i visitatori possono scorrere il testo per tornare rapidamente alla conversazione.

![](assets/dynamic-chat-aug-2024-release-2.png)

### Notifiche Core Pulse {#core-pulse-notifications}

Gli utenti ricevono ora una [notifica e-mail](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md#failed-action-notifications){target="_blank"} quando la prenotazione di una riunione o la chat in tempo reale non riesce.

![](assets/dynamic-chat-aug-2024-release-3.png)

### Supporto per più conversazioni {#support-for-multiple-conversations}

Il chatbot ora supporta più conversazioni. I visitatori del sito web possono intrattenere conversazioni diverse su pagine diverse nello stesso momento, con la possibilità di passare da una all’altra.

![](assets/dynamic-chat-aug-2024-release-4.png)

### Ordinamento predefinito per il contenuto {#default-sorting-for-content}

Per impostazione predefinita, i registri di conversazione, le domande senza risposta e le tabelle di generazione delle domande sono ordinati in base alla data di creazione (dal più recente al più recente).

### Risoluzione dei lead in tempo reale {#real-time-lead-resolution}

Durante una conversazione con un lead anonimo e viene fornito un ID e-mail, risolviamo se esiste un record lead noto con tale ID e-mail e utilizziamo tale record per la personalizzazione in tempo reale. Se vengono rilevati più record, questi verranno uniti in tempo reale. Questo comportamento è implementato sia per le finestre di dialogo che per i flussi conversazionali.

### Sincronizzazione dei lead senza cookie da Marketo Engage {#syncing-leads-without-cookies}

In precedenza, quando la sincronizzazione Marketo Engage veniva attivata, Dynamic Chat sincronizzava solo i lead noti con uno o più ID cookie di Marketo Engage. Ora, tutti i lead noti (ID cookie presente o meno) verranno sincronizzati in Dynamic Chat e possono essere utilizzati per la personalizzazione delle conversazioni.

### Trasmettere i dati aggiuntivi del visitatore ai flussi conversazionali {#pass-additional-visitor-data}

Se acquisisci le informazioni del visitatore tramite altri canali, come moduli o accesso, ora puoi passare queste informazioni direttamente a Dynamic Chat.

![](assets/dynamic-chat-aug-2024-release-5.png)

### Dati dedotti aggiornati {#refreshed-inferred-data}

La maggior parte delle conversazioni su un sito web sono con visitatori anonimi. Puoi comunque eseguirne il targeting tramite dati dedotti, che si basano sugli IP dei visitatori. Abbiamo aggiornato il nostro database di IP e dei rispettivi dati dedotti che ora supporta un numero di IP quattro volte superiore.

### Suono aggiunto alla notifica del browser agenti {#sound-added-to-agent-browser-notification}

Quando una chat in tempo reale viene assegnata a un agente, questi riceve una notifica dal browser. Ma a volte non li vedono. È stato aggiunto un [suono di notifica](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md#when-a-live-chat-is-routed-to-an-agent){target="_blank"} per evitare che le notifiche non completate vengano ignorate.

![](assets/dynamic-chat-aug-2024-release-6.png)

### Possibilità di aggiornare il profilo del lead durante la chat in diretta {#update-lead-profile-during-live-chat}

Durante una chat in diretta, gli agenti desiderano acquisire informazioni sul visitatore e aggiornare il rispettivo profilo. È ora disponibile un’opzione per aggiornare i valori degli attributi degli oggetti lead e company.

![](assets/dynamic-chat-aug-2024-release-7.png)

## Versione di giugno 2024 {#june-release}

**Data di rilascio: venerdì 6 giugno 2024**

### Scheda flusso conversazionale {#conversational-flow-card}

Semplifica più passaggi in un flusso all’interno delle finestre di dialogo sfruttando la scheda Flusso conversazionale.

Esempio: se l’obiettivo è quello di promuovere le registrazioni per il webinar tramite più finestre di dialogo, è necessario ricreare lo stesso flusso in tutte le finestre di dialogo che hanno tale obiettivo. Per aggiornare i dettagli, è necessario modificare ogni singola finestra di dialogo una alla volta. Non è più così, grazie alla scheda Conversational Flow.

Oltre a ridefinire l’utilizzo dei flussi in più finestre di dialogo, puoi utilizzare lo stesso flusso di transizione per passare ad altri canali, come moduli e pagine di destinazione.

![](assets/dynamic-chat-june-2024-release-1.png)

### Limiti di utilizzo {#usage-limits}

La pagina Limiti di utilizzo mostra informazioni importanti, ad esempio i dettagli del pacchetto e lo stato del limite di utilizzo.

![](assets/dynamic-chat-june-2024-release-2.png)

## Versione di maggio 2024 {#may-release}

**Data di rilascio: giovedì 15 maggio 2024**

### Libreria di risposte preapprovata {#pre-approved-response-library}

[Crea una libreria approvata dal marketing](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md){target="_blank"} di domande e risposte generate da IA per configurare in pochi minuti una chat generativa basata su IA.

![](assets/dynamic-chat-may-2024-release-1.png)

### Domande senza risposta {#unanswered-questions}

[Utilizza un archivio di domande senza risposta](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/unanswered-questions.md){target="_blank"} di conversazioni precedenti per generare nuove risposte preapprovate mantenendo una libreria di risposte con le informazioni più recenti.

![](assets/dynamic-chat-may-2024-release-2.png)

### Riepiloghi conversazione {#conversation-summaries}

[Offri agli agenti di vendita una sintesi delle conversazioni](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#conversation-summary){target="_blank"} con approfondimenti su argomenti di discussione chiave prima delle riunioni per ridurre i tempi di preparazione e fornire agli agenti di vendita informazioni aggiornate.

![](assets/dynamic-chat-may-2024-release-3.png)

### Scelte rapide per le vendite GenAI {#genai-sales-shortcuts}

[Fornisci agli agenti chat in tempo reale metodi più rapidi](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#shortcuts){target="_blank"} per accedere alle risposte generate dall&#39;intelligenza artificiale, modificare le risposte generate esistenti e cercare contenuti aggiuntivi da inviare agli acquirenti durante la conversazione.

![](assets/dynamic-chat-may-2024-release-4.png)

### Assistente conversazioni {#conversation-assist}

Aiuta gli agenti di vendita a rispondere con precisione durante le conversazioni live utilizzando risposte pre-approvate dal tuo team di marketing.

### Spigoli di conversazione {#conversation-nudges}

Assegna ai visitatori del web un call-to-action per indirizzare le conversazioni verso la conclusione.

<p>

## Versione di aprile 2024 {#april-release}

**Data di rilascio: mercoledì 23 aprile 2024**

### Flussi conversazionali ora disponibili per tutti gli utenti {#conversational-flows-available-to-all-users}

Rendi i tuoi moduli e le tue pagine di destinazione più conversazionali e riduci il funnel di vendita consentendo ai lead qualificati di prenotare una riunione o una chat con Sales subito dopo l&#39;invio di un modulo con Conversational Forms, ora completamente disponibile&#42; per tutti gli utenti Dynamic Chat.

_&#42;Precedentemente disponibile come funzionalità di prova con 100 contratti a vita. Gli impegni di flusso conversazionale ora verranno conteggiati per il limite mensile di 250 conversazioni impegnate per gli utenti nel pacchetto Select._

### Funzioni di callback {#callback-functions}

Le [funzioni di callback](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/callback-functions.md){target="_blank"} ti consentono di raccogliere eventi di analisi Dynamic Chat in sistemi esterni, come Adobe Analytics o Google Analytics, in quanto i visitatori sono coinvolti in conversazioni Dynamic Chat. Per abilitare gli eventi di analisi Dynamic Chat, registra un callback con l’API per l’ascolto degli eventi. Questo ti consente di avere una visione più olistica del tuo coinvolgimento con Dynamic Chat in relazione ad altri dati chiave, come il traffico web.

### Sono state aggiunte condizioni di disponibilità dell’agente live al ramo condizionale {#live-agent-availability-conditional-branching}

Oltre ai campi Marketo Engage nativi e personalizzati, ora puoi utilizzare la diramazione condizionale per creare rami in base alla disponibilità dell’agente. Questo è utile se desideri offrire ai visitatori solo l’opzione di parlare con un agente live quando sono disponibili agenti live.

![](assets/dynamic-chat-release-1.png)

### Condizione elenco smart aggiunta alla diramazione condizionale {#smart-list-condition}

Con l’aggiunta della nuova condizione Elenco avanzato di Marketo Engage nell’diramazione condizionale, puoi creare diramazioni in base a tipi di pubblico preesistenti già creati in Marketo Engage, anziché definire le condizioni di diramazione del pubblico in Dynamic Chat.

![](assets/dynamic-chat-release-2.png)

### Diramazione condizionale per flussi conversazionali {#conditional-branching-for-conversational-flows}

All’inizio di quest’anno è stata rilasciata la diramazione condizionale per i dialoghi e ora puoi sfruttare questa possibilità anche nei flussi conversazionali. La diramazione condizionale consente di creare diramazioni nel flusso in base a condizioni diverse.

### Chat live per flussi conversazionali {#live-chat-for-conversational-flows}

Abbiamo rilasciato la funzionalità di chat in diretta per Dialoghi nel 2023 e ora puoi aggiungere impegni di chat in diretta anche ai flussi conversazionali. Se utilizzi i flussi di conversazione con i moduli Marketo Engage, ora puoi consentire ai visitatori qualificati di chattare con un agente live immediatamente dopo l’invio del modulo.

### Attività Marketo Engage recenti nella casella in entrata dell’agente {#recent-marketo-engage-activities-in-agent-inbox}

Abbiamo aggiunto le recenti attività di Marketo Engage alla sezione Attività recenti della Casella in entrata dell’agente, in modo che, quando un visitatore del sito richiede di chattare con un agente, l’agente possa vedere rapidamente se il visitatore è stato recentemente coinvolto in una delle seguenti attività di Marketo Engage (ultime 25 attività):

* E-mail aperta
* Pagina web visitata
* Modulo compilato
* Momento interessante

![](assets/dynamic-chat-release-3.png)

### Stato della connessione al calendario in Gestione agenti {#calendar-connection-status-in-agent-management}

Gli amministratori possono ora vedere facilmente quali agenti con autorizzazioni per la prenotazione di riunioni hanno connesso i loro calendari in Dynamic Chat. In questo modo, potete assicurarvi che l&#39;intero team di vendita sia connesso e pronto ad accettare le convocazioni di riunione da Dynamic Chat.

![](assets/dynamic-chat-release-4.png)

### Impostazione avviso minimo nella configurazione del calendario dell&#39;agente {#minimum-notice-setting-in-agent-calendar-configuration}

Gli utenti hanno segnalato che i visitatori web prenotavano le riunioni sul calendario con appena 10 minuti di preavviso, per questo abbiamo introdotto un’impostazione di preavviso minimo nella configurazione del calendario dell’agente e impostato il lead time predefinito su 24 ore.

![](assets/dynamic-chat-release-5.png)

### Comportamento dell&#39;utente aggiunto/rimosso aggiornato {#add-remove-user-behavior-updated}

Alcuni utenti hanno segnalato problemi durante l’aggiunta e la rimozione di agenti in Dynamic Chat, per cui abbiamo apportato alcune modifiche per risolvere questi problemi.

Quando un utente viene aggiunto ad Admin Console con l’autorizzazione alla prenotazione di chat in diretta o riunioni, viene immediatamente visualizzato nell’elenco Gestione agenti e può essere aggiunto a Finestre di dialogo, Flussi conversazionali, regole di routing e team.

Quando un utente con autorizzazioni per la prenotazione di riunioni o la chat in tempo reale viene rimosso da Admin Console, verrà immediatamente rimosso da Dynamic Chat, non sarà più disponibile per la chat in tempo reale o l’instradamento di riunioni e non verrà più conteggiato nei limiti di licenza.

### Migliori prestazioni del rapporto a livello di conversazione {#improved-conversation-level-report-performance}

I rapporti a livello di dialogo individuale e di flusso conversazionale ora sono più performanti e precisi. In precedenza, il caricamento dei rapporti delle finestre di dialogo poteva richiedere diversi secondi e talvolta i dati non erano coerenti con i rapporti sulle prestazioni globali. Ora i singoli rapporti della finestra di dialogo vengono caricati in un istante e i dati saranno sempre allineati con i dati di reporting globali.

![](assets/dynamic-chat-release-6.png)

### Aggiornamenti delle autorizzazioni {#permission-updates}

Abbiamo ripulito la struttura delle autorizzazioni e la denominazione in Adobe Admin Console per rendere la gestione delle autorizzazioni più intuitiva.

* La categoria &quot;Gestione conversazioni&quot; è ora denominata &quot;Conversazioni&quot;
* La categoria &quot;Riunioni&quot; è ora denominata &quot;Attività&quot;
* La categoria &quot;Impostazioni agente&quot; è ora denominata &quot;Agenti&quot;
* La categoria &quot;Impostazioni amministratore&quot; è ora denominata &quot;Configurazione&quot;
* La categoria &quot;Chat in tempo reale&quot; è stata rimossa e tutte le autorizzazioni di chat in tempo reale sono state spostate nella categoria Agenti

![](assets/dynamic-chat-release-7.png)

### Supporto per i collegamenti ipertestuali nella casella in entrata dell’agente {#support-for-hyperlinks-in-agent-inbox}

Ora, quando gli agenti di chat live condividono gli URL con i visitatori nella chat, questi saranno collegati ipertestualmente in modo che i visitatori possano semplicemente fare clic su di essi per passare alla pagina, anziché dover copiare e incollare l’URL nel browser.

### Immettete il comportamento chiave aggiornato nella casella in entrata dell&#39;agente {#enter-key-behavior-updated-in-agent-inbox}

È stato cambiato il comportamento del tasto di ritorno nella casella in entrata dell’agente, quindi premendo il tasto Invio o Indietro verrà inviato il messaggio e premendo Maiusc+Invio verrà creata un’interruzione di riga.

![](assets/dynamic-chat-release-8.png)

### Pagina Round robin rimossa {#round-robin-page-removed}

Non si preoccupi! Round robin routing è ancora completamente funzionale e funziona come sempre. Abbiamo appena rimosso la pagina che mostrava un elenco spesso impreciso di agenti e il loro ordine nella coda di routing round robin.

Quando abbiamo rilasciato Dynamic Chat nel 2022, non c’era supporto per la chat in diretta, ma solo per la prenotazione di riunioni, e la pagina di indirizzamento round robin è stata progettata pensando solo alla prenotazione di riunioni. Con l&#39;introduzione della chat dal vivo lo scorso anno, la pagina round robin è diventata obsoleta in quanto non rifletteva con precisione la natura più complessa del round robin routing tra agenti con sia la prenotazione delle riunioni che le autorizzazioni di chat dal vivo. Abbiamo esplorato alcune opzioni diverse per risolvere questo problema, ma alla fine abbiamo deciso che rimuoverlo del tutto era l’opzione migliore per ridurre al minimo la confusione.

![](assets/dynamic-chat-release-9.png)

## Versione di febbraio 2024 {#february-release}

**Data di rilascio: venerdì 22 febbraio 2024**

### Pagina Conversazioni {#conversations-page}

La nuova pagina Conversazioni offre un punto di riferimento unico per la visualizzazione delle trascrizioni di tutte le conversazioni (automatizzate e live) avvenute per l’istanza, da lead noti e anonimi, fornendo una migliore visibilità sul modo in cui i clienti interagiscono con dialoghi, flussi conversazionali e agenti live.

![](assets/dynamic-chat-release-10.png)

### L’intervallo di date nel dashboard globale è aumentato da 90 giorni a 24 mesi {#date-range-in-global-dashboard}

Hai chiesto e abbiamo consegnato. Ora è possibile visualizzare i dati sul coinvolgimento di Dynamic Chat per un massimo di due anni in tutte le dashboard di analisi.

### Diramazione condizionale nelle finestre di dialogo {#conditional-branching-in-dialogues}

La diramazione condizionale consente di creare rami nei flussi della finestra di dialogo in base a condizioni diverse. Ora è possibile presentare contenuti diversi a persone diverse nella stessa finestra di dialogo in base agli attributi del lead e dell’azienda in Marketo Engage.

## Versione di gennaio 2024 {#january-release}

**Data di rilascio: giovedì 24 gennaio 2024**

### Limite simultaneo di chat live nella gestione degli agenti {#Concurrent-live-chat-limit-setting}

Per impostazione predefinita, ogni agente di chat live nella tua istanza può partecipare a un massimo di 5 sessioni di chat live alla volta. Abbiamo introdotto una nuova impostazione nella gestione degli agenti che consente di regolare questo limite da 1 a 10.

![](assets/dynamic-chat-release-11.png)
