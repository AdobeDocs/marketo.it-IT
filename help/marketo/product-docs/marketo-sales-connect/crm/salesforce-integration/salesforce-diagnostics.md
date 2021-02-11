---
unique-page-id: 14745730
description: Diagnostica Salesforce - Documenti Marketo - Documentazione del prodotto
title: Diagnostica Salesforce
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '1427'
ht-degree: 0%

---


# Diagnostica Salesforce {#salesforce-diagnostics}

Parte della nostra integrazione Salesforce include una pagina Diagnostica Salesforce all&#39;interno dell&#39;applicazione Web. Questa pagina acquisisce gli errori dalla registrazione dei dati non riuscita a Salesforce. Gli errori possono essere utili, ma non sempre leggibili. In quanto tali, abbiamo messo insieme un foglio di imbroglio che aiuta a spiegare i messaggi di errore.

**Errore:** API_CURRENTLY_DISABLED\
**Categoria:** Accesso/Convalida\
**Messaggio:** API disabilitata per l&#39;utente\
**Cosa succede:** L&#39;utente non dispone dell&#39;accesso API\
**Procedura di risoluzione dei problemi:** Salesforce Admin deve concedere all&#39;utente l&#39;accesso API.

<br> 

**Errore:** AUTHENTICATION_FAILURE\
**Categoria:** Autenticazione\
**Messaggio:** Invalid_Grant: errore di autenticazione\
**Cosa accade:** Autenticazione non riuscita\
**Procedura di risoluzione dei problemi:** scollegare da Salesforce e riconnettersi.

<br> 

**Errore:** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY\
**Categoria:** Accesso/Convalida\
**Messaggio:** {&quot;errorCode&quot;:&quot;INVALID_SESSION_ID&quot;,&quot;message&quot;:&quot;Sessione scaduta o non valida&quot;}\
**Cosa sta succedendo:**

1 - Il codice di attivazione causa il fallimento dell&#39;aggiornamento.\
2 - L&#39;utente non dispone di autorizzazioni di scrittura a livello di oggetto per l&#39;oggetto specificato.

**Procedura di risoluzione dei problemi:**

1 - Controllo dell&#39;attivatore non riuscito.\
2 - Concedere l&#39;accesso in scrittura all&#39;utente per l&#39;oggetto OPPURE disabilitare la funzionalità che sta tentando di scrivere nell&#39;oggetto.

<br> 

**Errore:** CANNOT_UPDATE_CONVERTED_LEAD\
**Categoria:** Altro\
**Messaggio:** impossibile fare riferimento al lead convertito\
**Cosa succede:** Stiamo tentando di accedere a un lead convertito durante la registrazione attività più recente per contatti e lead. Ho visto anche un paio di questi per le piazzole.\
**Procedura per la risoluzione dei problemi:** Segnalare eventuali casi al nostro team [ di ](https://nation.marketo.com/t5/Support/ct-p/Support)assistenza.

<br> 

**Errore:** ENTITY_IS_LOCKED\
**Categoria:** Accesso/Convalida\
**Messaggio:** l&#39;entità è bloccata per la modifica\
**Cosa accade:** Il record è in un processo di approvazione in cui viene bloccato da qualsiasi modifica aggiuntiva finché non viene approvato o rifiutato da una persona che possiede l&#39;approvazione.\
**Procedura per la risoluzione dei problemi:** vedere sopra.

<br> 

**Errore:** EXPIRED_ACCESS 
**Category:** Authentication 
**Message:** Invalid_Grant: token di accesso/aggiornamento scaduto 
**Cosa accade:** il token di accesso o aggiornamento è scaduto. I token scadono in base alle [impostazioni di sessione in Salesforce](https://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via).
**Procedura di risoluzione dei problemi:** dovrai autenticare nuovamente. Disconnetti la connessione Salesforce e ricollega.

<br> 

**Errore:** FAILED_WRITE\
**Categoria:** Intermittente\
**Messaggio:** fine del file raggiunto\
**Cosa succede: problema di** prestazioni con Salesforce, probabilmente a causa di attivazioni non ottimali dal lato del cliente.\
**Procedura di risoluzione dei problemi: la logica** dei tentativi deve gestire questo problema. Se non funziona, chiedi all’amministratore di Salesforce di risolvere eventuali problemi di attivazione.

<br> 

**Errore:** FIELD_CUSTOM_VALIDATION_EXCEPTION 
**Category:** Access/Validation 
**Message:** Varia da cliente a cliente.
**Cosa accade:** mancata riuscita di una regola di convalida personalizzata per l&#39;oggetto.
**Procedura di risoluzione dei problemi:** verificare la regola di convalida personalizzata che causa l&#39;errore. Poiché si tratta di una regola personalizzata, l&#39;errore deve essere risolto una tantum.

<br> 

**Errore:** FIELD_FILTER_VALIDATION_EXCEPTION\
**Categoria:** Accesso/Convalida\
**Messaggio:** Il valore non esiste o non corrisponde ai criteri del filtro\
**Cosa succede: i dati** errati esistenti in Salesforce vengono applicati al momento dell&#39;aggiornamento.\
**Procedura per la risoluzione dei problemi:** vedere sopra.

<br> 

**Errore:** FIELD_INTEGRITY_EXCEPTION\
**Categoria:** Accesso/Convalida\
**Messaggio:** Il paese/territorio esistente non riconosce il valore dello stato per il campo: Codice stato/provincia\
**Cosa succede: i dati** errati esistenti in Salesforce vengono applicati al momento dell&#39;aggiornamento.\
**Procedura per la risoluzione dei problemi:** vedere sopra.

<br> 

**Errore:** INACTIVE_ORGANIZATION\
**Categoria:** Autenticazione\
**Messaggio:** Invalid_Grant: organizzazione inattiva\
**Cosa succede:** la tua organizzazione Salesforce non è più attiva.\
**Procedura di risoluzione dei problemi:** Disconnetti e quindi ricollega da Salesforce.

**Errore:** INACTIVE_USER 
**Category:** Authentication 
**Message:** Invalid_Grant: utente inattivo 
**Cosa sta succedendo:** L’utente Salesforce non è più attivo 
**Procedura di risoluzione dei problemi:** Disconnetti e riconnette da Salesforce.

**Errore:** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MAINTENANCE\
**Categoria:** Intermittente\
**Messaggio:** (nessun messaggio aggiuntivo)\
**Cosa accade: l’istanza** Salesforce è in modalità di manutenzione.\
**Procedura di risoluzione dei problemi:** Attendere il completamento della manutenzione del sistema, quindi riprovare a registrare.

**Errore:** INSUFFICIENT_ACCESS_ON_CROSS_REFERENCE_ENTITY 
**Categoria:** Access/Validation 
**Message:** insufficienti diritti di accesso sull&#39;ID oggetto 
**Cosa accade:** Nessun accesso al record padre per un&#39;attività.
**Procedura per la risoluzione dei problemi:** vedere sopra.

<br> 

**Errore:** INSUFFICIENT_ACCESS_OR_READONLY\
**Categoria:** Accesso/
**Messaggio di convalida:diritti di accesso** insufficienti sull&#39;ID oggetto 
**Cosa accade:Registrazione attività** più recente non può modificare il record specifico perché l&#39;utente non dispone dell&#39;accesso in scrittura.\
**Procedura di risoluzione dei problemi:** concedere all&#39;utente l&#39;accesso in Salesforce O disabilitare la registrazione delle attività più recenti per quell&#39;oggetto per quell&#39;utente.

**Errore:** INVALID_FIELD\
**Categoria:** Intermittente\
**Messaggio:** Net::ReadTimeout\
**Cosa sta succedendo:** la richiesta è tempo esaurito. Questo è probabilmente il risultato di troppe transazioni lente.\
**Procedura di risoluzione dei problemi:** rivedere le personalizzazioni esistenti per i potenziali colpevoli dei problemi di latenza e/o disabilitare la registrazione delle attività più recenti per uno o tutti gli oggetti per ridurre il carico.

**Errore:** INVALID_FIELD_FOR_INSERT_UPDATE\
**Categoria:** Accesso/Convalida\
**Messaggio:** Impossibile creare/aggiornare i campi: ToutApp__Tout_Last_Replied__c. Controllare le impostazioni di protezione di questo campo.
**Cosa succede:** Gli utenti non dispongono dell&#39;accesso in scrittura ai campi personalizzati Tout necessari per eseguire la transazione di registrazione delle attività più recenti. È possibile che il team abbia installato il pacchetto ma non abbia attivato i campi corretti per gli utenti.\
**Procedura di risoluzione dei problemi:** Salesforce Admin deve concedere l&#39;accesso ai campi personalizzati OPPURE disattivare la registrazione delle attività più recenti.

**Errore:** INVALID_GRANT\
**Categoria:** Autenticazione\
**Messaggio:** Invalid_Grant: ip con restrizioni\
**Cosa sta succedendo:** Stiamo tentando di accedere alla tua Salesforce, ma hai delle limitazioni IP che ci impediscono di farlo.\
**Procedura di risoluzione dei problemi:** l&#39;amministratore Salesforce dovrà  i nostri IP inserire nell&#39;elenco Consentiti. Per ottenere gli indirizzi IP, gli utenti devono contattare il supporto.

**Errore:** INVALID_TYPE\
**Categoria:** Accesso/Convalida\
**Messaggio:** Data creazione, (SELECT Id FROM Tasks) FROM Lead WHERE Email=&#39;email&#39;^ERROR at Row:1:Column:53sTipo di oggetto &#39;Lead&#39; non è supportato. Se si sta tentando di utilizzare un oggetto personalizzato, assicurarsi di aggiungere il simbolo &#39;__c&#39; dopo il nome dell&#39;entità. Fare riferimento al WSDL o alla chiamata di descrizione per i nomi appropriati
**Cosa sta succedendo:** Stiamo tentando di eseguire una query su un tipo di oggetto da Salesforce a cui l&#39;utente non ha accesso. Ciò è probabilmente correlato al fatto che l&#39;utente non dispone del diritto di accesso all&#39;oggetto lead.\
**Procedura di risoluzione dei problemi:** concedere l&#39;accesso in lettura e aggiornamento all&#39;oggetto Lead in Salesforce oppure disattivare la registrazione delle e-mail e la registrazione delle attività più recenti per i record principali.

**Errore:** QUERY_TIMEOUT\
**Categoria:** Intermittente\
**Messaggio:** La richiesta di query è stata eseguita troppo a lungo\
**Cosa sta succedendo:** Vedere sopra.\
**Procedura di risoluzione dei problemi: la logica** dei tentativi deve gestire questo problema. Se non funziona, chiedi aiuto all&#39;amministratore di Salesforce per risolvere eventuali problemi di attivazione.

**Errore:** REQUEST_LIMIT_EXCEEDED\
**Categoria:** Intermittente\
**Messaggio:**
1 - Limite ConcurrentPerOrgLongTxn superato\
2 - Limite Totale richieste superato\
3 - ConcurrentRequest\
**Cosa accade:**
1 - Limite di richieste simultanee superato, probabilmente a causa di codice di attivazione inefficiente.\
2 - Troppe integrazioni mettono l&#39;organizzazione oltre la finestra 24 ore.\
**Procedura di risoluzione dei problemi:**
1 - Esaminare gli attivatori esistenti sugli oggetti interessati. È possibile disattivare la registrazione rollup per uno o più oggetti.\
2 - Acquista più chiamate API da Salesforce. È possibile disattivare la registrazione rollup per uno o più oggetti.

**Errore:** REQUIRED_FIELD_MISSING\
**Categoria:** Accesso/Convalida\
**Messaggio:Mancano i campi** richiesti:  `[Amount_Committed_Private_Capital__c]`
**Cosa accade:** Questo generalmente accade per la registrazione delle attività più recenti. I campi personalizzati sono stati impostati in modo da essere obbligatori ma contengono valori vuoti. Ciò può accadere se il record è stato creato con un valore vuoto del campo personalizzato e successivamente reso obbligatorio. Il requisito è imposto quando si tenta di aggiornare il record, anche se non si tocca il campo personalizzato.\
**Procedura di risoluzione dei problemi:** aggiornare manualmente i valori dei campi mancanti. Puoi quindi riprovare il messaggio da ToutApp.

**Errore:** SERVER_UNAVAILABLE\
**Categoria:** Intermittente\
**Messaggio:** server troppo occupato\
**Cosa succede:** Problema di prestazioni con Salesforce, probabilmente a causa di attivazioni non ottimali da parte del cliente\
**Procedura di risoluzione dei problemi: la logica** dei tentativi deve gestire questo problema. Se continua a non funzionare, chiedi aiuto all&#39;amministratore di Salesforce per risolvere i problemi relativi a un trigger problematico.

**Errore:** TXN_SECURITY_NO_ACCESS\
**Categoria:** Accesso/Convalida\
**Messaggio:** l&#39;operazione richiesta non è consentita a causa di un criterio di protezione nell&#39;organizzazione. Contattate l’amministratore.<br/>
**Cosa sta succedendo:** È stato configurato un tipo di limite di protezione - consultate https://developer.salesforce.com/forums/?id=&quot;record ID&quot;\
**Procedura di risoluzione dei problemi:** parla con l’amministratore Salesforce e scopri quale potrebbe essere la limitazione specifica.

**Errore:** UNABLE_TO_LOCK_ROW\
**Categoria:** Intermittente\
**Messaggio:** impossibile ottenere l&#39;accesso esclusivo a questo record o a 1 record: &quot;record ID&quot;\
**Cosa accade:** Probabilmente esiste un trigger che sta causando più tentativi di accesso allo stesso record, probabilmente nel caso di un&#39;e-mail di gruppo.\
**Procedura di risoluzione dei problemi: la logica** dei tentativi deve gestire questo problema. Se non funziona, chiedi aiuto all&#39;amministratore di Salesforce per risolvere eventuali problemi di attivazione.

**Errore:** UNKNOWN_EXCEPTION 
**Category:** Altro\
**Messaggio:Eccezione** sconosciuta\
**Cosa succede: eccezione** non gestita in Salesforce.\
**Procedura di risoluzione dei problemi:** archiviare un caso in Salesforce e copiare i valori numerici nel messaggio di errore. Codice Salesforce che non gestisce correttamente un errore.
