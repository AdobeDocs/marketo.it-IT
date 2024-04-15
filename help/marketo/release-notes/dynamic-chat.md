---
description: Note sulla versione del Dynamic Chat - Documentazione di Marketo - Documentazione del prodotto
title: Note sulla versione del Dynamic Chat
hide: true
hidefromtoc: true
feature: Release Information, Dynamic Chat
source-git-commit: c2c95f36c710ba7a9ac75c2160c72e44b5f81a99
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 0%

---

# Note sulla versione: aprile 2024 {#release-notes-apr-24}

I rilasci di Adobe Dynamic Chat funzionano su un modello di distribuzione continua che consente un approccio più scalabile alla distribuzione delle funzioni. A volte ci sono più versioni in un mese, quindi controlla regolarmente per informazioni sempre aggiornate.

Pagina Note sulla versione standard per il Marketo Engage [si trova qui](/help/marketo/release-notes/current.md){target="_blank"}.

## Versione di aprile {#april-release}

**Data di rilascio: 16 aprile 2024**

### Flussi conversazionali ora disponibili per i clienti su Seleziona pacchetto {#conversational-flows-select-package}

Quando abbiamo rilasciato i flussi conversazionali l’anno scorso, i clienti del pacchetto Dynamic Chat Select potevano sfruttare questa funzionalità solo come prova di 100 impegni a vita. Ora i flussi conversazionali sono completamente disponibili per tutti i clienti nel pacchetto Select.

Gli impegni di flusso conversazionale verranno conteggiati fino al limite mensile di 250 conversazioni impegnate per i clienti nel pacchetto Select.

### Funzioni di callback {#callback-functions}

Le funzioni di callback consentono di raccogliere eventi di analisi del Dynamic Chat in sistemi esterni, come Adobe Analytics o Google Analytics, in modo che i visitatori possano interagire con le conversazioni di Dynamic Chat. Per abilitare gli eventi di analisi di Dynamic Chat, devi registrare un callback con l’API per ascoltare gli eventi. Questo ti consente di avere una visione più olistica del coinvolgimento del Dynamic Chat in relazione ad altri dati chiave, come il traffico web.

### Sono state aggiunte condizioni di disponibilità dell’agente live al ramo condizionale {#live-agent-availability-conditional-branching}

Oltre ai campi Marketo nativi e personalizzati, ora puoi utilizzare la diramazione condizionale per creare rami in base alla disponibilità dell’agente. Questo è utile se desideri offrire ai visitatori solo l’opzione di parlare con un agente live quando sono disponibili agenti live.

SCHERMATA

### Condizione elenco smart aggiunta alla diramazione condizionale {#smart-list-condition}

Con l’aggiunta della nuova condizione Elenco avanzato Marketo Engage nel ramo condizionale, puoi creare rami in base ai tipi di pubblico preesistenti già creati in Marketo, anziché definire le condizioni di ramo del pubblico nel Dynamic Chat.

SCHERMATA

### Diramazione condizionale per flussi conversazionali {#conditional-branching-for-conversational-flows}

All’inizio di quest’anno è stata rilasciata la diramazione condizionale per i dialoghi e ora puoi sfruttare questa possibilità anche nei flussi conversazionali. La diramazione condizionale consente di creare diramazioni nel flusso in base a condizioni diverse.

### Chat live per flussi conversazionali {#live-chat-for-conversational-flows}

L’anno scorso abbiamo rilasciato la funzionalità di chat in diretta per Dialogs e ora puoi aggiungere impegni di chat in diretta anche nei flussi conversazionali. Se utilizzi i flussi di conversazione con i moduli Marketo, ora puoi consentire ai visitatori qualificati di chattare con un agente live immediatamente dopo l’invio del modulo.

### Attività recenti del Marketo Engage nella casella in entrata dell’agente {#recent-marketo-engage-activities-in-agent-inbox}

Abbiamo aggiunto le attività di Marketo Engage recenti alla sezione Attività recenti della casella in entrata dell’agente in modo che, quando un visitatore del sito richiede di chattare con un agente, l’agente possa facilmente vedere se il visitatore è stato recentemente coinvolto in una delle seguenti attività di Marketo (ultime 25 attività):

* E-mail aperta
* Pagina Web visitata
* Modulo compilato
* Momento interessante

SCHERMATA

### Stato della connessione al calendario in Gestione agenti {#calendar-connection-status-in-agent-management}

Gli amministratori possono ora vedere facilmente quali agenti con autorizzazioni per la prenotazione di riunioni hanno connesso i loro calendari nel Dynamic Chat. In questo modo è possibile assicurarsi che l&#39;intero team vendite sia connesso e pronto ad accettare convocazioni di riunioni dal Dynamic Chat.

SCHERMATA

### Impostazione avviso minimo nella configurazione del calendario dell&#39;agente {#minimum-notice-setting-in-agent-calendar-configuration}

I clienti hanno segnalato che i visitatori web prenotavano le riunioni sul calendario con appena 10 minuti di preavviso, per questo abbiamo introdotto un’impostazione di preavviso minimo nella configurazione del calendario dell’agente e impostato il lead time predefinito su 24 ore.

SCHERMATA

### Nuove notifiche in-app {#new-in-app-notifications}

Sono state introdotte tre nuove notifiche in-app per mantenerti informato sullo stato dell’istanza di Dynamic Chat in tempo reale.

* Testo
* Testo
* Testo

### Comportamento dell&#39;utente aggiunto/rimosso aggiornato {#add-remove-user-behavior-updated}

Alcuni clienti ci informano dei problemi riscontrati con l’aggiunta e la rimozione di agenti in Dynamic Chat, per cui abbiamo apportato alcune modifiche per risolvere questi problemi.

Quando un utente viene aggiunto all’Admin Console con l’autorizzazione per chat in diretta o prenotazione riunione, viene immediatamente visualizzato nell’elenco Gestione agenti e può essere aggiunto a Finestre di dialogo, Flussi conversazionali, regole di routing e team.

Quando un utente con autorizzazioni per la prenotazione di riunioni o la chat in tempo reale viene rimosso da Admin Console, verrà immediatamente rimosso dal Dynamic Chat, non sarà più disponibile per la chat in tempo reale o l’instradamento di riunioni e non verrà più conteggiato rispetto ai limiti di licenza.

### Migliori prestazioni del rapporto a livello di conversazione {#improved-conversation-level-report-performance}

I rapporti a livello di dialogo individuale e di flusso conversazionale ora sono più performanti e precisi. In precedenza, il caricamento dei rapporti delle finestre di dialogo poteva richiedere diversi secondi e i dati talvolta non erano coerenti con i rapporti sulle prestazioni globali. Ora i singoli rapporti della finestra di dialogo vengono caricati in un istante e i dati saranno sempre allineati con i dati di reporting globali.

SCHERMATA

### Aggiornamenti delle autorizzazioni {#permission-updates}

Abbiamo ripulito la struttura delle autorizzazioni e la denominazione in Adobe Admin Console per rendere la gestione delle autorizzazioni più intuitiva.

* La categoria Gestione conversazioni è ora denominata Conversazioni
* La categoria Riunioni è ora denominata Attività
* La categoria Impostazioni agente è ora denominata Agenti
* La categoria Impostazioni amministratore è ora denominata Configurazione
* La categoria Chat live è stata rimossa e tutte le autorizzazioni di chat live sono state spostate nella categoria Agenti

SCHERMATA

### Supporto per i collegamenti ipertestuali nella casella in entrata dell’agente {#support-for-hyperlinks-in-agent-inbox}

Ora, quando gli agenti di chat live condividono gli URL con i visitatori nella chat, questi saranno collegati ipertestualmente in modo che i visitatori possano semplicemente fare clic su di essi per passare alla pagina, anziché dover copiare e incollare l’URL nel browser.

### Immettete il comportamento chiave aggiornato nella casella in entrata dell&#39;agente {#enter-key-behavior-updated-in-agent-inbox}

È stato cambiato il comportamento del tasto di ritorno nella casella in entrata dell’agente, in modo che premendo il tasto Invio o A capo si invii il messaggio e premendo Maiusc+Invio si crei un’interruzione di riga.

SCHERMATA

### Pagina Round robin rimossa {#round-robin-page-removed}

Non si preoccupi! Round robin routing è ancora completamente funzionale e funziona come sempre. Abbiamo appena rimosso la pagina che mostrava un elenco spesso impreciso di agenti e il loro ordine nella coda di routing round robin.

Per fornire un contesto, quando abbiamo rilasciato il Dynamic Chat nel 2022, non c’era supporto per la chat in diretta, solo la prenotazione di riunioni e la pagina di indirizzamento round robin è stata progettata solo per la prenotazione di riunioni. Con l&#39;introduzione della chat dal vivo lo scorso anno, la pagina round robin è diventata obsoleta perché non rifletteva con precisione la natura più complessa del round robin routing tra agenti con sia la prenotazione delle riunioni che le autorizzazioni di chat dal vivo. Abbiamo esplorato alcune opzioni diverse per risolvere questo problema, ma alla fine abbiamo deciso che rimuoverlo del tutto era l’opzione migliore per ridurre al minimo la confusione.

## Versione di febbraio {#february-release}

**Data di rilascio: 22 febbraio 2024**

### Pagina Conversazioni {#conversations-page}

La nuova pagina Conversazioni offre un unico punto di riferimento per la visualizzazione delle trascrizioni di tutte le conversazioni (automatizzate e live) avvenute per la tua istanza, da lead noti e anonimi, fornendo una migliore visibilità sul modo in cui i clienti si relazionano con i tuoi dialoghi, flussi conversazionali e agenti live.

SCHERMATA

L’intervallo di date nel dashboard globale è aumentato da 90 giorni a 24 mesi

Hai chiesto e abbiamo consegnato. Ora è possibile visualizzare i dati di coinvolgimento del Dynamic Chat fino a due anni in tutte le dashboard di Analytics.

### Diramazione condizionale nelle finestre di dialogo {#conditional-branching-in-dialogues}

La diramazione condizionale consente di creare rami nei flussi della finestra di dialogo in base a condizioni diverse. Ora è possibile presentare contenuti diversi a persone diverse nella stessa finestra di dialogo in base agli attributi del lead e dell’azienda in Marketo.

## Versione di gennaio {#january-release}

**Data di rilascio: 24 gennaio 2024**

### Limite simultaneo di chat live nella gestione degli agenti {#Concurrent-live-chat-limit-setting}

Per impostazione predefinita, ogni agente di chat live nella tua istanza può partecipare a un massimo di 5 sessioni di chat live alla volta. Abbiamo introdotto una nuova impostazione nella gestione degli agenti che consente di regolare questo limite da 1 a 10.

SCHERMATA
