---
title: 2022
description: 2022 - Documentazione di Marketo - Documentazione del prodotto
feature: Release Information
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: b0bb9048-d951-48d8-8232-45cf248a7e27id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: d65b4a73-87a3-4d56-b638-74e74d9939ceid: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: ea90ebee-5c84-42d9-8b21-006bdabc95a3id: f71e690b-4480-4b67-9ef5-88f42f9cdfdbid: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2: id: ad89fb33-8541-4339-afe7-bb13d1633714id: d0251300-e25f-466f-9856-7e11ce8fa7aaid: efc9a24a-a6a4-449d-a3e6-44f6c74dfd46
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adebid: d095671a-1355-40aa-8b5f-06c33c68080bid: e1e0219c-f879-479f-8427-888ed2a6e9c2id: eddd9b14-83bd-4ff4-9072-54a4a484abb7id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 1e70b9383bf3a1cd30715df4379d440c4efb1abd
workflow-type: tm+mt
source-wordcount: 4254
ht-degree: 6%

---

# 2022

## Gennaio 2022 {#january}

Le seguenti funzioni sono incluse nella versione di gennaio 2022. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![star](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

**_Versioni trimestrali_**

Le seguenti funzionalità inizieranno a essere rilasciate il **21 gennaio 2022**, con un rollout graduale di ogni funzionalità nelle settimane successive (salvo diversa indicazione).

## Esperienza di nuova generazione

* **Screens aggiornato nell&#39;esperienza di nuova generazione**: verranno forniti schermi aggiuntivi e aggiornati nell&#39;esperienza di nuova generazione che offrono una progettazione aggiornata e miglioramenti a livello di usabilità accessibili tramite l&#39;interruttore:

   * Dettagli risorsa pagina di destinazione in [!UICONTROL Design Studio]
   * Dettagli risorsa pagina di destinazione in [!UICONTROL Marketing Activities]

## Integrazione di [!DNL Microsoft Dynamics] {#microsoft-dynamics-integration}

* **Sincronizzazione del tipo di campo Multiselect Optionset generalmente disponibile**: sincronizza il tipo di campo Multiselect Optionset da [!DNL Microsoft Dynamics] per sfruttare in elenchi avanzati e campagne avanzate per un targeting più granulare del pubblico. Alcuni esempi includono: argomenti/prodotti di interesse, modalità di comunicazione preferite e altro ancora. Questa nuova sincronizzazione è disponibile per [!DNL Microsoft Dynamics] versione 9.X (incluso Dynamics 365 Online).

* **Autenticazione da server a server per[!DNL Microsoft Dynamics 365 Online]**: per una maggiore sicurezza, ora supporteremo Server to Server (S2S) come modalità di autenticazione aggiuntiva per l&#39;utente di sincronizzazione Marketo Engage su Azure Active Directory per l&#39;accesso non interattivo a [!DNL Microsoft Dynamics 365 Online]. Questo ti consente di utilizzare l’autenticazione a più fattori, in quanto tutte le autenticazioni e gli accessi saranno basati su OAuth (solo ID client e segreto client).

>[!NOTE]
>
>La modalità S2S si basa sull&#39;utente dell&#39;applicazione anziché sull&#39;utente con licenza, che consente di risparmiare l&#39;uso di una licenza aggiuntiva.

## Amministrazione {#administration}

* **[Regole di convalida modulo](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**: consente di mantenere l&#39;integrità del database con la possibilità di impedire l&#39;invio di Marketo Engage Form a domini e-mail problematici o indesiderati. Il pannello Regola di convalida modulo globale consente agli amministratori di definire un inserisco nell&#39;elenco Bloccati di o di abilitare un elenco predefinito di domini consumer liberi da bloccare dai moduli.

* **[Sicurezza intestazione pagina di destinazione](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**: gli amministratori possono gestire intestazioni Strict Transport Security e X-Frame Options nei domini delle pagine di destinazione per applicare requisiti di sicurezza elevati.

**_Rilascio nel corso del trimestre_**

Le seguenti funzioni sono in un ciclo non trimestrale e verranno rilasciate nei prossimi mesi.

## Connettore di destinazione Marketo Engage per AEP: creazione di nuovi lead {#aep-marketo-engage-destination-connector}

I clienti di Marketo Engage che utilizzano anche Adobe Experience Platform (AEP) possono massimizzare il database con la possibilità di inviare in rete i nuovi record di persone da AEP a Marketo Engage tramite il connettore di destinazione di AEP. Quando si inviano segmenti di pubblico da AEP a Marketo Engage, è possibile aggiungere automaticamente al segmento persone che non esistono già nel database di Marketo Engage [1.](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md)

## [!DNL Sales Insight]

![(stella)](assets/yellow-star.png)

**[!DNL Sales Insight]per [!DNL Salesforce] CRM**

* **Nuova colonna dei tipi per[!UICONTROL Best Bets]**: i venditori riceveranno informazioni più rapide con una nuova colonna denominata &quot;Tipo&quot; per distinguere i lead dai contatti nella pagina [!UICONTROL Best Bets].

* Aggiornamento API **[!DNL Salesforce]della piattaforma**: in risposta al ritiro di [!DNL Salesforce] delle versioni da 21.0 a 30.0 dell&#39;API della piattaforma [!DNL Salesforce], il pacchetto [!DNL Sales Insight] è stato aggiornato con le API più recenti.

* **Branding aggiornato**: tutte le [!DNL Sales Insight] pagine sono in fase di aggiornamento per l&#39;allineamento con il branding Adobe.

**[!DNL Sales Insight]per[!DNL Microsoft Dynamics]**

* **Layout account aggiornato**: i venditori possono ottenere una visualizzazione collettiva delle attività principali, ad esempio: attività e-mail, attività Web, momenti di interesse e variazioni di punteggio per tutti i contatti all&#39;interno di un account.

## [!DNL Sales Connect]

![(stella)](assets/yellow-star.png)

* **Risultati e motivi della chiamata**: scopri e tieni traccia in modo più dettagliato degli sforzi dei tuoi team di vendita in uscita con nuove opzioni personalizzabili per esito e motivo della chiamata. Oltre a questi nuovi campi, stiamo introducendo una nuova governance per applicare la selezione del motivo e del risultato della chiamata mentre i venditori effettuano chiamate, una nuova governance per abilitare o disabilitare i motivi e i risultati della chiamata e un nuovo campo personalizzato Motivo chiamata e Risultato chiamata [!DNL Salesforce] attività per la registrazione dei dati in [!DNL Salesforce]. [Fai clic qui](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) per ulteriori informazioni.

* Personalizzazione dettagli attività **[!DNL Salesforce]**: acquisisci ulteriori dati attività di vendita e attività in [!DNL Salesforce] personalizzando le informazioni aggiunte al campo dell&#39;oggetto attività [!DNL Salesforce] quando un&#39;attività di vendita viene registrata in [!DNL Salesforce] da [!DNL Sales Connect]. [Fai clic qui](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) per ulteriori informazioni.

## Annunci

* **Deprecazione di Marketo Sky**: a marzo, Marketo Sky non sarà più disponibile, in quanto le nostre risorse saranno concentrate sulla distribuzione dell&#39;esperienza utente di nuova generazione. Nel tentativo di mantenere l’accesso a funzionalità esclusive di Marketo Sky, a marzo le funzioni Scadenza risorse e Sostituzione priorità campagna avanzata saranno integrate nell’esperienza mainstream. [Fai clic qui](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) per ulteriori informazioni.

* **Deprecazione endpoint modulo**: i moduli programmatici POST non supportati per l&#39;endpoint leadCapture/save2 verranno rifiutati da Marketo Engage Form. [Fai clic qui](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) per ulteriori informazioni.

* **Accesso nella finestra di dialogo Invita utente**: a marzo, la funzionalità opzionale esistente &quot;Accesso nella finestra di dialogo Invita utente&quot; diventerà obsoleta. La funzionalità &quot;[!UICONTROL Login in Invite User Dialog]&quot; è sovrascritta dalla funzionalità Universal ID, necessaria per la prossima integrazione di sistema di Adobe Identity Management, ed è stata abilitata ad agosto 2021 per tutte le sottoscrizioni. In seguito alla rimozione di, Marketo Engage forzerà l’associazione di un solo utente per indirizzo e-mail all’interno di un abbonamento.

**Domini Marketo Engage - [!DNL Sales Insight] Configurazione**: per i domini Marketo Engage per i quali non è stato eseguito il provisioning del certificato SSL e https://, le chiamate non riusciranno e verrà restituito un errore di handshake SSL. Pertanto, questi domini saranno ritirati. Di conseguenza, [!DNL Sales Insight] utenti con una configurazione precedente che punta a uno di questi domini potrebbero riscontrare errori di callout di sistema nella pagina Lead, Contatto, Account, Pannelli opportunità o Globale Marketo. Se riscontri questo errore, ti consigliamo di aggiornare la [configurazione di Marketo Engage](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) in [!DNL Salesforce]. È sufficiente aggiornare le credenziali di Marketo Engage evidenziate nella sezione &quot;[!DNL Marketo Sales Insight] Config&quot; del documento.

**_Webinar sulla versione del prodotto_**

[Webinar sulla versione di Marketo Engage di gennaio 2022](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)

## Marzo 2022 {#march}

Le seguenti funzioni sono incluse nella versione di marzo 2022. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![star](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

**_Versioni trimestrali_**

Le seguenti funzionalità inizieranno a essere rilasciate il **11 marzo 2022**, con un rollout graduale di ogni funzionalità nelle settimane successive (se non specificato diversamente).

## Orchestrazione cross-channel

* **[!DNL Dynamic Chat]**: massimizza ogni opportunità sul tuo sito web eseguendo il targeting sia dei lead che degli account con conversazioni proattive, coinvolgenti e 1:1 personalizzate. [Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"} consente agli utenti di Marketo Engage di iniziare a sfruttare le chat come parte chiave delle esperienze cross-channel integrate per i casi di utilizzo di marketing e vendite B2B. Le caratteristiche includono: la possibilità di prenotare le riunioni direttamente all&#39;interno della chat, l&#39;indirizzamento dei lead, modelli di avvio, creazione di conversazioni con trascinamento e molto altro. Dynamic Chat è incluso in tutti i pacchetti Marketo Engage e verrà introdotto quest’anno per tutti gli utenti di Marketo Engage.

* **Miglioramento del filtro dell&#39;attività bot e-mail**: come miglioramento della funzione [Filtro dell&#39;attività bot e-mail](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"} rilasciata in precedenza, ora puoi dare il consenso per la registrazione delle attività identificate come bot. Puoi quindi filtrare e attivare le azioni in base alle attività identificate come eseguite dai bot.

## Esperienza di nuova generazione

* **Screens aggiornato nell&#39;esperienza di nuova generazione**: verranno forniti schermi aggiuntivi e aggiornati nell&#39;esperienza di nuova generazione che offrono una progettazione aggiornata e miglioramenti a livello di usabilità accessibili tramite l&#39;interruttore:

   * Visualizzazione elenco moduli in [!UICONTROL Design Studio] (incluse nuove azioni in blocco)

* **Aggiornamento del flusso di lavoro del programma di importazione**: il flusso di lavoro del programma di importazione viene consegnato nell&#39;esperienza di nuova generazione con una progettazione aggiornata e miglioramenti a livello di usabilità. Si tratta di una modifica automatica senza interruttore.

* **Controllo amministratore per l&#39;interruttore di attivazione dell&#39;esperienza di nuova generazione**: gestisce il rollout dell&#39;esperienza di nuova generazione in modo che funzioni per gli utenti, consentendo agli amministratori di selezionare i tipi di utenti che possono accedere all&#39;interruttore di attivazione.

## Automazione dell’esperienza

* **Passaggi di flusso self-service (Beta)**: espandi la connettività tra Marketo Engage e il resto dello stack con la possibilità di creare passaggi di flusso personalizzati da utilizzare nelle campagne avanzate. Sia gli utenti che i partner di Marketo possono sfruttare questa funzionalità per consentire l’utilizzo di servizi web esterni in campagne batch ed eseguibili, a differenza dei webhook, che possono essere utilizzati solo in campagne trigger.

* **Scadenza risorsa**: mantieni il controllo delle risorse e delle campagne sensibili al tempo con la possibilità di pianificare la loro disattivazione automatica a una data e un&#39;ora specificate nell&#39;esperienza utente classica.

* **Sostituzione priorità campagna avanzata**: assicurati che le campagne avanzate attivino l&#39;alta priorità il prima possibile, con la possibilità di ignorare la classificazione di priorità della campagna standard. È inoltre possibile ridurre la priorità delle campagne intelligenti con trigger a bassa priorità per liberare risorse di elaborazione per altre attività ad alta priorità.

## Miglioramenti API

* **Restituisci lo stato di tracciamento delle e-mail aperte**: consente la lettura dello stato di tracciamento delle e-mail aperte tramite API
* **Recupera righe oggetto contenuto dinamico da e-mail**: consente agli addetti al marketing di eseguire analisi delle righe oggetto dinamiche negli strumenti di business intelligence
* **Campi personalizzati membro del programma CRUD**: consente agli addetti al marketing di creare in modo programmatico campi personalizzati membro del programma
* **Esportazione oggetti personalizzati in blocco aggiornataAl filtro**: consente agli addetti al marketing di sincronizzare in modo programmatico gli oggetti personalizzati
* **Impostazione di avvio automatico esposizione per i programmi e-mail**: consente agli addetti al marketing di configurare programmi e-mail con avvio automatico tramite API
* **Aggiornamento selettivo dei tag del programma**: consente agli addetti al marketing di inviare aggiornamenti selettivi dei tag senza spingere tutti i tag contemporaneamente
* **Campo actionResult estrazione attività in blocco**: consente agli addetti al marketing di identificare le attività ignorate o non riuscite

**_Rilascio nel corso del trimestre_**

Le seguenti funzioni sono in un ciclo non trimestrale e verranno rilasciate nei prossimi mesi.

## [!DNL Bizible] {#bizible}

![(stella)](assets/yellow-star.png)

* **Modelli BI**: [!DNL Bizible] fornirà gli artefatti di report fondamentali e scaricabili e i report di esempio per Tableau e Power BI per consentire lo sviluppo rapido di report personalizzati adatti alle tue esigenze aziendali specifiche.

## [!DNL Sales Connect]

![(stella)](assets/yellow-star.png)

* **Limitazione della connessione e-mail (GA)**: la limitazione della connessione e-mail consente agli amministratori di [!DNL Sales Connect] di configurare la frequenza di invio delle e-mail quando si utilizza Gmail o [!DNL Exchange] come canale di consegna, in modo che la frequenza con cui le e-mail vengono consegnate al provider del canale di consegna non superi i limiti imposti.

## Annunci

* **Deprecazione di Marketo Sky**: a marzo, Marketo Sky non sarà più disponibile, in quanto le nostre risorse saranno concentrate sulla distribuzione dell&#39;esperienza utente di nuova generazione. Nel tentativo di mantenere l’accesso a funzionalità esclusive di Marketo Sky, ora con Asset Expiration e Smart Campaign Priority Override vengono introdotte nell’esperienza classica. [Fai clic qui](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) per ulteriori informazioni.

**_Webinar sulla versione del prodotto_**

[Webinar sulla versione di Marketo Engage di marzo e maggio 2022](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}

## Maggio 2022 {#may}

Di seguito sono elencate tutte le funzioni incluse nella versione di maggio 2022. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![star](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

**_Versioni trimestrali_**

Le seguenti funzionalità inizieranno a essere rilasciate il **6 maggio 2022**, con un rollout graduale delle funzioni rimanenti nelle settimane successive (salvo diversa indicazione).

## Integrazione CRM nativa {#native-crm-integration}

**[Integrazione nativa di Veeva CRM](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target="_blank"} (disponibilità limitata)**: migliora il coinvolgimento con i professionisti del settore sanitario sincronizzando l&#39;attività tra Veeva CRM e Marketo Engage tramite l&#39;integrazione nativa. Questa integrazione consente agli esperti di marketing di creare esperienze cross-channel più personalizzate e ottimizzate per i professionisti del settore sanitario. Se sei interessato a partecipare, contatta il tuo Customer Success Manager.

## Orchestrazione cross-channel

**Eventi Chatbot per[!DNL Dynamic Chat]**: sfrutta dati di comportamento più dettagliati per i visitatori web, ad esempio il tempo sulla pagina, il tempo sul sito e la percentuale di scorrimento delle pagine, per definire quando visualizzare una finestra di dialogo di chat.

**Incorpora PDF per[!DNL Dynamic Chat]**: aumenta il coinvolgimento e condividi contenuti significativi incorporando PDF nelle finestre di dialogo della chat e misurando le prestazioni dei contenuti tramite il tracciamento delle attività di coinvolgimento.

**Supporto linguistico esteso per[!DNL Dynamic Chat]**: l&#39;interfaccia utente [!DNL Dynamic Chat] sarà ora disponibile anche in francese, tedesco, giapponese, portoghese e spagnolo. È inoltre possibile configurare le finestre di dialogo delle chat in queste lingue.

**Escludi URL per[!DNL Dynamic Chat]**: controlla su quale delle tue pagine Web [!DNL Dynamic Chat] viene visualizzato e puoi escludere URL specifici dai criteri di targeting.

**[Miglioramenti al filtro dell&#39;attività bot e-mail](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}**: continua a proteggere l&#39;integrità del database con la possibilità di identificare il comportamento dei bot in base agli agenti utente o agli IP di collegamento nascosti e ai pattern di prossimità, oltre all&#39;identificazione della corrispondenza nell&#39;elenco IAB esistente. Visualizza gli stati delle attività bot che ti consentono di comprendere il numero di attività bot identificate per ogni tipo.

**[Intestazione STS per i collegamenti di tracciamento e-mail](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target="_blank"}**: soddisfa le best practice di sicurezza con la possibilità di applicare intestazioni di sicurezza trasporto sicuro per garantire che il traffico verso i collegamenti tracciati sia sempre sicuro.

## Esperienza di nuova generazione

**Attiva/Disattiva opzione predefinita per Esperienza di nuova generazione**: l&#39;opzione attiva/disattiva verrà impostata come predefinita per la nuova esperienza in tutte le schermate in cui è disponibile, facilitando l&#39;individuazione delle progettazioni aggiornate e dei miglioramenti a livello di usabilità.

**Schermata aggiornata nell&#39;esperienza di nuova generazione**:

Stiamo distribuendo la visualizzazione dei dettagli del modello di e-mail entro [!UICONTROL Design Studio] nell&#39;esperienza di nuova generazione, offrendo una progettazione aggiornata e miglioramenti a livello di usabilità accessibili tramite interruttore.

## Automazione dell’esperienza

**Passaggi di flusso self-service (versione beta continua)**: espandi la connettività tra Marketo Engage e il resto dello stack con la possibilità di creare passaggi di flusso personalizzati da utilizzare nelle campagne avanzate. Sia gli utenti che i partner di Marketo Engage possono sfruttare questa funzionalità per consentire l’utilizzo di servizi web esterni nelle campagne trigger, batch ed eseguibili (a differenza dei webhook che possono essere utilizzati solo nelle campagne trigger).

## Miglioramenti API

* **Accesso API espanso per sottoscrizioni abilitate per CRM**: è in corso l&#39;espansione dell&#39;accesso API per sottoscrizioni per cui è abilitata la sincronizzazione CRM per consentire agli utenti di recuperare società, opportunità e venditori da Marketo Engage.
* **Supporto per i tipi di dati &quot;nascosti&quot; in Forms**: consente di gestire i campi modulo nascosti tramite API.
* **Supporto di più valori di confronto per isNot Form tramite regole**: consente di gestire la visibilità dei campi modulo in base al fatto che il valore di un altro campo non sia uno dei valori di un elenco specifico.
* **Consenti l&#39;impostazione dei valori visualizzati e inviati in Seleziona elenchi separatamente**: imposta il valore visualizzato e il valore inviato in un campo separatamente. Ad esempio, mostra il nome di un hotel, ma invia un ID interno al backend.
* **Consenti impostazione di Disabilita tracciamento apertura durante la creazione o l&#39;aggiornamento dell&#39;e-mail**: crea un messaggio e-mail con tracciamento apertura disabilitato.

## Annunci

**Verifica e-mail e univocità**: a partire da aprile, inizierà il rollout della verifica e-mail. A questo punto, gli indirizzi e-mail degli utenti di Marketo Engage richiederanno verifica e univocità (questo non si applica agli utenti solo API). Gli utenti autenticati del servizio directory avranno automaticamente le loro e-mail verificate quando la loro sottoscrizione sarà abilitata con Verifica e-mail.

La verifica e-mail per gli abbonamenti che utilizzano la funzionalità &quot;[!UICONTROL Login in Invite User Dialog]&quot; o che hanno un&#39;unica e-mail associata a più utenti coinciderà con la versione di maggio. Gli abbonamenti con un’unica e-mail associata a più utenti verranno abilitati con Verifica e-mail e richiederanno a tali utenti di risolvere il conflitto e di utilizzare un’e-mail univoca per utente. Quando la funzione &quot;Login in Invite User Dialog&quot; è abilitata, gli utenti invitati tramite questa funzione dovranno disporre di un indirizzo e-mail univoco. Per gli utenti invitati solo API tramite questa funzione, l’indirizzo e-mail non deve necessariamente essere univoco.

**Modifica del comportamento della cartella di archiviazione**: con questa versione, la possibilità di creare nuove risorse nelle cartelle di archiviazione non sarà più disponibile dai menu di scelta rapida della struttura. Le opzioni di menu per la creazione di nuove risorse saranno nascoste per tutte le risorse. Per ulteriori informazioni, [consulta questo articolo](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target="_blank"}.

**_Webinar sulla versione del prodotto_**

[Webinar sulla versione di Marketo Engage di marzo e maggio 2022](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}

## Giugno 2022 {#june}

Qui sotto troverai tutte le funzioni incluse nella versione di giugno 2022. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![star](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

Le seguenti funzionalità inizieranno a essere rilasciate il **24 giugno 2022**, con un rollout graduale delle funzioni rimanenti nelle settimane successive (salvo diversa indicazione).

## Ambiente dati di marketing

* **Esporre i campi CreatedAt/UpdatedAt per gli oggetti personalizzati**: consente di esaminare questi campi nella schermata Dettagli persona per ottenere ulteriori insight.

## Orchestrazione cross-channel

* **Miglioramento dell&#39;usabilità di Stream Designer per[!DNL Dynamic Chat]**: aggiungere schede direttamente dall&#39;area di lavoro Stream Designer senza dover essere trascinate. È stata migliorata anche l&#39;interfaccia [!DNL Dynamic Chat] per offrire una migliore visibilità dei contenuti nelle singole schede.

* **Regole di routing degli appuntamenti avanzate per[!DNL Dynamic Chat]**: [!DNL Dynamic Chat] offre ulteriori opzioni per il routing degli appuntamenti di destinazione. Specifica gli appuntamenti dell&#39;agente da instradare in base agli attributi Marketo Engage, in modo da garantire che i lead vengano instradati agli agenti appropriati.

* **Generazione rapporti di finestre di dialogo avanzate per[!DNL Dynamic Chat]**: visualizza le prestazioni delle campagne [!DNL Dynamic Chat] in modo più dettagliato utilizzando visualizzazioni di dati completamente nuove per le metriche di coinvolgimento e conversione.

* **Annulla sincronizzazione attributi Marketo Engage inutilizzati per[!DNL Dynamic Chat]**: annulla la sincronizzazione degli attributi Marketo Engage dalla sottoscrizione [!DNL Dynamic Chat] che non vengono utilizzati, per facilitare la pulizia dei dati e consentire la sincronizzazione di attributi alternativi in base alle esigenze.

## Esperienza di nuova generazione

**Nuove visualizzazioni per commutazione**: le visualizzazioni seguenti sono ora disponibili nell&#39;esperienza di nuova generazione:

* [Vista dettagli e-mail](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [Vista elenco e-mail](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## Automazione dell’esperienza

* **Esclusioni regole di convalida campo modulo globale**: escludi moduli specifici dalle regole di convalida modulo globale in modo che i centri sottoscrizioni e altri flussi di lavoro business critical possano accettare tutti i valori.

* **Passaggi di flusso self-service**: espandi la connettività tra Marketo Engage e il resto dello stack con la possibilità di creare passaggi di flusso personalizzati da utilizzare nelle campagne avanzate. Sia gli utenti che i partner di Marketo Engage possono sfruttare questa funzionalità per consentire l’utilizzo di servizi web esterni nelle campagne Trigger, Batch ed Eseguibili, a differenza dei webhook, che possono essere utilizzati solo nelle campagne Trigger.

* **Tracciamento collegamenti agnostici del protocollo di Munchkin**: estendere il supporto per il tracciamento di `tel` e `mailto` collegamenti con Munchkin per tenere traccia di un set esteso di comportamenti Web.

* **Metodi HTTP aggiuntivi per i webhook**: specificare PUT, PATCH e DELETE come tipi di richiesta per interagire con i servizi Web.

## [!DNL Sales Insight]

![(stella)](assets/yellow-star.png)

* Set di autorizzazioni **[!DNL Sales Insight]in[!DNL Salesforce]**: gli amministratori possono fornire l&#39;accesso [!DNL Sales Insight] a un gruppo limitato di persone a livello di utente anziché a livello di profilo tramite il set di autorizzazioni dell&#39;app Marketo, che fa parte del pacchetto [!DNL Sales Insight] [!DNL Salesforce].

* **Aggiornamento sezioni di My Marketo - [!DNL Sales Insight] Azioni**: gli amministratori di Marketo (e gli utenti da essi designati) possono ora passare rapidamente alla propria istanza di [!DNL Sales Insight] azioni tramite una nuova sezione di [!DNL Sales Insight] azioni che si trova nella pagina My Marketo.

## [!DNL Sales Connect]

![(stella)](assets/yellow-star.png)

* Aggiornamento API **[!DNL Salesforce]**: con la versione estiva &#39;22 di [!DNL Salesforce], le versioni legacy API 21 -30 non saranno più supportate da [!DNL Salesforce]. Con questa versione di Marketo Engage, tutte le richieste [!DNL Sales Connect] che utilizzano versioni API legacy sono state aggiornate per rimanere all&#39;interno di una versione supportata. Per informazioni complete sui piani di ritiro API [!DNL Salesforce], fare clic [qui](https://help.salesforce.com/s/articleView?language=en_US&type=1&id=000354473){target="_blank"}.

## Miglioramenti API

* **Nuove funzionalità di filtro per API di estrazione membri programma in blocco**: consente di filtrare in base allo stato di appartenenza al programma, a UpdateAt, alla cadenza o al contenuto esaurito per perfezionare il set di dati estratto.

* **Miglioramento dell&#39;API di estrazione membri programma in blocco**: specificare fino a 10 programmi durante la creazione di processi per migliorare la velocità effettiva.

## Annunci

* **Deprecazione di Forms - Forms 1.0, endpoint di acquisizione/salvataggio lead e versioni senza script dei moduli**: il supporto per le risorse di Forms 1.0 verrà rimosso completamente da Marketo Engage entro ottobre 2022. Tutte le risorse Forms 1.0 esistenti cesseranno di funzionare. Marketo Engage forms richiederà il caricamento di JavaScript su pagine di destinazione e siti Web.

**_Webinar sulla versione del prodotto_**

[Webinar sulla versione di Marketo Engage di giugno e agosto 2022](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}

## Agosto 2022 {#august}

Qui sotto trovi tutte le funzioni incluse nella versione di agosto 2022. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![star](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

Le seguenti funzionalità hanno iniziato un rollout graduale il **26 agosto 2022**.

## Orchestrazione cross-channel

* Attiva/Disattiva tutte le finestre di dialogo pubblicate contemporaneamente per [!DNL Dynamic Chat]**: abilita/disabilita globalmente tutte le finestre di dialogo pubblicate contemporaneamente dalla pagina Configurazione con la pressione di un pulsante.

* **Avatar personalizzati per[!DNL Dynamic Chat]**: carica un avatar chatbot personalizzato che potrà essere personalizzato con il tuo marchio.

* **Trascrizioni chat per[!DNL Dynamic Chat]**: visualizza le trascrizioni chat per ogni conversazione per ottenere insight più approfondito su ciò che ogni visitatore web è interessato.

## Esperienza di nuova generazione

* **Marchio Adobe**: è stato aggiornato l&#39;aspetto degli editor e la pagina dei dettagli della persona con il nuovo marchio Adobe Experience Cloud.

* **Visualizza gerarchia cartelle della cartella di destinazione nella finestra di dialogo Sposta**: la visualizzazione della gerarchia di cartelle per ogni cartella semplifica lo spostamento delle risorse e riduce la probabilità di inserirle nella cartella errata.

* **[Screens aggiornato nell&#39;esperienza di nuova generazione](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md){target="_blank"}**: verranno forniti schermi aggiuntivi e aggiornati nell&#39;esperienza di nuova generazione che offrono una progettazione aggiornata e miglioramenti a livello di usabilità accessibili tramite l&#39;interruttore:

   * Dettagli snippet
   * Dettagli di &quot;Immagini e file&quot;

>[!NOTE]
>
>Si verifica un’eccezione durante lo spostamento di una risorsa in una cartella all’interno di un programma in Attività di marketing. Questa azione di spostamento non consente di visualizzare la gerarchia delle cartelle, poiché le cartelle all&#39;interno di un programma non possono avere nomi duplicati.

## Automazione dell’esperienza

* **[Passaggi di flusso self-service - Miglioramenti dell&#39;importazione dei programmi](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/flow-step-service.md){target="_blank"}**: è stato migliorato il supporto per l&#39;importazione di programmi con passaggi di flusso personalizzati, in cui è ora possibile utilizzare più istanze dello stesso provider di servizi e importare programmi con passaggi di flusso compatibili con tali provider di servizi.

* **[!DNL Munchkin]- Tracciamento collegamenti espansi**: estendere il supporto per il tracciamento di `tel` e `mailto` collegamenti con Munchkin per tenere traccia di un set esteso di comportamenti Web.

* **Visibilità intestazione personalizzata webhook**: le intestazioni personalizzate del webhook sono ora visualizzate nella scheda [!UICONTROL Admin] > [!UICONTROL Webhooks] per una migliore visibilità.

* **CAPTCHA**: valuta la validità degli invii di moduli [utilizzando reCAPTCHA v3](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target="_blank"} per valutare il traffico del modulo in arrivo. Crea flussi di lavoro di marketing per escludere, mettere in quarantena o eliminare automaticamente il traffico da bot sospetti.

* **Autorizzazione ad approvare il modulo**: nuova autorizzazione per controllare quali designer possono approvare le modifiche apportate a un modulo in linea con altre risorse [!UICONTROL Design Studio]. In questo modo si impedisce ad altri progettisti di inviare le modifiche ai moduli senza che un altro utente con l&#39;autorizzazione di approvazione possa rivederle.

* **Esegui sempre la ripetizione della campagna dopo l&#39;unione anonima**: prima della ripetizione della campagna si verifica un&#39;unione lead anonima, pertanto i filtri dei campi personalizzati si comportano in modo affidabile al termine della ripetizione anonima della campagna.

## Ambiente dati di marketing

* **Correzione del troncamento dell&#39;interfaccia utente dei campi dell&#39;oggetto personalizzato &quot;[!UICONTROL Used By]&quot;**: è ora più semplice identificare i campi dell&#39;oggetto personalizzato &quot;in uso&quot; in modo da poter eliminare i campi da un oggetto personalizzato quando necessario.

## Miglioramenti API

* **Nuove funzionalità di filtro per API di estrazione membri programma in blocco**: consente di filtrare in base allo stato di appartenenza al programma, a UpdateAt, alla cadenza o al contenuto esaurito per perfezionare il set di dati estratto.

## [!DNL Sales Insight]

![(stella)](assets/yellow-star.png)

* **[[!DNL Sales Insight] Integrazione con [!DNL Dynamic Chat]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"}**: visualizza le attività di [!DNL Dynamic Chat] nel pannello [!DNL Sales Insight] e sfrutta questo nuovo punto dati nel tuo tentativo di ricerca di potenziali clienti.

## Annunci

**_Webinar sulla versione del prodotto_**

[Webinar sulla versione di Marketo Engage di giugno e agosto 2022](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}

## Ottobre 2022 {#october}

Qui sotto trovi tutte le funzioni incluse nella versione di ottobre 2022. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![star](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzioni rientrano nel ciclo di rilascio standard. Inizieranno a essere rilasciate il **sabato 14 ottobre 2022**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Di seguito è riportato lo stato di ciascuna funzionalità.

### Ambiente dati di marketing

</br>

* **Sincronizzazione campo personalizzato membro del programma**: possibilità di sincronizzare in modo bidirezionale i campi estensibili acquisiti per un membro del programma (ad esempio, le preferenze del partecipante durante la registrazione dell&#39;evento come cibo, sessioni, brani, ecc.) con Campi membro della campagna in Salesforce.

<table>
  <tr>
   <td><b>Stato</b></td>
   <td><b>Aggiornamenti alla documentazione</b></td>
  </tr>
  <tr>
   <td>Rilasciato</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md">Sincronizzazione campo personalizzato del membro del programma</a></td>
  </tr>
  </tbody>
</table>

* **Integrazione di Adobe Privacy Service**: esegui l&#39;armonizzazione con Privacy Service per automatizzare la conformità alle normative sulla privacy dei dati nei prodotti Experience Cloud. Attualmente, questo servizio è disponibile solo per i clienti Marketo Engage che hanno effettuato l’onboarding in Adobe Identity Management System.

<table>
  <tr>
   <td><b>Stato</b></td>
   <td><b>Aggiornamenti alla documentazione</b></td>
  </tr>
  <tr>
   <td>Rilasciato</td>
   <td><a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md">Adobe Identity Management</a></td>
  </tr>
  </tbody>
</table>

### Esperienza di nuova generazione

</br>

* **Screens aggiornato nell&#39;esperienza di nuova generazione**: verranno forniti schermi aggiuntivi e aggiornati nell&#39;esperienza di nuova generazione che offrono una progettazione aggiornata e miglioramenti a livello di usabilità accessibili tramite l&#39;interruttore:

   * Dettagli modello pagina di destinazione
   * Elenco modelli e-mail

<table>
  <tr>
   <td><b>Stato</b></td>
   <td><b>Aggiornamenti alla documentazione</b></td>
  </tr>
  <tr>
   <td>Rilasciato</td>
   <td><a href="/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md">Attiva/Disattiva</a></td>
  </tr>
  </tbody>
</table>

* **Utilizzo ottimizzato da scheda in Dettagli modello e-mail**: nella nuova esperienza verranno visualizzate informazioni aggiuntive relative alle risorse che utilizzano il modello e-mail, inclusi Stato risorsa, Ultima modifica e Ultima modifica di. Puoi anche cercare, ordinare e filtrare l’elenco delle risorse utilizzate.

<table>
  <tr>
   <td><b>Stato</b></td>
   <td><b>Aggiornamenti alla documentazione</b></td>
  </tr>
  <tr>
   <td>Rilasciato</td>
   <td>n/d</td>
  </tr>
  </tbody>
</table>

* **Modali filtro risorse report**: nuova progettazione per i moduli di configurazione dei report con una nuova struttura di risorse nel menu di configurazione e un filtro per Data di creazione e Modifica.

<table>
  <tr>
   <td><b>Stato</b></td>
   <td><b>Aggiornamenti alla documentazione</b></td>
  </tr>
  <tr>
   <td>Rilasciato</td>
   <td>n/d</td>
  </tr>
  </tbody>
</table>

### Miglioramenti API

</br>

* **Importazione lead in blocco: associazione venditore**: parità con API REST lead per associare i lead ai venditori durante il processo di importazione dei lead in blocco, riducendo la complessità e il numero di chiamate API richieste.

<table>
  <tr>
   <td><b>Stato</b></td>
   <td><b>Aggiornamenti alla documentazione</b></td>
  </tr>
  <tr>
   <td>Rilasciato</td>
   <td><a href="https://developer.adobe.com/marketo-apis/api/mapi/#tag/Bulk-Import-Leads">Importazione lead in blocco</a></td>
  </tr>
  </tbody>
</table>

### Insight di vendita

</br>

![(stella)](assets/yellow-star.png)

* **Integrazione di Sales Insight con Dynamic Chat**: il dashboard approfondimenti ora include le attività Dynamic Chat in Smart Grid insieme a un riepilogo settimanale e schede di dettagli.

<table>
  <tr>
   <td><b>Stato</b></td>
   <td><b>Aggiornamenti alla documentazione</b></td>
  </tr>
  <tr>
   <td>Rilasciato</td>
   <td><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md">Integrazione Dynamic Chat</a></td>
  </tr>
  </tbody>
</table>

## Funzioni di rilascio Agile

Le seguenti funzioni seguono un formato Agile e vengono rilasciate in varie date prima o dopo la data di rilascio standard. Di seguito è riportato lo stato di ciascuna funzionalità.

* **Flussi per finestre di dialogo di disposizione automatica per Dynamic Chat**: migliora l&#39;area di lavoro della finestra di dialogo di gruppo organizzando tutto ciò che si trova nell&#39;area di lavoro in un formato pulito e di facile lettura con la pressione di un pulsante tramite Disponi automaticamente.

<table>
  <tr>
   <td><b>Stato</b></td>
   <td><b>Aggiornamenti alla documentazione</b></td>
  </tr>
  <tr>
   <td>Rilasciato</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#stream-designer-icons">Icone Streaming Designer</a></td>
  </tr>
  </tbody>
</table>

* **Collegamenti riunione per Dynamic Chat**: opzione per includere automaticamente un collegamento Team o Incontro per Google e Outlook in ogni invito del calendario inviato ai visitatori.

<table>
  <tr>
   <td><b>Stato</b></td>
   <td><b>Aggiornamenti alla documentazione</b></td>
  </tr>
  <tr>
   <td>Rilasciato</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-settings.md">Calendario</a></td>
  </tr>
  </tbody>
</table>

* **Supporta tipi di dati aggiuntivi per Dynamic Chat**: tre nuovi tipi di dati (booleano, intero, in virgola mobile) consentono di sfruttare più campi Marketo Engage esistenti in Dynamic Chat per elementi quali il targeting in base a punteggi o la richiesta ai visitatori di domande sì/no.

<table>
  <tr>
   <td><b>Stato</b></td>
   <td><b>Aggiornamenti alla documentazione</b></td>
  </tr>
  <tr>
   <td>Rilasciato</td>
   <td>n/d</td>
  </tr>
  </tbody>
</table>

## Annunci

* **Forms 1.0**: la versione obsoleta di Forms 1.0 verrà completata con la versione di ottobre. Le risorse di Forms 1.0 non saranno più in grado di inviare dati a Marketo Engage e, se tentate, restituiranno errori.

* **Forms senza script**: Forms non funzionerà più se JavaScript è disabilitato nel browser. Per l’invio di un modulo è necessario abilitare JavaScript.
