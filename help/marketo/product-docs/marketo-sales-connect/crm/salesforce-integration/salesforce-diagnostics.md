---
unique-page-id: 14745730
description: Diagnostica Salesforce - Documenti Marketo - Documentazione del prodotto
title: Diagnostica Salesforce
translation-type: tm+mt
source-git-commit: 44ed91b485b52173922c709de63a4353e16c5072
workflow-type: tm+mt
source-wordcount: '1426'
ht-degree: 0%

---


# Diagnostica Salesforce {#salesforce-diagnostics}

Parte della nostra integrazione Salesforce include una pagina Diagnostica Salesforce all&#39;interno dell&#39;applicazione Web. Questa pagina acquisisce gli errori dalla registrazione dei dati non riuscita a Salesforce. Gli errori possono essere utili, ma non sempre leggibili. In quanto tali, abbiamo messo insieme un foglio di imbroglio che aiuta a spiegare i messaggi di errore.

**Errore:** API_CURRENTLY_DISABLED\
**Categoria:** Accesso/Convalida\
**Messaggio:** API disabilitata per questo utente\
**Cosa sta succedendo:** L&#39;utente non dispone dell&#39;accesso API\
**Procedura di risoluzione dei problemi:** L&#39;amministratore di Salesforce deve concedere all&#39;utente l&#39;accesso API.

<br> 

**Errore:** AUTHENTICATION_FAILURE\
**Categoria:** Autenticazione\
**Messaggio:** invalid_Grant: errore di autenticazione\
**Cosa sta succedendo:** Autenticazione non riuscita\
**Procedura di risoluzione dei problemi:** Disconnettetevi da Salesforce e quindi riconnettetevi.

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
**Cosa sta succedendo:** Stiamo tentando di eseguire il login a un lead convertito durante la registrazione delle attività più recenti per contatti e lead. Ho visto anche un paio di questi per le piazzole.\
**Procedura di risoluzione dei problemi:** Segnalare eventuali casi al nostro team [di](http://nation.marketo.com/community/support_solutions)supporto.

<br> 

**Errore:** ENTITY_IS_LOCKED\
**Categoria:** Accesso/Convalida\
**Messaggio:** l&#39;entità è bloccata per la modifica\
**Cosa sta succedendo:** Il record è in un processo di approvazione in cui viene bloccato da qualsiasi modifica aggiuntiva fino a quando non viene approvato o rifiutato da una persona proprietaria dell&#39;approvazione.\
**Procedura di risoluzione dei problemi:** Vedere sopra.

<br> 

**Errore:** EXPIRED_ACCESS **Category:** Messaggio di autenticazione **:** invalid_Grant: token **di accesso/aggiornamento scadutoCosa succede:** Il token di accesso o aggiornamento è scaduto. I token scadono in base alle impostazioni [della sessione in Salesforce](http://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via).
**Procedura di risoluzione dei problemi:** Dovrai autenticarti di nuovo. Disconnetti la connessione Salesforce e ricollega.

<br> 

**Errore:** FAILED_WRITE\
**Categoria:** Intermittente\
**Messaggio:** fine del file raggiunto\
**Cosa sta succedendo:** Problema di prestazioni con Salesforce, probabilmente a causa di attivatori non ottimali dal lato del cliente.\
**Procedura di risoluzione dei problemi:** La logica dei tentativi deve gestire questo problema. Se non funziona, chiedi all’amministratore di Salesforce di risolvere eventuali problemi di attivazione.

<br> 

**Errore:** FIELD_CUSTOM_VALIDATION_EXCEPTION **Category:** Messaggio di accesso/convalida **:** Varia da cliente a cliente.
**Cosa sta succedendo:** Non è riuscita una regola di convalida personalizzata per l&#39;oggetto.
**Procedura di risoluzione dei problemi:** Controllare la regola di convalida personalizzata che causa l&#39;errore. Poiché si tratta di una regola personalizzata, l&#39;errore deve essere risolto una tantum.

<br> 

**Errore:** FIELD_FILTER_VALIDATION_EXCEPTION\
**Categoria:** Accesso/Convalida\
**Messaggio:** Il valore non esiste o non corrisponde ai criteri del filtro\
**Cosa sta succedendo:** I dati errati esistenti in Salesforce vengono applicati al momento dell&#39;aggiornamento.\
**Procedura di risoluzione dei problemi:** Vedere sopra.

<br> 

**Errore:** FIELD_INTEGRITY_EXCEPTION\
**Categoria:** Accesso/Convalida\
**Messaggio:** Il paese/territorio esistente non riconosce il valore dello stato per il campo: Codice stato/provincia\
**Cosa sta succedendo:** I dati errati esistenti in Salesforce vengono applicati al momento dell&#39;aggiornamento.\
**Procedura di risoluzione dei problemi:** Vedere sopra.

<br> 

**Errore:** INACTIVE_ORGANIZATION\
**Categoria:** Autenticazione\
**Messaggio:** invalid_Grant: organizzazione inattiva\
**Cosa sta succedendo:** La tua organizzazione Salesforce non è più attiva.\
**Procedura di risoluzione dei problemi:** Disconnettiti, quindi ricollega da Salesforce.

**Errore:** INACTIVE_USER **Category:** Messaggio di autenticazione **:** invalid_Grant: utente **inattivo Cosa accade:** L&#39;utente Salesforce non è più attivo **per la risoluzione dei problemi:** Disconnettiti, quindi ricollega da Salesforce.

**Errore:** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MAINTENANCE\
**Categoria:** Intermittente\
**Messaggio:** (nessun messaggio aggiuntivo)\
**Cosa sta succedendo:** L&#39;istanza Salesforce è in modalità di manutenzione.\
**Procedura di risoluzione dei problemi:** Attendete che la manutenzione del sistema sia completata, quindi riprovate a registrare.

**Errore:** INSUFFICIENT_ACCESS_ON_CROSS_REFERENCE_ENTITY **Categoria:** Messaggio di accesso/convalida **:** diritti di accesso insufficienti sull&#39;ID **oggetto In corso:** Nessun accesso al record padre per un&#39;attività.
**Procedura di risoluzione dei problemi:** Vedere sopra.

<br> 

**Errore:** INSUFFICIENT_ACCESS_OR_READONLY\
**Categoria:** Accesso/Convalida** ****Messaggio:** diritti di accesso insufficienti sull&#39;ID oggetto** ****Cosa sta succedendo:** La registrazione delle attività più recenti non può modificare il record specifico perché l&#39;utente non ha accesso in scrittura.\
**Procedura di risoluzione dei problemi:** Concedere all&#39;utente l&#39;accesso in Salesforce OPPURE disabilitare la registrazione delle attività più recenti per quell&#39;oggetto per quell&#39;utente.

**Errore:** INVALID_FIELD\
**Categoria:** Intermittente\
**Messaggio:** Net::ReadTimeout\
**Cosa sta succedendo:** La richiesta è timeout. Questo è probabilmente il risultato di troppe transazioni lente.\
**Procedura di risoluzione dei problemi:** Rivedete le personalizzazioni esistenti per i potenziali colpevoli dei problemi di latenza e/o disattivate la registrazione delle attività più recenti per uno o tutti gli oggetti per ridurre il carico.

**Errore:** INVALID_FIELD_FOR_INSERT_UPDATE\
**Categoria:** Accesso/Convalida\
**Messaggio:** Impossibile creare/aggiornare i campi: ToutApp__Tout_Last_Replied__c. Controllare le impostazioni di protezione di questo campo.\
**Cosa sta succedendo:** Gli utenti non dispongono dell&#39;accesso in scrittura ai campi personalizzati Tout necessari per eseguire la transazione di registrazione delle attività più recenti. È possibile che il team abbia installato il pacchetto ma non abbia attivato i campi corretti per gli utenti.\
**Procedura di risoluzione dei problemi:** L&#39;amministratore di Salesforce deve concedere l&#39;accesso ai campi personalizzati OPPURE disattivare la registrazione delle attività più recenti.

**Errore:** INVALID_GRANT\
**Categoria:** Autenticazione\
**Messaggio:** invalid_Grant: ip con restrizioni\
**Cosa sta succedendo:** Stiamo tentando di accedere alla tua Salesforce, ma hai già delle limitazioni IP che ci impediscono di farlo.\
**Procedura di risoluzione dei problemi:** L&#39;amministratore di Salesforce dovrà  i nostri IP. Per ottenere gli indirizzi IP, gli utenti devono contattare il supporto.

**Errore:** INVALID_TYPE\
**Categoria:** Accesso/Convalida\
**Messaggio:** Data creazione, (SELECT Id FROM Tasks) FROM Lead WHERE Email=&#39;email&#39;^ERROR at Row:1:Column:53sTipo di oggetto &#39;Lead&#39; non è supportato. Se si sta tentando di utilizzare un oggetto personalizzato, assicurarsi di aggiungere il simbolo &#39;__c&#39; dopo il nome dell&#39;entità. Fare riferimento al WSDL o alla chiamata di descrizione per i nomi appropriati\
**Cosa sta succedendo:** Stiamo tentando di eseguire una query su un tipo di oggetto da Salesforce a cui l&#39;utente non ha accesso. Ciò è probabilmente correlato al fatto che l&#39;utente non dispone del diritto di accesso all&#39;oggetto lead.\
**Procedura di risoluzione dei problemi:** Concedere l&#39;accesso in lettura e aggiornamento all&#39;oggetto Lead in Salesforce oppure disattivare la registrazione delle e-mail e la registrazione delle attività più recenti per i record principali.

**Errore:** QUERY_TIMEOUT\
**Categoria:** Intermittente\
**Messaggio:** La richiesta di query è stata eseguita troppo a lungo\
**Cosa sta succedendo:** Vedere sopra.\
**Procedura di risoluzione dei problemi:** La logica dei tentativi deve gestire questo problema. Se non funziona, chiedi aiuto all&#39;amministratore di Salesforce per risolvere eventuali problemi di attivazione.

**Errore:** REQUEST_LIMIT_EXCEEDED\
**Categoria:** Intermittente\
**Messaggio:**
1 - Limite ConcurrentPerOrgLongTxn superato\
2 - Limite Totale richieste superato\
3 - ConcurrentRequest\
**Cosa sta succedendo:**
1 - Limite di richieste simultanee superato, probabilmente a causa di codice di attivazione inefficiente.\
2 - Troppe integrazioni mettono l&#39;organizzazione oltre la finestra 24 ore.\
**Procedura di risoluzione dei problemi:**
1 - Esaminare i trigger esistenti sugli oggetti interessati. È possibile disattivare la registrazione rollup per uno o più oggetti.\
2 - Acquista più chiamate API da Salesforce. È possibile disattivare la registrazione rollup per uno o più oggetti.

**Errore:** REQUIRED_FIELD_MISSING\
**Categoria:** Accesso/Convalida\
**Messaggio:** Campi obbligatori mancanti: [Amount_Impegnated_Private_Capital_c]\
**Cosa sta succedendo:** Ciò si verifica generalmente per la registrazione delle attività più recenti. I campi personalizzati sono stati impostati in modo da essere obbligatori ma contengono valori vuoti. Ciò può accadere se il record è stato creato con un valore vuoto del campo personalizzato e successivamente reso obbligatorio. Il requisito è imposto quando si tenta di aggiornare il record, anche se non si tocca il campo personalizzato.\
**Procedura di risoluzione dei problemi:** Aggiornare manualmente i valori dei campi mancanti. Puoi quindi riprovare il messaggio da ToutApp.

**Errore:** SERVER_UNAVAILABLE\
**Categoria:** Intermittente\
**Messaggio:** server troppo occupato\
**Cosa sta succedendo:** Problema di prestazioni con Salesforce, probabilmente a causa di attivatori non ottimali da parte del cliente\
**Procedura di risoluzione dei problemi:** La logica dei tentativi deve gestire questo problema. Se continua a non funzionare, chiedi aiuto all&#39;amministratore di Salesforce per risolvere i problemi relativi a un trigger problematico.

**Errore:** TXN_SECURITY_NO_ACCESS\
**Categoria:** Accesso/Convalida\
**Messaggio:** L&#39;operazione richiesta non è consentita a causa di un criterio di protezione nell&#39;organizzazione. Contattate l’amministratore.\
**Cosa sta succedendo:** È stato configurato un tipo di restrizione di sicurezza - vedi `https://developer.salesforce.com/forums/?id="record` ID&quot;\
**Procedura di risoluzione dei problemi:** Parla con il tuo amministratore Salesforce e scopri quale potrebbe essere la restrizione specifica.

**Errore:** UNABLE_TO_LOCK_ROW\
**Categoria:** Intermittente\
**Messaggio:** impossibile ottenere l&#39;accesso esclusivo a questo record o a 1 record: &quot;record ID&quot;\
**Cosa sta succedendo:** È probabile che si verifichi un trigger che sta causando più tentativi di accesso allo stesso record, probabilmente nel caso di un&#39;e-mail di gruppo.\
**Procedura di risoluzione dei problemi:** La logica dei tentativi deve gestire questo problema. Se non funziona, chiedi aiuto all&#39;amministratore di Salesforce per risolvere eventuali problemi di attivazione.

**Errore:** UNKNOWN_EXCEPTION\
**Categoria:** Altro\
**Messaggio:** Eccezione sconosciuta\
**Cosa sta succedendo:** Eccezione non gestita in Salesforce.\
**Procedura di risoluzione dei problemi:** Archiviare un caso con Salesforce e copiare i valori numerici nel messaggio di errore. Codice Salesforce che non gestisce correttamente un errore.
