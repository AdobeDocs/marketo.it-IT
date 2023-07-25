---
description: Servizio Flusso - Documentazione Marketo - Documentazione del prodotto
title: Servizio passaggio di flusso
exl-id: 81367562-8b27-4ec5-8a9b-b02083a2e999
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1220'
ht-degree: 0%

---

# Servizio passaggio di flusso {#flow-step-service}

Passaggi di flusso self-service è un framework e un set di funzioni per l’authoring, la pubblicazione e l’integrazione di servizi web nelle campagne Adobe Marketo Engage Smart. Questa guida è destinata agli utenti finali del Marketo Engage che desiderano installare e utilizzare servizi già creati e pubblicati. Per informazioni sull’authoring e la pubblicazione del servizio, consulta [Archivio GitHub per l’interfaccia Service Provider](https://github.com/adobe/Marketo-SSFS-Service-Provider-Interface){target="_blank"}. A Proof-of-Concept Lookup Table implementation may be found [here](https://github.com/adobe/mkto-flow-lookup){target="_blank"}.

## Servizi di onboarding e gestione {#onboarding-and-managing-services}

L’installazione di un passaggio di flusso personalizzato richiede le autorizzazioni di amministratore in Marketo (**Gestione webhook** nella versione del 21 gennaio, Modifica nella versione dell’11 marzo). Oltre all’URL di installazione, dopo aver completato l’onboarding iniziale è possibile modificare tutti gli altri aspetti di un servizio servito, espandendo la schermata dei dettagli del servizio dalla griglia dei service provider.

## URL di installazione {#installation-url}

Per iniziare l’installazione, devi prima ottenere l’URL del documento OpenAPI che definisce il servizio. Il provider di servizi dovrebbe essere in grado di fornirtelo e in genere avrà un URL che termina con `/openapi.json`. Gli URL completi avranno un aspetto simile a `https://www.example.com/OpenAPI.json`. Una volta ottenuto questo URL, vai al menu Service Providers (Fornitori di servizi) nella sezione Admin (Amministratore).

Clic **Successivo** per passare alla sezione Immettere le credenziali del servizio.

![](assets/flow-step-service-1.png)

## Immetti credenziali servizio {#enter-service-credentials}

Per accedere al servizio da installare, Marketo deve disporre di credenziali API valide. Queste credenziali devono essere fornite dal provider di servizi. I servizi dispongono di tre diverse opzioni di autenticazione, pertanto è possibile che vengano visualizzate tre diverse richieste di credenziali: **Chiave API** che dispone di un solo campo di input, **Autenticazione di base** che richiede un nome utente e una password e che può anche richiedere un campo denominato Realm, e **OAuth2** utilizzando _Credenziali client_ concessione, che richiede _ID client_ e _Segreto client_.

Quando salvi le credenziali, Marketo tenterà di chiamare l’endpoint di stato del servizio per verificarne la validità. Se le credenziali fornite non sono valide, verrà visualizzato un errore che indica che si tratta di un errore.

## Guida all’onboarding (facoltativo) {#onboarding-guide}

Alcuni provider di servizi includeranno un passaggio facoltativo della Guida all’onboarding. Questo passaggio include eventuali istruzioni aggiuntive per completare l’onboarding del servizio specifiche per quel servizio.

## Mappatura campi {#field-mapping}

Per ricevere o restituire dati da un campo lead specifico, è necessario mappare tale campo. Anche se la mappatura è un passaggio obbligatorio durante l’onboarding, puoi sempre tornare ad alterarla in un secondo momento. Esistono due tipi di mappature configurate in schermate separate: **Campi in uscita**, che vengono inviati al servizio quando Marketo richiama il passaggio di flusso e **Campi in entrata** che sono campi che possono ricevere dati dal servizio quando restituisce dati a Marketo.

>[!NOTE]
>
>Mediante la mappatura di un campo in uscita, si concede a Marketo l&#39;autorizzazione a trasmettere dati da tale campo relativi ai lead elaborati dal servizio associato. Assicurati di avere l’autorità e la legittimazione legali appropriate per trasmettere questi dati al tuo fornitore di servizi, in quanto questi campi possono includere informazioni personali coperte dalle leggi sulla privacy, la protezione e la locazione dei dati.

Le mappature di campo opzionali possono essere disattivate senza interrompere il servizio, ma quelle richieste potrebbero non essere rimosse o disattivate completamente.

## Mappature basate sui servizi {#service-driven-mappings}

I servizi che dispongono di un set fisso di ingressi e uscite, come un passaggio del flusso di registrazione degli eventi, utilizzano **Mappature basate sui servizi**. Per questo tipo di mappatura, il provider di servizi fornirà sia un tipo di dati che un suggerimento sotto forma di un nome API. Se l’hint corrisponde al nome API di un campo lead esistente, tale campo verrà automaticamente popolato nella sezione di mappatura. Per i campi senza un hint corrispondente, è necessario compilare manualmente la mappatura dall’elenco dei campi con il tipo di dati corrispondente. Per completare l’onboarding, è necessario compilare le mappature richieste.

![](assets/flow-step-service-2.png)

## Mappature guidate dall&#39;utente {#user-driven-mappings}

I servizi che non hanno un set fisso di input e output, come un servizio di formattazione della data, utilizzano **Mappature guidate dall&#39;utente**. Ciò significa che ogni campo in entrata e in uscita deve essere configurato da un amministratore.

![](assets/flow-step-service-3.png)

## Campi in uscita {#outgoing-fields}

I campi in uscita sono quelli che vengono inviati al servizio Fase flusso quando quel passaggio di flusso viene utilizzato in una campagna intelligente.

## Campi in entrata {#incoming-fields}

I campi in ingresso sono quelli in cui il servizio Flusso passaggio può scrivere i dati.

## Opzioni di configurazione (facoltativo) {#configuration-options}

Alcuni servizi dispongono di opzioni di configurazione globale facoltative o obbligatorie. Se sono richieste opzioni, prima di salvare o completare l’onboarding è necessario impostare un valore per tutte le opzioni richieste. I parametri i cui nomi sono in corsivo vengono inviati al servizio richiamato come intestazioni.

![](assets/flow-step-service-4.png)

## Ritiro di un servizio {#retiring-a-service}

Per facilitare la transizione a versioni nuove o alternative di un servizio, senza interrompere l’utilizzo attivo, è possibile ritirare i servizi dal menu Service Provider. **Ritiro di un servizio** rimuove il passaggio di flusso corrispondente dalla palette di flusso di Smart Campaign, in modo che non sia possibile crearne di nuovi utilizzi. Nella maggior parte dei casi, quando si sceglie di ritirare un servizio, è necessario disporre di un servizio sostitutivo pronto a sostituire quello esistente.

## Servizio obsoleto {#service-deprecation}

A volte i provider di servizi devono rendere obsoleti i servizi delle fasi di flusso come parte normale del ciclo di vita del software. Quando un provider di servizi annuncia questa situazione, la Data di rimozione e il Messaggio verranno inseriti nella visualizzazione griglia Provider di servizi. Se si continua a utilizzare un servizio che è stato dichiarato obsoleto, è possibile che si verifichino interruzioni del servizio se il servizio non risponde più nel modo previsto o non accetta più le richieste di Marketo Smart Campaigns. Pertanto, è necessario prestare particolare attenzione a tutte le notifiche di obsolescenza del servizio ricevute e adottare le misure appropriate per ritirare o sostituire eventuali passaggi del servizio ancora in uso.

## Utilizzo di passaggi di flusso di terze parti e personalizzati {#using-third-party-and-custom-flow-steps}

Le fasi di flusso installate possono essere utilizzate in gran parte allo stesso modo delle fasi di flusso standard. Tutti i parametri di flusso definiti dal servizio vengono presentati agli utenti finali.

## Aggiornamento degli elenchi di scelta {#refreshing-picklists}

Marketo aggiornerà ogni notte le scelte degli elenchi di selezione per i servizi, ma ci sono momenti in cui dovrai avere nuove scelte disponibili, ad esempio la creazione di campagne. Puoi aggiornarli facilmente da qualsiasi istanza del passaggio del flusso utilizzando il pulsante di aggiornamento oppure andando al menu Admin > Service Providers (Amministratore > Fornitori di servizi) e facendo clic su Refresh Picklist (Aggiorna elenco di selezione) dopo aver selezionato il servizio.

## Controllo dei campi in ingresso {#checking-incoming-fields}

Per verificare quali campi in ingresso sono configurati per un determinato passaggio di flusso, passa il puntatore sull&#39;icona della descrizione comando corrispondente. Questo è utile per determinare quali campi potrebbero cambiare quando un lead vi scorre attraverso, in modo da poter configurare le scelte nei passaggi successivi utilizzando tali campi.

![](assets/flow-step-service-5.png)

## Campi in entrata e modifiche ai valori dei dati {#incoming-fields-and-data-value-changes}

A differenza della maggior parte degli altri passaggi di flusso, quelli implementati con il framework SSFS possono riscrivere i dati nei campi lead mappati da un amministratore e registrare tali modifiche come attività di modifica del valore dei dati.  Quando un passaggio di flusso scrive i dati in questo modo, tutte queste modifiche verranno completate prima che Smart Campaign passi a qualsiasi passaggio successivo, in modo che tutti i dati scritti possano essere utilizzati nelle scelte successive del passaggio di flusso.

## Registri dei servizi e statistiche {#service-logs-and-statistics}

A ciascun servizio Flusso sono associati diversi tipi di registrazione per monitorare lo stato e risolvere eventuali problemi relativi all’integrazione.

## Statistiche servizio {#service-statistics}

Il registro delle statistiche del servizio aggrega i risultati delle chiamate e dei callback per ciascun servizio. Sono raggruppati per ora, livello (blocco o record) e codice e forniscono i conteggi e il messaggio di registro più recente per ogni codice ricevuto. Questo dashboard è progettato principalmente per supportare il monitoraggio dello stato dei servizi.
