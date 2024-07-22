---
unique-page-id: 14745730
description: Diagnostica Salesforce - Documentazione Marketo - Documentazione del prodotto
title: Diagnostica Salesforce
exl-id: a2b5bd10-bc92-4fd4-bc1b-4e02b48c9d83
feature: Marketo Sales Connect
source-git-commit: 9384d72b335a4b975b190816ea999ad067fddeda
workflow-type: tm+mt
source-wordcount: '1354'
ht-degree: 0%

---

# Diagnostica Salesforce {#salesforce-diagnostics}

Parte dell’integrazione con Salesforce include una pagina di diagnostica Salesforce all’interno dell’applicazione web. Questa pagina acquisisce gli errori derivanti dalla registrazione dei dati non riuscita in Salesforce. Gli errori possono essere utili, ma non sono sempre leggibili. Per questo motivo, abbiamo creato una scheda di riferimento che aiuta a spiegare i messaggi di errore.

**Errore:** API_CURRENT_DISABLED\
**Categoria:** Accesso/Convalida\
**Messaggio: l&#39;API** è disabilitata per questo utente\
**Cosa sta succedendo:** l&#39;utente non dispone dell&#39;accesso API\
**Passaggi per la risoluzione dei problemi:** l&#39;amministratore Salesforce deve concedere all&#39;utente l&#39;accesso API.

<br> 

**Errore:** ERRORE_AUTENTICAZIONE\
**Categoria:** Autenticazione\
**Messaggio:** invalid_grant: errore di autenticazione\
**Operazione in corso:** autenticazione non riuscita\
**Passaggi per la risoluzione dei problemi:** Disconnettiti da Salesforce, quindi riconnettiti.

<br> 

**Errore:** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY\
**Categoria:** Accesso/Convalida\
**Messaggio:** {&quot;errorCode&quot;:&quot;INVALID_SESSION_ID&quot;,&quot;messaggio&quot;:&quot;Sessione scaduta o non valida&quot;}\
**In corso:**

1 - Il codice del trigger non riesce a eseguire l’aggiornamento.\
2 - L’utente non dispone di autorizzazioni di scrittura a livello di oggetto per l’oggetto specificato.

**Passaggi per la risoluzione dei problemi:**

1 - Errore durante la revisione del trigger.\
2 - Concedere all&#39;utente l&#39;accesso in scrittura per l&#39;oggetto OPPURE disabilitare la funzione che sta tentando di scrivere sull&#39;oggetto.

<br> 

**Errore:** CANNOT_UPDATE_CONVERTED_LEAD\
**Categoria:** Altro\
**Messaggio:** non può fare riferimento al lead convertito\
**Cosa sta succedendo:** stiamo tentando di accedere a un lead convertito durante la registrazione attività più recente per contatti e lead. Ho visto anche un paio di questi per le piazzole.\
**Procedura di risoluzione dei problemi:** Segnala eventuali istanze di questo al nostro [team di supporto](https://nation.marketo.com/t5/Support/ct-p/Support).

<br> 

**Errore:** ENTITY_IS_LOCKED\
**Categoria:** Accesso/Convalida\
**Messaggio:** l&#39;entità è bloccata per la modifica\
**Operazione in corso:** Il record è in un processo di approvazione in cui è bloccato da eventuali modifiche aggiuntive fino a quando non viene approvato o negato da un utente proprietario dell&#39;approvazione.\
**Passaggi per la risoluzione dei problemi:** Vedi sopra.

<br> 

**Errore:** EXPIRED_ACCESS
**Categoria:** Autenticazione
**Messaggio:** invalid_grant: token di accesso/aggiornamento scaduto
**Operazione in corso:** Il token di accesso o di aggiornamento è scaduto. I token scadono in base alle [impostazioni di sessione in Salesforce](https://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via).
**Passaggi per la risoluzione dei problemi:** Sarà necessario ripetere l&#39;autenticazione. Disconnetti la connessione Salesforce e riconnettiti.

<br> 

**Errore:** FAILED_WRITE\
**Categoria:** intermittente\
**Messaggio:** fine file raggiunta\
**Cosa sta succedendo:** problema di prestazioni con Salesforce, probabilmente dovuto a trigger non ottimali sul lato cliente.\
**Passaggi per la risoluzione dei problemi:** La logica dei tentativi deve gestire questo problema. Se il problema persiste, contatta l’amministratore Salesforce per risolvere il problema del trigger.

<br> 

**Errore:** FIELD_CUSTOM_VALIDATION_EXCEPTION
**Categoria:** Accesso/Convalida
**Messaggio:** Varia da cliente a cliente.
**Operazione in corso:** Impossibile eseguire una regola di convalida personalizzata per l&#39;oggetto.
**Passaggi per la risoluzione dei problemi:** Controllare la regola di convalida personalizzata che causa l&#39;errore. Trattandosi di una regola consuetudinaria, l’errore deve essere trattato una tantum.

<br> 

**Errore:** FIELD_FILTER_VALIDATION_EXCEPTION\
**Categoria:** Accesso/Convalida\
**Messaggio:** Il valore non esiste o non corrisponde ai criteri di filtro\
**Cosa sta succedendo:** dati non validi esistenti in Salesforce che vengono applicati al momento dell&#39;aggiornamento.\
**Passaggi per la risoluzione dei problemi:** Vedi sopra.

<br> 

**Errore:** FIELD_INTEGRITY_EXCEPTION\
**Categoria:** Accesso/Convalida\
**Messaggio:** Il paese/territorio esistente non riconosce il valore dello stato per il campo: Codice stato/provincia\
**Cosa sta succedendo:** dati non validi esistenti in Salesforce che vengono applicati al momento dell&#39;aggiornamento.\
**Passaggi per la risoluzione dei problemi:** Vedi sopra.

<br> 

**Errore:** INACTIVE_ORGANIZATION\
**Categoria:** Autenticazione\
**Messaggio:** invalid_grant: organizzazione inattiva\
**In corso:** L&#39;organizzazione Salesforce non è più attiva.\
**Passaggi per la risoluzione dei problemi:** Disconnettiti e riconnettiti da Salesforce.

**Errore:** INACTIVE_USER
**Categoria:** Autenticazione
**Messaggio:** invalid_grant: utente inattivo
**In corso:** L&#39;utente Salesforce non è più attivo
**Passaggi per la risoluzione dei problemi:** Disconnettiti e riconnettiti da Salesforce.

**Errore:** INSERT_UPDATE_DELETE_NOT_ALLOWED_WHILE_MAINTENANCE\
**Categoria:** intermittente\
**Messaggio:** (nessun messaggio aggiuntivo)\
**Operazione in corso:** l&#39;istanza Salesforce è in modalità di manutenzione.\
**Passaggi per la risoluzione dei problemi:** Attendere il completamento della manutenzione del sistema, quindi riprovare a eseguire la registrazione.

**Errore:** INSUFFICIENTE_ACCESS_ON_CROSS_REFERENCE_ENTITY
**Categoria:** Accesso/Convalida
**Messaggio:** diritti di accesso insufficienti per l&#39;ID oggetto
**Operazione in corso:** Nessun accesso al record padre per un&#39;attività.
**Passaggi per la risoluzione dei problemi:** Vedi sopra.

<br> 

**Errore:** INSUFFICIENTE_ACCESS_OR_READONLY\
**Categoria:** Accesso/Convalida
**Messaggio:** diritti di accesso insufficienti per l&#39;ID oggetto
**Operazione in corso:** La registrazione attività più recente non è in grado di modificare il record specifico perché l&#39;utente non dispone dell&#39;accesso in scrittura.\
**Passaggi per la risoluzione dei problemi:** Concedere all&#39;utente l&#39;accesso in Salesforce OPPURE disabilitare la registrazione delle attività più recenti per l&#39;oggetto per l&#39;utente.

**Errore:** INVALID_FIELD\
**Categoria:** intermittente\
**Messaggio:** Net::ReadTimeout\
**In corso:** Timeout della richiesta. Questo è probabilmente il risultato di troppe transazioni lente.\
**Passaggi per la risoluzione dei problemi:** esamina le personalizzazioni esistenti per individuare i potenziali responsabili dei problemi di latenza e/o disabilita la registrazione delle attività più recenti per uno o tutti gli oggetti per ridurre il carico.

**Errore:** INVALID_FIELD_FOR_INSERT_UPDATE\
**Categoria:** Accesso/Convalida\
**Messaggio:** Impossibile creare/aggiornare i campi: ToutApp__Tout_Last_Relied__c. Verifica le impostazioni di protezione di questo campo.
**Operazione in corso:** gli utenti non dispongono dell&#39;accesso in scrittura ai campi personalizzati Tout necessari per eseguire la transazione di registrazione attività più recente. È possibile che il team abbia installato il pacchetto ma non abbia attivato i campi corretti per gli utenti.\
**Procedura per la risoluzione dei problemi:** L&#39;amministratore Salesforce deve concedere l&#39;accesso ai campi personalizzati OPPURE disattivare la registrazione delle attività più recenti.

**Errore:** INVALID_GRANT\
**Categoria:** Autenticazione\
**Messaggio:** invalid_grant: ip limitato\
**Cosa sta succedendo:** stiamo tentando di accedere alla tua Salesforce, ma sono presenti restrizioni IP che ci impediscono di farlo.\
inserire nell&#39;elenco Consentiti **Passaggi per la risoluzione dei problemi:** L&#39;amministratore Salesforce dovrà i nostri IP. Gli utenti devono contattare il supporto tecnico per ottenere gli indirizzi IP.

**Errore:** INVALID_TYPE\
**Categoria:** Accesso/Convalida\
**Messaggio:** CreatedDate, (SELECT Id FROM Tasks) FROM Lead WHERE E-mail=&#39;emailid&#39;^ERROR at `Row:1:Column:53sObject` type &#39;Lead&#39; non è supportato. Se tenti di utilizzare un oggetto personalizzato, assicurati di aggiungere &quot;__c&quot; dopo il nome dell’entità. Fai riferimento al tuo WSDL o alla chiamata descrittiva per i nomi appropriati
**In corso:** stiamo tentando di eseguire una query su un tipo di oggetto di Salesforce a cui l&#39;utente non ha accesso. Ciò è probabilmente dovuto al fatto che l’utente non dispone del diritto di accesso all’oggetto lead.\
**Passaggi per la risoluzione dei problemi:** Concedi l&#39;accesso in lettura e aggiornamento all&#39;oggetto Lead in Salesforce oppure disattiva la registrazione e-mail e la registrazione attività più recente nei record dei lead.

**Errore:** QUERY_TIMEOUT\
**Categoria:** intermittente\
**Messaggio:** la richiesta di query è stata eseguita troppo a lungo\
**Cosa sta succedendo:** Vedi sopra.\
**Passaggi per la risoluzione dei problemi:** La logica dei tentativi deve gestire questo problema. Se il problema persiste, contatta l’amministratore Salesforce per risolvere il problema del trigger.

**Errore:** REQUEST_LIMIT_EXCEEDED\
**Categoria:** intermittente\
**Messaggio:**
1 - Limite ConcurrentPerOrgLongTxn superato\
2 - Limite TotalRequests superato\
3 - ConcurrentRequest\
**In corso:**
1 - È stato superato il limite di richieste simultanee, probabilmente a causa di un codice di attivazione inefficiente.\
2 - Troppe integrazioni superano la finestra continua di 24 ore.\
**Passaggi per la risoluzione dei problemi:**
1 - Verifica i trigger esistenti sugli oggetti interessati. Disattivare potenzialmente la registrazione di rollup per uno o più oggetti.\
2 - Acquista altre chiamate API da Salesforce. Disattivare potenzialmente la registrazione di rollup per uno o più oggetti.

**Errore:** CAMPO_OBBLIGATORIO_MANCANTE\
**Categoria:** Accesso/Convalida\
**Messaggio:** Campi obbligatori mancanti: `[Amount_Committed_Private_Capital__c]`
**Cosa sta succedendo:** Questo generalmente accade per la registrazione delle attività più recenti. I campi personalizzati erano impostati per essere obbligatori ma contenevano valori vuoti. Ciò può verificarsi se il record è stato creato con un valore vuoto del campo personalizzato e quindi è stato reso obbligatorio. La richiesta viene applicata quando si tenta di aggiornare il record, anche se il campo personalizzato non viene toccato.\
**Passaggi per la risoluzione dei problemi:** Aggiorna manualmente i valori dei campi mancanti. Puoi quindi riprovare a inviare il messaggio da ToutApp.

**Errore:** SERVER_NON DISPONIBILE\
**Categoria:** intermittente\
**Messaggio:** server troppo occupato\
**Cosa sta succedendo:** problema di prestazioni con Salesforce, probabilmente dovuto a trigger non ottimali del cliente\
**Passaggi per la risoluzione dei problemi:** La logica dei tentativi deve gestire questo problema. Se il problema persiste, rivolgiti al tuo amministratore Salesforce per risolvere il problema di un trigger.

**Errore:** TXN_SECURITY_NO_ACCESS\
**Categoria:** Accesso/Convalida\
**Messaggio:** l&#39;operazione richiesta non è consentita a causa di criteri di sicurezza nell&#39;organizzazione. Contatta l’amministratore.<br/>
**In corso:** È stato impostato un tipo di restrizione di sicurezza. Vedere https://developer.salesforce.com/forums/?id=&quot;ID record&quot;\
**Passaggi per la risoluzione dei problemi:** Rivolgiti al tuo amministratore Salesforce e scopri quale potrebbe essere la restrizione specifica.

**Errore:** IMPOSSIBILE_BLOCCARE_RIGA\
**Categoria:** intermittente\
**Messaggio:** impossibile ottenere l&#39;accesso esclusivo a questo record o a 1 record: &quot;ID record&quot;\
**Cosa sta accadendo:** è probabile che un trigger stia causando più tentativi di accesso allo stesso record, probabilmente nel caso di un&#39;e-mail di gruppo.\
**Passaggi per la risoluzione dei problemi:** La logica dei tentativi deve gestire questo problema. Se il problema persiste, contatta l’amministratore Salesforce per risolvere il problema del trigger.

**Errore:** ECCEZIONE_SCONOSCIUTA
**Categoria:** Altro\
**Messaggio:** Si è verificata un&#39;eccezione sconosciuta\
**In corso:** Eccezione non gestita in Salesforce.\
**Passaggi per la risoluzione dei problemi:** Crea un caso con Salesforce e copia i valori numerici nel messaggio di errore. Questo è il codice Salesforce che non gestisce correttamente un errore.
