---
description: Diagnostica Salesforce - Documentazione Marketo - Documentazione del prodotto
title: Diagnostica Salesforce
exl-id: c449f938-9615-47cb-b232-613ec29068a3
source-git-commit: 15c3124a53ce55810b598c43e29e21321534c81f
workflow-type: tm+mt
source-wordcount: '1445'
ht-degree: 0%

---

# Diagnostica Salesforce {#salesforce-diagnostics}

Parte dell’integrazione con Salesforce include una pagina di diagnostica Salesforce all’interno dell’applicazione web. Questa pagina acquisisce gli errori derivanti dalla registrazione dei dati non riuscita in Salesforce. Gli errori possono essere utili, ma non sono sempre leggibili. Per questo motivo, abbiamo creato una scheda di riferimento che aiuta a spiegare i messaggi di errore.

## Diagnostica degli accessi {#access-diagnostics}

1. Fai clic sull’icona a forma di ingranaggio e scegli **Impostazioni**.

   ![](assets/salesforce-diagnostics-1.png)

1. In Integrazioni, fai clic su **Diagnostica**.

   ![](assets/salesforce-diagnostics-2.png)

## Scheda di riferimento per gli errori {#error-cheat-sheet}

**Errore:** API_CURRENT_DISABLED\
**Categoria:** Accesso/convalida\
**Messaggio:** API disabilitata per questo utente\
**Cosa sta succedendo:** L’utente non dispone dell’accesso API\
**Passaggi per la risoluzione dei problemi:** L’amministratore Salesforce deve concedere all’utente l’accesso API.

**Errore:** AUTHENTICATION_FAILURE\
**Categoria:** Autenticazione\
**Messaggio:** invalid_grant: errore di autenticazione\
**Cosa sta succedendo:** Autenticazione non riuscita\
**Passaggi per la risoluzione dei problemi:** Disconnettiti da Salesforce, quindi riconnettiti.

**Errore:** IMPOSSIBILE_INSERIRE_AGGIORNA_ATTIVA_ENTITÀ\
**Categoria:** Accesso/convalida\
**Messaggio:** {&quot;errorCode&quot;:&quot;INVALID_SESSION_ID&quot;,&quot;message&quot;:&quot;Sessione scaduta o non valida&quot;}\
**Cosa sta succedendo:**

1 - Il codice del trigger non riesce a eseguire l’aggiornamento.\
2 - L’utente non dispone di autorizzazioni di scrittura a livello di oggetto per l’oggetto specificato.

**Passaggi per la risoluzione dei problemi:**

1 - Errore durante la revisione del trigger.\
2 - Concedere all&#39;utente l&#39;accesso in scrittura per l&#39;oggetto OPPURE disabilitare la funzione che sta tentando di scrivere sull&#39;oggetto.

**Errore:** CANNOT_UPDATE_CONVERTED_LEAD\
**Categoria:** Altro\
**Messaggio:** impossibile fare riferimento al lead convertito\
**Cosa sta succedendo:** Stiamo tentando di accedere a un lead convertito durante la registrazione delle attività più recenti per contatti e lead. Ho visto anche un paio di questi per le piazzole.\
**Passaggi per la risoluzione dei problemi:** Segnala eventuali istanze di questo al nostro [team di supporto](https://nation.marketo.com/t5/Support/ct-p/Support).

**Errore:** ENTITY_IS_LOCKED\
**Categoria:** Accesso/convalida\
**Messaggio:** l’entità è bloccata per la modifica\
**Cosa sta succedendo:** Il record è in un processo di approvazione in cui è bloccato da eventuali modifiche aggiuntive fino a quando non viene approvato o negato da una persona a cui appartiene l&#39;approvazione.\
**Passaggi per la risoluzione dei problemi:** Vedi sopra.

**Errore:** EXPIRED_ACCESS
**Categoria:** Autenticazione
**Messaggio:** invalid_grant: token di accesso/aggiornamento scaduto
**Cosa sta succedendo:** Il token di accesso o di aggiornamento è scaduto. I token scadono in base a [impostazioni di sessione in Salesforce](https://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via).
**Passaggi per la risoluzione dei problemi:** Sarà necessario autenticare di nuovo. Disconnetti la connessione Salesforce e riconnettiti.

**Errore:** SCRITTURA_NON RIUSCITA\
**Categoria:** Intermittente\
**Messaggio:** fine del file raggiunta\
**Cosa sta succedendo:** Problema di prestazioni con Salesforce, probabilmente dovuto a trigger non ottimali sul lato cliente.\
**Passaggi per la risoluzione dei problemi:** La logica dei tentativi deve gestire questo problema. Se il problema persiste, contatta l’amministratore Salesforce per risolvere il problema del trigger.

**Errore:** FIELD_CUSTOM_VALIDATION_EXCEPTION
**Categoria:** Accesso/convalida
**Messaggio:** Varia da cliente a cliente.
**Cosa sta succedendo:** Impossibile eseguire una regola di convalida personalizzata per l&#39;oggetto.
**Passaggi per la risoluzione dei problemi:** Controllare la regola di convalida personalizzata che causa l&#39;errore. Trattandosi di una regola consuetudinaria, l’errore deve essere trattato una tantum.

**Errore:** FIELD_FILTER_VALIDATION_EXCEPTION\
**Categoria:** Accesso/convalida\
**Messaggio:** Il valore non esiste o non corrisponde ai criteri del filtro\
**Cosa sta succedendo:** I dati non validi esistenti in Salesforce vengono applicati al momento dell’aggiornamento.\
**Passaggi per la risoluzione dei problemi:** Vedi sopra.

**Errore:** FIELD_INTEGRITY_EXCEPTION\
**Categoria:** Accesso/convalida\
**Messaggio:** Il paese/territorio esistente non riconosce il valore di stato per il campo: Codice stato/provincia\
**Cosa sta succedendo:** I dati non validi esistenti in Salesforce vengono applicati al momento dell’aggiornamento.\
**Passaggi per la risoluzione dei problemi:** Vedi sopra.

**Errore:** INACTIVE_ORGANIZATION\
**Categoria:** Autenticazione\
**Messaggio:** invalid_grant: organizzazione inattiva\
**Cosa sta succedendo:** L&#39;organizzazione Salesforce non è più attiva.
**Passaggi per la risoluzione dei problemi:** Disconnettiti e riconnettiti da Salesforce.

**Errore:** INACTIVE_USER
**Categoria:** Autenticazione
**Messaggio:** invalid_grant: utente inattivo
**Cosa sta succedendo:** L’utente Salesforce non è più attivo
**Passaggi per la risoluzione dei problemi:** Disconnettiti e riconnettiti da Salesforce.

**Errore:** INSERT_UPDATE_DELETE_NOT_ALLOWED_WHILE_MAINTENANCE\
**Categoria:** Intermittente\
**Messaggio:** (nessun messaggio aggiuntivo)\
**Cosa sta succedendo:** L’istanza Salesforce è in modalità manutenzione.\
**Passaggi per la risoluzione dei problemi:** Attendere il completamento della manutenzione del sistema, quindi riprovare la registrazione.

**Errore:** INSUFFICIENTE_ACCESS_ON_CROSS_REFERENCE_ENTITY
**Categoria:** Accesso/convalida
**Messaggio:** diritti di accesso insufficienti sull&#39;id oggetto
**Cosa sta succedendo:** Nessun accesso al record padre per un&#39;attività.
**Passaggi per la risoluzione dei problemi:** Vedi sopra.

**Errore:** INSUFFICIENTE_ACCESS_OR_READONLY\
**Categoria:** Accesso/convalida
**Messaggio:** diritti di accesso insufficienti sull&#39;id oggetto
**Cosa sta succedendo:** La registrazione attività più recente non può modificare il record specifico perché l’utente non dispone dell’accesso in scrittura.\
**Passaggi per la risoluzione dei problemi:** Concedi all’utente l’accesso in Salesforce OPPURE disabilita la registrazione delle attività più recenti per tale oggetto per tale utente.

**Errore:** CAMPO_NON VALIDO\
**Categoria:** Intermittente\
**Messaggio:** Net::TimeoutLettura\
**Cosa sta succedendo:** Timeout della richiesta. Questo è probabilmente il risultato di troppe transazioni lente.\
**Passaggi per la risoluzione dei problemi:** Esamina le personalizzazioni esistenti per individuare potenziali colpevoli dei problemi di latenza e/o disabilita la registrazione delle attività più recenti per uno o tutti gli oggetti al fine di ridurre il carico.

**Errore:** INVALID_FIELD_FOR_INSERT_UPDATE\
**Categoria:** Accesso/convalida\
**Messaggio:** Impossibile creare/aggiornare i campi: MSE_Relied__c. Verifica le impostazioni di protezione di questo campo.
**Cosa sta succedendo:** Gli utenti non dispongono dell’accesso in scrittura ai campi personalizzati delle Azioni di approfondimento sulle vendite necessari per eseguire la transazione di registrazione dell’attività più recente. È possibile che il team abbia installato il pacchetto ma non abbia attivato i campi corretti per gli utenti.\
**Passaggi per la risoluzione dei problemi:** L’amministratore Salesforce deve concedere l’accesso ai campi personalizzati O disattivare la registrazione delle attività più recenti.

**Errore:** INVALID_GRANT\
**Categoria:** Autenticazione\
**Messaggio:** invalid_grant: ip limitato\
**Cosa sta succedendo:** Stiamo tentando di accedere alla tua Salesforce, ma sono in vigore restrizioni IP che ci impediscono di farlo.\
**Passaggi per la risoluzione dei problemi:** Il tuo amministratore Salesforce dovrà inserire nell&#39;elenco Consentiti i nostri IPs. Gli utenti devono contattare il supporto tecnico per ottenere gli indirizzi IP.

**Errore:** INVALID_TYPE\
**Categoria:** Accesso/convalida\
**Messaggio:** CreatedDate, (SELECT Id FROM Tasks) FROM Lead WHERE E-mail=&#39;emailid&#39;^ERROR at Row:1:Column:53sIl tipo &#39;Lead&#39; di oggetto non è supportato. Se tenti di utilizzare un oggetto personalizzato, assicurati di aggiungere &quot;__c&quot; dopo il nome dell’entità. Fai riferimento al tuo WSDL o alla chiamata descrittiva per i nomi appropriati
**Cosa sta succedendo:** Stiamo tentando di eseguire una query su un tipo di oggetto da Salesforce a cui l’utente non ha accesso. Ciò è probabilmente dovuto al fatto che l’utente non dispone del diritto di accesso all’oggetto lead.\
**Passaggi per la risoluzione dei problemi:** Concedi l’accesso in lettura e aggiornamento all’oggetto Lead in Salesforce, oppure disattiva la registrazione e-mail e la registrazione delle attività più recenti per i record dei lead.

**Errore:** QUERY_TIMEOUT\
**Categoria:** Intermittente\
**Messaggio:** La richiesta di query era in esecuzione troppo lunga\
**Cosa sta succedendo:** Vedi sopra.\
**Passaggi per la risoluzione dei problemi:** La logica dei tentativi deve gestire questo problema. Se il problema persiste, contatta l’amministratore Salesforce per risolvere il problema del trigger.

**Errore:** REQUEST_LIMIT_EXCEEDED\
**Categoria:** Intermittente\
**Messaggio:**
1 - Limite ConcurrentPerOrgLongTxn superato\
2 - Limite TotalRequests superato\
3 - ConcurrentRequest\
**Cosa sta succedendo:**
1 - È stato superato il limite di richieste simultanee, probabilmente a causa di un codice di attivazione inefficiente.\
2 - Troppe integrazioni superano la finestra continua di 24 ore.\
**Passaggi per la risoluzione dei problemi:**
1 - Verifica i trigger esistenti sugli oggetti interessati. Disattivare potenzialmente la registrazione di rollup per uno o più oggetti.\
2 - Acquista altre chiamate API da Salesforce. Disattivare potenzialmente la registrazione di rollup per uno o più oggetti.

**Errore:** CAMPO_OBBLIGATORIO_MANCANTE\
**Categoria:** Accesso/convalida\
**Messaggio:** Mancano campi obbligatori: `[Amount_Committed_Private_Capital__c]`
**Cosa sta succedendo:** Questo accade generalmente per la registrazione delle attività più recenti. I campi personalizzati erano impostati per essere obbligatori ma contenevano valori vuoti. Ciò può verificarsi se il record è stato creato con un valore vuoto del campo personalizzato e quindi è stato reso obbligatorio. La richiesta viene applicata quando si tenta di aggiornare il record, anche se il campo personalizzato non viene toccato.\
**Passaggi per la risoluzione dei problemi:** Aggiorna manualmente i valori dei campi mancanti. A questo punto puoi ripetere il messaggio da Azioni approfondimento vendite.

**Errore:** SERVER_UNAVAILABLE\
**Categoria:** Intermittente\
**Messaggio:** server troppo occupato\
**Cosa sta succedendo:** Problema di prestazioni con Salesforce, probabilmente dovuto a trigger non ottimali del cliente\
**Passaggi per la risoluzione dei problemi:** La logica dei tentativi deve gestire questo problema. Se il problema persiste, rivolgiti al tuo amministratore Salesforce per risolvere il problema di un trigger.

**Errore:** TXN_SECURITY_NO_ACCESS\
**Categoria:** Accesso/convalida\
**Messaggio:** L&#39;operazione richiesta non è consentita a causa di un criterio di sicurezza nell&#39;organizzazione. Contatta l’amministratore.
**Cosa sta succedendo:** È stato impostato un tipo di restrizione di sicurezza. Consulta https://developer.salesforce.com/forums/?id=&quot;ID record&quot;\
**Passaggi per la risoluzione dei problemi:** Parla con il tuo amministratore Salesforce e scopri quale potrebbe essere la restrizione specifica.

**Errore:** IMPOSSIBILE_BLOCCARE_RIGA\
**Categoria:** Intermittente\
**Messaggio:** impossibile ottenere l’accesso esclusivo a questo record o a 1 record: &quot;record ID&quot;\
**Cosa sta succedendo:** Probabilmente esiste un trigger che sta causando più tentativi di accesso allo stesso record, probabilmente nel caso di un’e-mail di gruppo.\
**Passaggi per la risoluzione dei problemi:** La logica dei tentativi deve gestire questo problema. Se il problema persiste, contatta l’amministratore Salesforce per risolvere il problema del trigger.

**Errore:** ECCEZIONE_SCONOSCIUTA
**Categoria:** Altro\
**Messaggio:** Si è verificata un&#39;eccezione sconosciuta\
**Cosa sta succedendo:** Eccezione non gestita in Salesforce.\
**Passaggi per la risoluzione dei problemi:** Inserisci una maiuscola in minuscolo con Salesforce e copia i valori numerici nel messaggio di errore. Questo è il codice Salesforce che non gestisce correttamente un errore.
