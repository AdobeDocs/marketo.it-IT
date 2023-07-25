---
description: Note sulla versione - Maggio 2022 - Documentazione di Marketo - Documentazione del prodotto
title: Note sulla versione - Maggio 2022
exl-id: f591ab95-5ad8-45fa-8c4e-8e42b5d1359a
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 0%

---

# Note sulla versione: maggio 2022 {#release-notes-may-22}

Di seguito sono elencate tutte le funzioni incluse nella versione di maggio 2022. Verifica la disponibilità delle funzioni nella tua edizione di Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Caratteristiche contrassegnate da una stella (![stella](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

**_Versioni trimestrali_**

Le seguenti funzioni inizieranno ad essere rilasciate il **6 maggio 2022**, con un rollout graduale delle funzioni rimanenti nelle settimane successive (salvo diversa indicazione).

## Integrazione CRM nativa {#native-crm-integration}

**[Integrazione nativa con Veeva CRM](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target="_blank"} (disponibilità limitata)**: migliora il coinvolgimento con i professionisti del settore sanitario sincronizzando l’attività tra Veeva CRM e il Marketo Engage tramite l’integrazione nativa. Questa integrazione consente agli esperti di marketing di creare esperienze cross-channel più personalizzate e ottimizzate per i professionisti del settore sanitario. Se sei interessato a partecipare, contatta l’Adobe Account Team (il tuo Account Manager).

## Orchestrazione cross-channel {#cross-channel-orchestration}

**Eventi Chatbot per il Dynamic Chat**: sfrutta dati di comportamento più dettagliati per i visitatori web, come il tempo sulla pagina, il tempo sul sito e la percentuale di scorrimento delle pagine, per definire quando visualizzare una finestra di dialogo di chat.

**Incorpora PDF per Dynamic Chat**: aumenta il coinvolgimento e condividi contenuti significativi incorporando PDF nelle finestre di dialogo della chat e misurando le prestazioni dei contenuti tramite il tracciamento delle attività di coinvolgimento.

**Supporto linguistico esteso per il Dynamic Chat**: l’interfaccia utente del Dynamic Chat sarà ora disponibile anche in francese, tedesco, giapponese, portoghese e spagnolo. È inoltre possibile configurare le finestre di dialogo delle chat in queste lingue.

**Escludi URL per Dynamic Chat**: controlla su quale Dynamic Chat di pagine web viene visualizzato e puoi escludere URL specifici dai criteri di targeting.

**[Miglioramenti al filtro delle attività bot e-mail](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}**: continua a proteggere lo stato del database con la possibilità di identificare il comportamento dei bot in base agli agenti utente o agli IP di collegamento nascosti e ai pattern di prossimità, oltre a identificare la corrispondenza nell’elenco IAB esistente. Visualizza gli stati delle attività bot che ti consentono di comprendere il numero di attività bot identificate per ogni tipo.

**[Intestazione STS per i collegamenti di tracciamento e-mail](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target="_blank"}**: soddisfa le best practice sulla sicurezza con la possibilità di applicare intestazioni di sicurezza trasporto sicuro per garantire che il traffico dei collegamenti tracciati sia sempre sicuro.

## Esperienza di nuova generazione {#modern-ux}

**Attiva/Disattiva switch predefinito per l&#39;esperienza di nuova generazione**: l’interruttore di attivazione sarà predefinito per la nuova esperienza in tutte le schermate in cui è disponibile, consentendo agli utenti di scoprire più facilmente le progettazioni aggiornate e i miglioramenti a livello di usabilità.

**Schermata aggiornata nell’esperienza di nuova generazione**:

In Design Studio offriamo la visualizzazione dei dettagli dei modelli e-mail nell’esperienza di nuova generazione, con un design aggiornato e miglioramenti a livello di usabilità accessibili tramite interruttore.

## Automazione dell’esperienza {#experience-automation}

**Passaggi del flusso self-service (versione beta continua)**: espandi la connettività tra il Marketo Engage e il resto dello stack con la possibilità di creare passaggi di flusso personalizzati da utilizzare nelle campagne avanzate. Sia gli utenti del Marketo Engage che i partner possono sfruttare questa funzionalità per consentire l’utilizzo di servizi web esterni nelle campagne trigger, batch ed eseguibili (a differenza dei webhook che possono essere utilizzati solo nelle campagne trigger).

## Miglioramenti API {#api-enhancements}

* **Accesso API espanso per sottoscrizioni abilitate per CRM**: stiamo espandendo l’accesso API per gli abbonamenti che dispongono di una sincronizzazione CRM abilitata per consentire agli utenti di recuperare Aziende, Opportunità e Agenti di vendita dal Marketo Engage.
* **Supporto per i tipi di dati &quot;nascosti&quot; in Forms**: consente di gestire i campi modulo nascosti tramite API.
* **Supporto di più valori di confronto per isNot Form tramite regole**: gestisci la visibilità dei campi modulo in base al fatto che il valore di un altro campo non sia uno dei valori in un determinato elenco.
* **Consenti l&#39;impostazione dei valori di visualizzazione e di invio in Seleziona elenchi separatamente**: imposta il valore visualizzato e il valore inviato in un campo separatamente. Ad esempio, mostra il nome di un hotel, ma invia un ID interno al backend.
* **Consenti impostazione di Disabilita tracciamento apertura al momento della creazione o dell’aggiornamento dell’e-mail**: crea un’e-mail con il tracciamento delle aperture disabilitato.

## Annunci {#announcements}

**Verifica e univocità delle e-mail**: a partire da aprile, inizierà il rollout della verifica e-mail. A questo punto, gli indirizzi e-mail degli utenti del Marketo Engage richiederanno verifica e univocità (questo non si applica agli utenti solo API). Gli utenti autenticati del servizio directory avranno automaticamente le loro e-mail verificate quando la loro sottoscrizione sarà abilitata con Verifica e-mail.

La verifica e-mail per gli abbonamenti tramite la funzione &quot;Accedi alla finestra di dialogo Invita utente&quot; o che hanno una singola e-mail associata a più utenti coinciderà con la versione di maggio. Gli abbonamenti con un’unica e-mail associata a più utenti verranno abilitati con Verifica e-mail e richiederanno a tali utenti di risolvere il conflitto e di utilizzare un’e-mail univoca per utente. Quando la funzione &quot;Login in Invite User Dialog&quot; è abilitata, gli utenti invitati tramite questa funzione dovranno disporre di un indirizzo e-mail univoco. Per gli utenti invitati solo API tramite questa funzione, l’indirizzo e-mail non deve necessariamente essere univoco.

**Modifica comportamento cartella archivio**: con questa versione, la possibilità di creare nuove risorse nelle cartelle Archivio non sarà più disponibile dai menu di scelta rapida delle strutture. Le opzioni di menu per la creazione di nuove risorse saranno nascoste per tutte le risorse. [Fai clic qui per ulteriori informazioni](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target="_blank"}.

**_Webinar sulla versione del prodotto_**

[Webinar sulla versione del Marketo Engage di marzo e maggio 2022](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}
