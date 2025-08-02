---
description: Note sulla versione - Maggio 2022 - Documentazione di Marketo - Documentazione del prodotto
title: Note sulla versione, maggio 2022
exl-id: f591ab95-5ad8-45fa-8c4e-8e42b5d1359a
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# Note sulla versione: maggio 2022 {#release-notes-may-22}

Di seguito sono elencate tutte le funzioni incluse nella versione di maggio 2022. Verifica la disponibilità delle funzioni nella tua edizione di Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![stella](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

**_Versioni trimestrali_**

Le seguenti funzionalità inizieranno a essere rilasciate il **6 maggio 2022**, con un rollout graduale delle funzioni rimanenti nelle settimane successive (salvo diversa indicazione).

## Integrazione CRM nativa {#native-crm-integration}

**[Integrazione nativa di Veeva CRM](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target="_blank"} (disponibilità limitata)**: migliora il coinvolgimento con i professionisti del settore sanitario sincronizzando l&#39;attività tra Veeva CRM e Marketo Engage tramite l&#39;integrazione nativa. Questa integrazione consente agli esperti di marketing di creare esperienze cross-channel più personalizzate e ottimizzate per i professionisti del settore sanitario. Contatta il tuo Customer Success Manager se sei interessato a partecipare.

## Orchestrazione cross-channel {#cross-channel-orchestration}

**Eventi Chatbot per[!DNL Dynamic Chat]**: sfrutta dati di comportamento più dettagliati per i visitatori web, ad esempio il tempo sulla pagina, il tempo sul sito e la percentuale di scorrimento delle pagine, per definire quando visualizzare una finestra di dialogo di chat.

**Incorpora PDF per[!DNL Dynamic Chat]**: aumenta il coinvolgimento e condividi contenuti significativi incorporando PDF nelle finestre di dialogo della chat e misurando le prestazioni dei contenuti tramite il tracciamento delle attività di coinvolgimento.

**Supporto linguistico esteso per[!DNL Dynamic Chat]**: l&#39;interfaccia utente [!DNL Dynamic Chat] sarà ora disponibile anche in francese, tedesco, giapponese, portoghese e spagnolo. È inoltre possibile configurare le finestre di dialogo delle chat in queste lingue.

**Escludi URL per[!DNL Dynamic Chat]**: controlla su quale delle tue pagine Web [!DNL Dynamic Chat] viene visualizzato e puoi escludere URL specifici dai criteri di targeting.

**[Miglioramenti al filtro dell&#39;attività bot e-mail](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}**: continua a proteggere l&#39;integrità del database con la possibilità di identificare il comportamento dei bot in base agli agenti utente o agli IP di collegamento nascosti e ai pattern di prossimità, oltre all&#39;identificazione della corrispondenza nell&#39;elenco IAB esistente. Visualizza gli stati delle attività bot che ti consentono di comprendere il numero di attività bot identificate per ogni tipo.

**[Intestazione STS per i collegamenti di tracciamento e-mail](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target="_blank"}**: soddisfa le best practice di sicurezza con la possibilità di applicare intestazioni di sicurezza trasporto sicuro per garantire che il traffico verso i collegamenti tracciati sia sempre sicuro.

## Esperienza di nuova generazione {#modern-ux}

**Attiva/Disattiva opzione predefinita per Esperienza di nuova generazione**: l&#39;opzione attiva/disattiva verrà impostata come predefinita per la nuova esperienza in tutte le schermate in cui è disponibile, facilitando l&#39;individuazione delle progettazioni aggiornate e dei miglioramenti a livello di usabilità.

**Schermata aggiornata nell&#39;esperienza di nuova generazione**:

Stiamo distribuendo la visualizzazione dei dettagli del modello di e-mail entro [!UICONTROL Design Studio] nell&#39;esperienza di nuova generazione, offrendo una progettazione aggiornata e miglioramenti a livello di usabilità accessibili tramite interruttore.

## Automazione dell’esperienza {#experience-automation}

**Passaggi di flusso self-service (versione beta continua)**: espandi la connettività tra Marketo Engage e il resto dello stack con la possibilità di creare passaggi di flusso personalizzati da utilizzare nelle campagne avanzate. Sia gli utenti che i partner di Marketo Engage possono sfruttare questa funzionalità per consentire l’utilizzo di servizi web esterni nelle campagne trigger, batch ed eseguibili (a differenza dei webhook che possono essere utilizzati solo nelle campagne trigger).

## Miglioramenti API {#api-enhancements}

* **Accesso API espanso per sottoscrizioni abilitate per CRM**: è in corso l&#39;espansione dell&#39;accesso API per sottoscrizioni per cui è abilitata la sincronizzazione CRM per consentire agli utenti di recuperare società, opportunità e venditori da Marketo Engage.
* **Supporto per i tipi di dati &quot;nascosti&quot; in Forms**: consente di gestire i campi modulo nascosti tramite API.
* **Supporto di più valori di confronto per isNot Form tramite regole**: consente di gestire la visibilità dei campi modulo in base al fatto che il valore di un altro campo non sia uno dei valori di un elenco specifico.
* **Consenti l&#39;impostazione dei valori visualizzati e inviati in Seleziona elenchi separatamente**: imposta il valore visualizzato e il valore inviato in un campo separatamente. Ad esempio, mostra il nome di un hotel, ma invia un ID interno al backend.
* **Consenti impostazione di Disabilita tracciamento apertura durante la creazione o l&#39;aggiornamento dell&#39;e-mail**: crea un messaggio e-mail con tracciamento apertura disabilitato.

## Annunci {#announcements}

**Verifica e-mail e univocità**: a partire da aprile, inizierà il rollout della verifica e-mail. A questo punto, gli indirizzi e-mail degli utenti di Marketo Engage richiederanno verifica e univocità (questo non si applica agli utenti solo API). Gli utenti autenticati del servizio directory avranno automaticamente le loro e-mail verificate quando la loro sottoscrizione sarà abilitata con Verifica e-mail.

La verifica e-mail per gli abbonamenti che utilizzano la funzionalità &quot;[!UICONTROL Login in Invite User Dialog]&quot; o che hanno un&#39;unica e-mail associata a più utenti coinciderà con la versione di maggio. Gli abbonamenti con un’unica e-mail associata a più utenti verranno abilitati con Verifica e-mail e richiederanno a tali utenti di risolvere il conflitto e di utilizzare un’e-mail univoca per utente. Quando la funzione &quot;Login in Invite User Dialog&quot; (Consenti di accedere alla finestra di dialogo con l’utente) è abilitata, gli utenti invitati tramite questa funzione dovranno disporre di un indirizzo e-mail univoco. Per gli utenti invitati solo API tramite questa funzione, l’indirizzo e-mail non deve necessariamente essere univoco.

**Modifica del comportamento della cartella di archiviazione**: con questa versione, la possibilità di creare nuove risorse nelle cartelle di archiviazione non sarà più disponibile dai menu di scelta rapida della struttura. Le opzioni di menu per la creazione di nuove risorse saranno nascoste per tutte le risorse. [Ulteriori informazioni](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target="_blank"}.

**_Webinar sulla versione del prodotto_**

[Webinar sulla versione di Marketo Engage di marzo e maggio 2022](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}
