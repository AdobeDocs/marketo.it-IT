---
description: Diagnostica Salesforce - Documenti Marketo - Documentazione del prodotto
title: Diagnostica Salesforce
hide: true
hidefromtoc: true
source-git-commit: 94f89e64b69d3997effe6736241a68f8314db1e6
workflow-type: tm+mt
source-wordcount: '1445'
ht-degree: 0%

---

# Diagnostica Salesforce {#salesforce-diagnostics}

Parte della nostra integrazione Salesforce include una pagina Diagnostica Salesforce all&#39;interno dell&#39;applicazione web. Questa pagina acquisisce gli errori dalla registrazione dei dati non riuscita a Salesforce. Gli errori possono essere utili, ma non sempre leggibili. Come tale, abbiamo messo insieme un foglio di imbroglio che aiuta a spiegare i messaggi di errore.

## Diagnostica accesso {#access-diagnostics}

1. Fai clic sull’icona a forma di ingranaggio e scegli **Impostazioni**.

   ![](assets/salesforce-diagnostics-1.png)

1. In Integrazioni, fai clic su **Diagnostica**.

   ![](assets/salesforce-diagnostics-2.png)

## Foglio di riferimento errori {#error-cheat-sheet}

**Errore:** API_CURRENTLY_DISABLED\
**Categoria:** Accesso/Convalida\
**Messaggio:** API disabilitata per questo utente\
**Cosa succede:** L&#39;utente non ha accesso API\
**Passaggi per la risoluzione dei problemi:** L’amministratore di Salesforce deve concedere all’utente l’accesso API.

**Errore:** AUTHENTICATION_FAILURE\
**Categoria:** Autenticazione\
**Messaggio:** non valido_Grant: errore di autenticazione\
**Cosa succede:** Autenticazione non riuscita\
**Passaggi per la risoluzione dei problemi:** Disconnettiti da Salesforce e quindi riconnettiti.

**Errore:** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY\
**Categoria:** Accesso/Convalida\
**Messaggio:** {&quot;errorCode&quot;:&quot;INVALID_SESSION_ID&quot;,&quot;message&quot;:&quot;Sessione scaduta o non valida&quot;}\
**Cosa succede:**

1 - Il codice del trigger causa un errore di aggiornamento.\
2 - L&#39;utente non dispone di autorizzazioni di scrittura a livello di oggetto per l&#39;oggetto specificato.

**Passaggi per la risoluzione dei problemi:**

1 - Errore del trigger di revisione.\
2 - Concedere l&#39;accesso in scrittura all&#39;utente per l&#39;oggetto OPPURE disabilitare la funzione che sta tentando di scrivere sull&#39;oggetto.

**Errore:** CANNOT_UPDATE_CONVERTED_LEAD\
**Categoria:** Altro\
**Messaggio:** impossibile fare riferimento al lead convertito\
**Cosa succede:** Stiamo tentando di accedere a un lead convertito durante la registrazione attività più recente per contatti e lead. Ho visto anche un paio di questi per le piazzole.\
**Passaggi per la risoluzione dei problemi:** Segnala eventuali casi al nostro [team di supporto](https://nation.marketo.com/t5/Support/ct-p/Support).

**Errore:** ENTITY_IS_LOCKED\
**Categoria:** Accesso/Convalida\
**Messaggio:** l’entità è bloccata per la modifica\
**Cosa succede:** Il record si trova in un processo di approvazione in cui viene bloccato da qualsiasi modifica aggiuntiva fino a quando non viene approvato o negato da una persona che possiede l’approvazione.\
**Passaggi per la risoluzione dei problemi:** Vedi sopra.

**Errore:** EXPIRED_ACCESS
**Categoria:** Autenticazione
**Messaggio:** non valido_Grant: token di accesso/aggiornamento scaduto
**Cosa succede:** Il token di accesso o aggiornamento è scaduto. I token scadono in base a [impostazioni delle sessioni a Salesforce](https://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via).
**Passaggi per la risoluzione dei problemi:** Dovrai ripetere l&#39;autenticazione. Disconnettere la connessione Salesforce e riconnettersi.

**Errore:** FAILED_WRITE\
**Categoria:** Intermittente\
**Messaggio:** fine del file raggiunta\
**Cosa succede:** Problema di prestazioni con Salesforce, probabilmente a causa di trigger non ottimali sul lato cliente.\
**Passaggi per la risoluzione dei problemi:** La logica dei tentativi deve gestire questo problema. Se non funziona ancora, collabora con il tuo amministratore Salesforce per risolvere i problemi di un trigger problematico.

**Errore:** FIELD_CUSTOM_VALIDATION_EXCEPTION
**Categoria:** Accesso/Convalida
**Messaggio:** Varia da cliente a cliente.
**Cosa succede:** Non è stata eseguita una regola di convalida personalizzata per l&#39;oggetto.
**Passaggi per la risoluzione dei problemi:** Controlla la regola di convalida personalizzata che sta causando questo errore. Poiché si tratta di una regola personalizzata, l’errore deve essere risolto una volta sola.

**Errore:** FIELD_FILTER_VALIDATION_EXCEPTION\
**Categoria:** Accesso/Convalida\
**Messaggio:** Il valore non esiste o non corrisponde ai criteri del filtro\
**Cosa succede:** I dati errati esistenti in Salesforce vengono applicati al momento dell’aggiornamento.\
**Passaggi per la risoluzione dei problemi:** Vedi sopra.

**Errore:** FIELD_INTEGRITY_EXCEPTION\
**Categoria:** Accesso/Convalida\
**Messaggio:** Il paese/territorio esistente non riconosce il valore dello stato per il campo: Codice di stato/provincia\
**Cosa succede:** I dati errati esistenti in Salesforce vengono applicati al momento dell’aggiornamento.\
**Passaggi per la risoluzione dei problemi:** Vedi sopra.

**Errore:** INACTIVE_ORGANIZATION\
**Categoria:** Autenticazione\
**Messaggio:** non valido_Grant: organizzazione inattiva\
**Cosa succede:** La tua organizzazione Salesforce non è più attiva.
**Passaggi per la risoluzione dei problemi:** Disconnettiti e riconnettiti da Salesforce.

**Errore:** INACTIVE_USER
**Categoria:** Autenticazione
**Messaggio:** non valido_Grant: utente inattivo
**Cosa succede:** L&#39;utente Salesforce non è più attivo
**Passaggi per la risoluzione dei problemi:** Disconnettiti e riconnettiti da Salesforce.

**Errore:** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MAINTENANCE\
**Categoria:** Intermittente\
**Messaggio:** (nessun messaggio aggiuntivo)\
**Cosa succede:** L&#39;istanza Salesforce è in modalità di manutenzione.\
**Passaggi per la risoluzione dei problemi:** Attendi che la manutenzione del sistema venga eseguita, quindi riprova la registrazione.

**Errore:** INSUFFICIENT_ACCESS_ON_CROSS_REFERENCE_ENTITY
**Categoria:** Accesso/Convalida
**Messaggio:** diritti di accesso insufficienti sull&#39;ID oggetto
**Cosa succede:** Nessun accesso al record padre per un&#39;attività.
**Passaggi per la risoluzione dei problemi:** Vedi sopra.

**Errore:** INSUFFICIENT_ACCESS_OR_READONLY\
**Categoria:** Accesso/Convalida
**Messaggio:** diritti di accesso insufficienti sull&#39;ID oggetto
**Cosa succede:** La registrazione dell&#39;attività più recente non può modificare il record specifico perché l&#39;utente non ha accesso in scrittura.\
**Passaggi per la risoluzione dei problemi:** Concedi all&#39;utente l&#39;accesso in Salesforce O disabilita la registrazione dell&#39;attività più recente per quell&#39;oggetto per quell&#39;utente.

**Errore:** INVALID_FIELD\
**Categoria:** Intermittente\
**Messaggio:** Net::ReadTimeout\
**Cosa succede:** Timeout della richiesta. Questo è probabilmente il risultato di troppe transazioni lente.\
**Passaggi per la risoluzione dei problemi:** Rivedi le personalizzazioni esistenti per individuare potenziali colpevoli dei problemi di latenza e/o disabilita la registrazione delle attività più recenti per uno o tutti gli oggetti per ridurre il carico.

**Errore:** INVALID_FIELD_FOR_INSERT_UPDATE\
**Categoria:** Accesso/Convalida\
**Messaggio:** Impossibile creare/aggiornare i campi: MSE_Replied__c. Controlla le impostazioni di sicurezza di questo campo.
**Cosa succede:** Gli utenti non dispongono dell’accesso in scrittura ai campi personalizzati Azioni di Insight vendite necessari per eseguire la transazione di registrazione delle attività più recenti. È possibile che il team abbia installato il pacchetto ma non abbia attivato i campi corretti per gli utenti.\
**Passaggi per la risoluzione dei problemi:** L’amministratore di Salesforce deve concedere l’accesso ai campi personalizzati OPPURE disattivare la registrazione dell’attività più recente.

**Errore:** INVALID_GRANT\
**Categoria:** Autenticazione\
**Messaggio:** non valido_Grant: ip con restrizioni\
**Cosa succede:** Stiamo cercando di accedere alla tua Salesforce, ma hai delle restrizioni IP in vigore che ci impediscono di farlo.\
**Passaggi per la risoluzione dei problemi:** L’amministratore di Salesforce dovrà inserire nell&#39;elenco Consentiti i nostri IP. Per ottenere gli indirizzi IP, gli utenti devono contattare il supporto .

**Errore:** INVALID_TYPE\
**Categoria:** Accesso/Convalida\
**Messaggio:** CreatedDate, (SELECT Id FROM Tasks) FROM Lead WHERE Email=&#39;email&#39;^ERROR at Row:1:Colonna:53sTipo di oggetto &quot;Lead&quot; non supportato. Se si sta tentando di utilizzare un oggetto personalizzato, assicurarsi di aggiungere &#39;__c&#39; dopo il nome dell&#39;entità. Fai riferimento alla tua WSDL o alla chiamata di descrizione per i nomi appropriati
**Cosa succede:** Stiamo tentando di eseguire una query su un tipo di oggetto da Salesforce a cui l&#39;utente non ha accesso. Questo è probabilmente correlato all’utente che non ha il diritto di accesso all’oggetto lead.\
**Passaggi per la risoluzione dei problemi:** Concedere l’accesso in lettura e aggiornamento all’oggetto Lead in Salesforce oppure disattivare la registrazione delle e-mail e la registrazione delle attività più recenti per i record principali.

**Errore:** QUERY_TIMEOUT\
**Categoria:** Intermittente\
**Messaggio:** La richiesta di query è troppo lunga\
**Cosa succede:** Vedi sopra.\
**Passaggi per la risoluzione dei problemi:** La logica dei tentativi deve gestire questo problema. Se non funziona ancora, collabora con il tuo amministratore Salesforce per risolvere i problemi di un trigger problematico.

**Errore:** REQUEST_LIMIT_EXCEEDED\
**Categoria:** Intermittente\
**Messaggio:**
1 - Limite ConcurrentPerOrgLongTxn superato\
2 - Limite Totale richieste superato\
3 - ConcurrentRequest\
**Cosa succede:**
1 - Limite di richiesta simultanea superato, probabilmente a causa di codice trigger inefficiente.\
2 - Troppe integrazioni posizionano l’organizzazione oltre la finestra continua di 24 ore.\
**Passaggi per la risoluzione dei problemi:**
1 - Esamina i trigger esistenti sugli oggetti interessati. È possibile disattivare la funzione di registrazione per il rollup per uno o più oggetti.\
2 - Acquista altre chiamate API da Salesforce. È possibile disattivare la funzione di registrazione per il rollup per uno o più oggetti.

**Errore:** REQUIRED_FIELD_MISSING\
**Categoria:** Accesso/Convalida\
**Messaggio:** Mancano i campi obbligatori: `[Amount_Committed_Private_Capital__c]`
**Cosa succede:** Questo accade generalmente per la registrazione delle attività più recenti. I campi personalizzati sono stati impostati come obbligatori ma contengono valori vuoti. Ciò può accadere se il record è stato creato con un valore vuoto del campo personalizzato e successivamente reso obbligatorio. L’obbligo viene imposto quando si tenta di aggiornare il record, anche se non si tocca il campo personalizzato.\
**Passaggi per la risoluzione dei problemi:** Aggiorna manualmente i valori dei campi mancanti. È quindi possibile riprovare il messaggio da Azioni Insight vendite.

**Errore:** SERVER_UNAVAILABLE\
**Categoria:** Intermittente\
**Messaggio:** server troppo occupato\
**Cosa succede:** Problema di prestazioni con Salesforce, probabilmente a causa di attivatori non ottimali da parte del cliente\
**Passaggi per la risoluzione dei problemi:** La logica dei tentativi deve gestire questo problema. Se non funziona ancora, collabora con il tuo amministratore Salesforce per risolvere i problemi relativi a un trigger problematico.

**Errore:** TXN_SECURITY_NO_ACCESS\
**Categoria:** Accesso/Convalida\
**Messaggio:** L&#39;operazione richiesta non è consentita a causa di un criterio di sicurezza nell&#39;organizzazione. Contattare l&#39;amministratore.
**Cosa succede:** È stato impostato un qualche tipo di restrizione di sicurezza - vedi https://developer.salesforce.com/forums/?id=&quot;ID record&quot;\
**Passaggi per la risoluzione dei problemi:** Rivolgiti all’amministratore di Salesforce e scopri quale potrebbe essere la restrizione specifica.

**Errore:** UNABLE_TO_LOCK_ROW\
**Categoria:** Intermittente\
**Messaggio:** impossibile ottenere l&#39;accesso esclusivo a questo record o a 1 record: &quot;ID record&quot;\
**Cosa succede:** Probabilmente esiste un trigger che sta causando più tentativi di accedere allo stesso record, probabilmente nel caso di un’e-mail di gruppo.\
**Passaggi per la risoluzione dei problemi:** La logica dei tentativi deve gestire questo problema. Se non funziona ancora, collabora con il tuo amministratore Salesforce per risolvere i problemi di un trigger problematico.

**Errore:** UNKNOWN_EXCEPTION
**Categoria:** Altro\
**Messaggio:** Eccezione sconosciuta\
**Cosa succede:** Eccezione non gestita in Salesforce.\
**Passaggi per la risoluzione dei problemi:** Inserisci un caso con Salesforce e copia i valori numerici nel messaggio di errore. Questo è il codice Salesforce che non gestisce correttamente un errore.
