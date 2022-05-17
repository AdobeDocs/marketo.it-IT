---
description: Note sulla versione corrente - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione corrente
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: c040d8364bd353e31d26b98284130c22f44b24e8
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Note sulla versione: Maggio 2022 {#release-notes-may-22}

Di seguito sono elencate tutte le funzioni incluse nella versione del 22 maggio. Per informazioni sulla disponibilità delle funzioni, consulta l’edizione del Marketo Engage di Adobe.

>[!AVAILABILITY]
>
>Caratteristiche indicate da una stella (![stella](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

**_Versioni trimestrali_**

Le seguenti funzionalità inizieranno a essere rilasciate il **6 maggio 2022**, con un rollout graduale delle funzioni rimanenti nelle settimane successive (se non specificato diversamente).

## Integrazione CRM nativa {#native-crm-integration}

**[Integrazione CRM nativa Veeva](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target=&quot;_blank&quot;} (disponibilità limitata)**: Migliora il coinvolgimento con i professionisti del settore sanitario sincronizzando l&#39;attività tra Veeva CRM e il Marketo Engage tramite l&#39;integrazione nativa. Questa integrazione consente ai professionisti del marketing di creare esperienze cross-channel più personalizzate e fluide per i professionisti del settore sanitario. Contatta il tuo Customer Success Manager per partecipare.

## Orchestrazione tra canali {#cross-channel-orchestration}

**Eventi Chatbot per chat dinamico**: Utilizza dati di comportamento più dettagliati per i visitatori web, ad esempio il tempo sulla pagina, il tempo sul sito e la percentuale di scorrimento della pagina, per definire quando visualizzare una finestra di dialogo chat.

**Incorpora PDF per chat dinamica**: Aumenta il coinvolgimento e condividi contenuti significativi incorporando PDF nelle finestre di dialogo delle chat e misurando le prestazioni dei contenuti tramite il tracciamento delle attività di coinvolgimento.

**Supporto esteso della lingua per la chat dinamica**: L’interfaccia utente di Chat dinamica sarà ora disponibile anche in francese, tedesco, giapponese, portoghese e spagnolo. Le finestre di dialogo della chat possono essere configurate anche in queste lingue.

**Escludere gli URL per la chat dinamica**: Controlla su quale delle tue pagine web appare la chat dinamica con la possibilità di escludere URL specifici dai criteri di targeting.

**[Miglioramenti al filtro delle attività dei bot e-mail](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target=&quot;_blank&quot;}**: Continua a proteggere lo stato del database con la possibilità di identificare il comportamento di bot in base ai collegamenti nascosti Agenti utente o IP e ai pattern di prossimità, oltre all’identificazione esistente della corrispondenza dell’elenco IAB. Visualizzare gli stati delle attività bot che consentono di comprendere il numero di attività bot identificate per ciascun tipo.

**[Intestazione STS per i collegamenti di tracciamento e-mail](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target=&quot;_blank&quot;}**: Soddisfa le best practice di sicurezza con la possibilità di applicare intestazioni Secure Transport Security per garantire che il traffico verso i collegamenti tracciati sia sempre sicuro.

## Esperienza di nuova generazione {#next-generation-experience}

**Attiva/disattiva switch predefinito per l&#39;esperienza di nuova generazione**: l’interruttore di attivazione/disattivazione sarà predefinito per la nuova esperienza in tutte le schermate in cui è disponibile, facilitando agli utenti la scoperta dei progetti aggiornati e dei miglioramenti all’usabilità.

**Schermata aggiornata nell’esperienza di nuova generazione**:

Nell’esperienza di nuova generazione, offriamo una visualizzazione dei dettagli dei modelli e-mail in Design Studio, che offre miglioramenti aggiornati alla progettazione e all’usabilità accessibili tramite l’interruttore di attivazione/disattivazione.

## Automazione delle esperienze {#experience-automation}

**Passaggi di flusso self-service (versione beta continua)**: Espandi la connettività tra il Marketo Engage e il resto della pila con la possibilità di creare passaggi di flusso personalizzati da utilizzare in Smart Campaigns. Sia gli utenti che i partner di Marketo Engage possono sfruttare questa funzionalità per consentire l’utilizzo di servizi Web esterni nelle campagne trigger, batch ed eseguibili (a differenza dei webhook che possono essere utilizzati solo nelle campagne di attivazione).

## Miglioramenti API {#api-enhancements}

* **Accesso API esteso per sottoscrizioni abilitate per gestione delle relazioni con i clienti**: Stiamo espandendo l’accesso API per gli abbonamenti con una sincronizzazione CRM abilitata per consentire agli utenti di recuperare società, opportunità e persone di vendita dal Marketo Engage.
* **Supporto per tipi di dati &quot;nascosti&quot; in Forms**: Consente di gestire i campi modulo nascosti tramite API.
* **Supporto di più valori di confronto per isNot Form tramite regole**: Gestire la visibilità dei campi modulo in base al fatto che il valore di un altro campo non sia uno dei valori di un elenco specifico.
* **Consenti impostazione di Visualizza e Valori inviati in Seleziona elenchi separatamente**: Impostare separatamente il valore visualizzato e il valore inviato in un campo. Ad esempio, mostrare il nome di un hotel, ma inviare un ID interno al backend.
* **Consenti impostazione di Disattiva tracciamento aperto su Crea o Aggiorna e-mail**: Crea un messaggio e-mail con tracciamento aperto disattivato.

## Annunci {#announcements}

**Verifica e-mail e univocità**: A partire da aprile, inizierà il rollout della verifica e-mail. A quel punto, gli indirizzi e-mail degli utenti di Marketo Engage richiederanno verifica e univocità (questo non si applica agli utenti solo API). Gli utenti autenticati del servizio di directory verificheranno automaticamente le loro e-mail quando la loro sottoscrizione viene abilitata con Verifica e-mail.

La verifica e-mail per gli abbonamenti che utilizzano la funzione &quot;Accesso nella finestra di dialogo per l’invito di utenti&quot; o che hanno un singolo messaggio e-mail associato a più utenti coinciderà con la versione di maggio. Gli abbonamenti con un’unica e-mail associata a più utenti verranno abilitati per Verifica e-mail e richiederanno a tali utenti di risolvere il conflitto e utilizzare un’e-mail univoca per ogni utente. Quando la funzione &quot;Accedi alla finestra di dialogo per l’invito dell’utente&quot; è abilitata, gli utenti invitati tramite questa funzione dovranno disporre di un indirizzo e-mail univoco. Per gli utenti solo API invitati tramite questa funzione, l’indirizzo e-mail non deve essere univoco.

**Modifica del comportamento della cartella archivio**: Con questa versione, la possibilità di creare nuove risorse nelle cartelle Archivia non sarà più disponibile dai menu di scelta rapida della struttura. Le opzioni del menu per la creazione di nuove risorse saranno nascoste per tutte le risorse. [Ulteriori informazioni qui](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target=&quot;_blank&quot;}.

**_Webinar sulla versione del prodotto_**

[Webinar sul rilascio del Marketo Engage di marzo e maggio 2022](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target=&quot;_blank&quot;}
