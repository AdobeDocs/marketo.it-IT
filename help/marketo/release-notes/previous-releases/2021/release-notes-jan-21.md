---
description: Note sulla versione - Gennaio 2021 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Gennaio 2021
exl-id: 24a5f955-ef4b-4adf-9478-2653db6f9d79
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '1234'
ht-degree: 0%

---

# Note sulla versione: gennaio 2021 {#release-notes-jan-21}

Le seguenti funzioni sono incluse nella versione del 21 gennaio. Verifica la disponibilità delle funzioni nella tua edizione di Marketo.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![(stella)](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

**_Versioni trimestrali_**

Le seguenti funzionalità saranno rilasciate il **15 gennaio 2021**.

## Esperienza utente di nuova generazione {#next-generation-user-experience}

* Supporto per le aree di lavoro: l&#39;esperienza utente di Marketo Engage di nuova generazione unisce l&#39;aspetto di Adobe Experience Cloud alle innovazioni di produttività per consentire ai professionisti del marketing di lavorare in modo più rapido e intelligente. Nell’ultima versione è stato aggiunto il supporto completo per aree di lavoro e partizioni, inclusa la possibilità di condividere cartelle tra aree di lavoro diverse. L’area di lavoro a destra offre un interruttore per passare facilmente dalle vecchie alle nuove esperienze per funzione senza perdere contesto. [Ulteriori informazioni](https://nation.marketo.com/t5/The-modern-ux/modern-ux-FAQ/ba-p/307124) dalle domande frequenti sull&#39;esperienza di nuova generazione su Marketing Nation.

## Personalization multicanale {#multi-channel-personalization}

* **[Adobe Experience Cloud Audience Sync Phase 3](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**: la funzionalità esistente di Adobe Experience Cloud (AEC) Audience Sync ora supporta la sincronizzazione bidirezionale continua del pubblico B2B da Marketo Engage ad altre applicazioni AEC, incluse offerte Adobe Experience Platform (AEP) come Real-time Customer Data Platform e Adobe Experience Platform Activation.  Man mano che i lead vengono aggiunti e rimossi dai segmenti di pubblico, Marketo Engage sincronizzerà automaticamente il pubblico aggiornato tra le app AEC connesse. Utilizzalo per sfruttare i casi d’uso multicanale di orchestrazione, retargeting, soppressione del pubblico, personalizzazione e reporting di Adobe nel tuo stack tecnologico AEC.
* **[Sincronizzazione continua del pubblico con Google, [!DNL Facebook] e [!DNL LinkedIn]](/help/marketo/product-docs/demand-generation/ad-network-integrations/send-a-list-to-an-ad-network.md)**: è possibile abilitare la sincronizzazione automatizzata continua con una rete di annunci in un elenco statico, aggiornando la rete di annunci come modifiche all&#39;iscrizione all&#39;elenco senza richiedere l&#39;intervento dell&#39;utente.
* **[Token per i campi personalizzati dei membri del programma](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/program-member-custom-field-tokens.md)**: sono state estese le funzionalità dei campi personalizzati dei membri del programma per supportare il framework dei token. Gli addetti al marketing possono inserire token di campi personalizzati per i membri del programma in e-mail, pagine di destinazione, messaggi SMS, notifiche push e webhook. Utilizza i nuovi token nelle azioni del flusso della campagna per modificare i valori dei dati, creare un’attività o un momento di interesse.

## Pagine di destinazione e Forms {#landing-pages-and-forms}

* **API modulo**: richiama le informazioni sul lead o attiva le campagne di acquisizione durante l&#39;estrazione dei dati da moduli non Marketo. I moduli non Marketo possono essere integrati con Marketo Engage tramite API REST. La nuova API consente di simulare l’invio di moduli Marketo Engage con tutte le funzionalità associate.
* **API per le pagine di destinazione**: semplifica i flussi di lavoro di modifica e traduzione nelle applicazioni integrate con la nuova API di anteprima della pagina di destinazione. I fornitori di terze parti possono ora eseguire il rendering delle anteprime completamente personalizzate delle pagine di destinazione senza effettuare l’accesso a Marketo Engage.  L’API di anteprima pagina di destinazione consente di modificare e localizzare i flussi di lavoro in applicazioni integrate di terze parti.

## E-mail marketing {#email-marketing}

* **[Limiti di recupero oggetti personalizzati aumentati](/help/marketo/product-docs/administration/email-setup/change-custom-object-retrieval-limits-in-velocity-scripting.md)**: gli sviluppatori di script di velocità e-mail possono aumentare rapidamente il numero di oggetti personalizzati a 100 tramite sostituzione self-service. Gli addetti al marketing possono aumentare l’efficacia delle campagne intelligenti accedendo a un numero maggiore di oggetti personalizzati di primo e secondo livello.

## Integrazione CRM [!DNL Salesforce] {#salesforce-crm-integration}

* [[!DNL Salesforce] Autenticazione CRM](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md): il protocollo OAuth 2.0 è disponibile per le operazioni di sincronizzazione tra Marketo Engage e [!DNL Salesforce] CRM. Per i nuovi abbonati, questa opzione è attivata per impostazione predefinita. Gli attuali abbonati possono richiedere questa funzionalità contattando il supporto Marketo.
* [[!DNL Salesforce] Dashboard di sincronizzazione CRM](/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.md): gli amministratori possono rivedere rapidamente lo stato di sincronizzazione di [!DNL Salesforce] CRM dal dashboard. La durata del rapporto sulle prestazioni di sincronizzazione è stata aumentata da 2 ore a 5 giorni.
* **Esportazione metadati**: migliorata per supportare gli attributi dell&#39;oggetto opportunità, gli account denominati e i campi standard e personalizzati del membro del programma.

## Amministrazione {#administration}

* **Pagina Account personale aggiornata**: controlla le informazioni essenziali sull&#39;abbonamento nella pagina Account personale. Gli utenti con qualsiasi livello di accesso possono visualizzare il nome della sottoscrizione, l&#39;identificatore del centro dati e l&#39;ID [!DNL Munchkin].

**_Rilascio nel corso del trimestre_**

Le seguenti funzioni sono in un ciclo non trimestrale e verranno rilasciate nei prossimi mesi.

## [!DNL Sales Insight] {#sales-insight}

![(stella)](assets/yellow-star.png)

* **[Flussi di lavoro e-mail per test migliorati ([!DNL Salesforce] CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/send-a-test-email.md)**: aumenta l&#39;efficienza del team di vendita con [!DNL Sales Insight] flussi di lavoro e-mail per test migliorati. I venditori possono inviare e-mail di prova agli indirizzi e-mail selezionati prima di inviare e-mail in blocco a 200 destinatari.
* **[Informazioni sullo stato delle e-mail ([!DNL Salesforce] CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/email-tab.md)**: gli utenti visualizzano un messaggio di avviso quando tentano di inviare un messaggio e-mail a un ID e-mail non valido o a un indirizzo e-mail non sottoscritto prima di inviare un messaggio e-mail.  Gli stati di consegna delle e-mail possono essere verificati nella scheda e-mail di [!DNL Sales Insight].
* **Invia e-mail in blocco da [Account](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#account-layout) e [Opportunità](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#opportunity-layout) Pannelli ([!DNL Salesforce] CRM)**: migliora l&#39;efficienza del flusso di lavoro del venditore e interagisci con un intero elenco di contatti dell&#39;account o dell&#39;opportunità utilizzando nuove funzioni per azioni in blocco. Invia e-mail o aggiungi contatti alle campagne Marketo Engage utilizzando la nuova opzione a discesa nelle schede account o opportunità invece di lavorare con i singoli contatti. Aggiungere contatti dell&#39;account a una watchlist per ricevere una notifica quando i lead diventano attivi.
* **[[!DNL Sales Insight] per integrazioni non native [!DNL Salesforce] CRM](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)**: gli abbonamenti GA con integrazioni Salesforce CRM personalizzate possono installare il pacchetto [!DNL Sales Insight] e aiutare i team di vendita a definire le priorità e interagire con i lead e le opportunità più promettenti.
* **[Miglioramenti elementi di maggiore rilevanza](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/marketo-tab/best-bets.md)**: contatta rapidamente gli hot lead dalla scheda Elementi di maggiore rilevanza inviandoli per e-mail o aggiungendoli a una campagna Marketo Engage. Visualizza un lead in Marketo Engage o aggiungilo alla watchlist. Le azioni in blocco e le opzioni di ordinamento nella scheda [!UICONTROL Best Bets] consentono di risparmiare tempo e migliorare l&#39;efficienza del team vendite.

## [!DNL Sales Connect] {#sales-connect}

![(stella)](assets/yellow-star.png)

* **Limitazione della connessione e-mail (BETA)**: migliora il recapito messaggi e-mail e ridimensiona le comunicazioni di vendita 1:1 con Limitazione della connessione e-mail per [!DNL Sales Connect]. La nostra nuova tecnologia di limitazione gestisce automaticamente la tempistica di invio delle e-mail per creare esperienze ottimizzate per [!DNL Exchange] e gli utenti Gmail. Riduzione o eliminazione dell&#39;utilizzo di applicazioni di invio di posta elettronica in blocco di terze parti.
* **Tracciamento mancato recapito connessione e-mail**: ottieni da insight la qualità del lead e le prestazioni del modello e-mail con il nuovo rapporto e-mail non recapitate. [!DNL Exchange] e gli utenti Gmail possono scegliere di ricevere le notifiche di mancato recapito che verranno riportate in Live Feed, Cartelle e-mail, Template Analytics e Campaign Analytics.
* **Configurazione pagina profilo**: gestisci facilmente le preferenze utente nella nuova pagina profilo. Modifica la password, modifica le impostazioni di geolocalizzazione e lingua e rivedi gli stati delle integrazioni da un’unica posizione.
* **Gestione modelli**: organizza i modelli e-mail per le vendite in categorie con una nuova funzione di trascinamento per garantire un accesso rapido ai modelli rilevanti e ridurre i tempi di ricerca.
* **[!DNL Sales Connect]aggiornamenti esperienza utente**: personalizza il layout della griglia [!DNL Sales Connect] ridimensionando e riordinando le colonne. Le preferenze di visualizzazione vengono salvate automaticamente.

**_Annunci ed elementi obsoleti_**

* Tutti gli utenti devono effettuare l&#39;aggiornamento alla versione più recente di Sales Insight **prima del 15 gennaio 2021**. Se non hai completato l’aggiornamento, ti verrà richiesto di farlo al momento dell’accesso all’applicazione. Segui le istruzioni [in questa guida](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md). La versione aggiornata include una patch per una vulnerabilità di sicurezza identificata. La patch è stata originariamente rilasciata il 6 aprile 2016. Nota: **Le versioni 1.4363 o successive** non devono eseguire un aggiornamento.
* Il servizio Form 1.0 diventerà obsoleto a partire dalla versione **maggio 2021**. Il servizio Forms 1.0 diventerà completamente obsoleto, con conseguente perdita di funzionalità delle risorse Forms 1.0 ancora in uso. Inoltre, gli invii di moduli effettuati tramite metodi non supportati, ad esempio moduli programmatici POST agli endpoint leadCapture/save e leadCapture/save2, verranno rifiutati. Per ulteriori informazioni e soluzioni, consulta [il nostro post in Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-the-Marketo-Engage-Form-Platform/ta-p/306631).
* Nel 2021, Marketo Engage apporterà modifiche alla struttura URL per le pagine di destinazione, i moduli e le risorse di immagini e file. Per gli abbonamenti Marketo Engage esistenti, inizieremo il rollout graduale il 1° aprile 2021. Ulteriori dettagli sulla timeline di rollout saranno rilasciati a marzo 2021. Per informazioni dettagliate su come cambierà ogni tipo di risorsa interessata, consulta [il nostro post in Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-Design-Studio-URLs/ta-p/306632).

**_Webinar sulla versione del prodotto_**

Vuoi saperne di più su queste funzioni e miglioramenti? [registratevi ora](https://engage.marketo.com/January_21_Release_Webinar_Registration.html) per partecipare a un webinar live con il nostro team di prodotto il 21 gennaio alle 13:00 PT / 16:00 ET e approfondire ulteriormente queste innovazioni.
