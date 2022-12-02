---
description: Note sulla versione - Jan 2021 - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione - Gennaio 2021
exl-id: 24a5f955-ef4b-4adf-9478-2653db6f9d79
source-git-commit: 85e04fb8a52a417982014bc4bb101b6044e53f84
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 0%

---

# Note sulla versione: Gen. 2021 {#release-notes-jan-21}

Le seguenti funzionalità sono incluse nella versione del 21 gennaio. Per informazioni sulla disponibilità delle funzioni, consulta la tua edizione Marketo .

>[!AVAILABILITY]
>
>Caratteristiche indicate da una stella (![(stella)](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

**_Versioni trimestrali_**

Le seguenti funzionalità verranno rilasciate il **15 gennaio 2021**.

## Esperienza utente di nuova generazione {#next-generation-user-experience}

* Supporto per le aree di lavoro: L’esperienza utente Marketo Engage di nuova generazione unisce l’aspetto e il design di Adobe Experience Cloud alle innovazioni di produttività per aiutare gli addetti al marketing a lavorare in modo più rapido e intelligente. Nell’ultima versione, è stato aggiunto il supporto completo per aree di lavoro e partizioni, inclusa la possibilità di condividere cartelle tra aree di lavoro. L’area di lavoro a destra offre un interruttore di attivazione/disattivazione che consente di passare facilmente da esperienze vecchie a nuove per caratteristica senza perdere contesto. [Ulteriori informazioni](https://nation.marketo.com/t5/The-modern-ux/modern-ux-FAQ/ba-p/307124) dalle domande frequenti sull’esperienza di nuova generazione su Marketing Nation.

## Personalizzazione multicanale {#multi-channel-personalization}

* **[Fase 3 di Adobe Experience Cloud Audience Sync](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**: La funzionalità di sincronizzazione dell&#39;audience di Adobe Experience Cloud (AEC) supporta ora la sincronizzazione continua e bidirezionale dell&#39;audience B2B dal Marketo Engage ad altre applicazioni AEC, tra cui le offerte Adobe Experience Platform (AEP) come Real-time Customer Data Platform e Adobe Experience Platform Activation.  Man mano che i lead vengono aggiunti e rimossi ai segmenti di pubblico, Marketi Engage sincronizza automaticamente il pubblico aggiornato nelle app AEC collegate. Usarlo per sfruttare l’orchestrazione multicanale di Adobe, il ritargeting, la soppressione del pubblico, la personalizzazione e i casi di utilizzo del reporting nello stack di tecnologie AEC.
* **[Sincronizzazione continua del pubblico con Google, Facebook e LinkedIn](/help/marketo/product-docs/demand-generation/ad-network-integrations/send-a-list-to-an-ad-network.md)**: La sincronizzazione automatica continua con una rete pubblicitaria può essere abilitata su un elenco statico, aggiornando la rete pubblicitaria come modifica dell’appartenenza all’elenco senza richiedere l’intervento dell’utente.
* **[Token per i campi personalizzati dei membri del programma](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/program-member-custom-field-tokens.md)**: Abbiamo esteso le funzionalità dei campi personalizzati dei membri del programma per supportare il framework dei token. Gli addetti al marketing possono inserire token di campi personalizzati per i membri del programma in e-mail, pagine di destinazione, messaggi SMS, notifiche push e webhook. Utilizza nuovi token nelle azioni di flusso delle campagne per modificare i valori dei dati, creare un’attività o un momento interessante.

## Pagine di destinazione e Forms {#landing-pages-and-forms}

* **API modulo**: Recupera informazioni lead o attiva campagne di sviluppo durante l’estrazione di dati da moduli non Marketo. I moduli non Marketo possono integrarsi con il Marketo Engage tramite l’API REST. La nuova API consente di simulare l’invio di moduli di Marketo Engage con tutte le funzionalità associate.
* **API delle pagine di destinazione**: Semplifica i flussi di lavoro di modifica e traduzione nelle applicazioni integrate con la nuova API di anteprima della pagina di destinazione. Ora i fornitori di terze parti possono eseguire il rendering di anteprime completamente personalizzate delle pagine di destinazione senza effettuare l’accesso al Marketo Engage.  L’API di anteprima della pagina di destinazione consente flussi di lavoro end-to-end per la modifica e la localizzazione in applicazioni integrate di terze parti.

## E-mail marketing {#email-marketing}

* **[Limiti di recupero oggetti personalizzati aumentati](/help/marketo/product-docs/administration/email-setup/change-custom-object-retrieval-limits-in-velocity-scripting.md)**: Gli sviluppatori di e-mail Velocity Scripting possono rapidamente aumentare il numero di oggetti personalizzati a 100 tramite l’override del self-service. Gli addetti al marketing possono aumentare l’efficacia delle campagne avanzate accedendo a un numero maggiore di oggetti personalizzati di primo e secondo livello.

## Integrazione CRM Salesforce {#salesforce-crm-integration}

* [Autenticazione CRM Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md): Il protocollo OAuth 2.0 è disponibile per le operazioni di sincronizzazione tra Marketi Engage e CRM Salesforce. Per i nuovi abbonati, questa opzione è attivata per impostazione predefinita. Gli abbonati attuali possono richiedere questa funzione contattando il supporto Marketo.
* [Dashboard di sincronizzazione di Salesforce CRM](/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.md): Gli amministratori possono rivedere rapidamente lo stato di sincronizzazione CRM Salesforce dal dashboard. L’intervallo di tempo del rapporto sulle prestazioni di sincronizzazione è stato aumentato da 2 a 5 giorni.
* **Esportazione metadati**: Migliorata per supportare gli attributi degli oggetti opportunità, gli account denominati, i campi standard e personalizzati dei membri del programma.

## Amministrazione {#administration}

* **Pagina Account personale aggiornata**: Rivedi le informazioni di iscrizione essenziali nella pagina Il mio account . Gli utenti con qualsiasi livello di accesso possono visualizzare il nome della sottoscrizione, l’identificatore del centro dati e l’ID Munchkin.

**_Rilascio in tutto il trimestre_**

Le seguenti caratteristiche sono su un ciclo non trimestrale e saranno rilasciate durante i prossimi mesi.

## Approfondimenti vendite {#sales-insight}

![(stella)](assets/yellow-star.png)

* **[Flussi di lavoro e-mail di test migliorati (CRM Salesforce)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/send-a-test-email.md)**: Aumenta l’efficienza del tuo team di vendita con flussi di lavoro e-mail di test Approfondimenti vendite migliorati. I venditori possono inviare e-mail di prova agli indirizzi e-mail selezionati prima di inviare e-mail in blocco a un massimo di 200 destinatari.
* **[Informazioni sullo stato delle e-mail (CRM Salesforce)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/email-tab.md)**: Gli utenti visualizzano un messaggio di avviso quando tentano di inviare un’e-mail a un ID e-mail non valido o a un indirizzo e-mail non iscritto prima di inviare un’e-mail.  Gli stati di consegna e-mail possono essere rivisti nella scheda e-mail di Informazioni sulle vendite.
* **Invia e-mail in blocco da [Account](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#account-layout) e [Opportunità](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#opportunity-layout) Pannelli (CRM Salesforce)**: Migliora l&#39;efficienza del flusso di lavoro del venditore e interagisci con un intero account o un elenco di contatti opportunità utilizzando nuove funzionalità di azione collettiva. Invia e-mail o aggiungi contatti alle campagne di Marketo Engage utilizzando la nuova opzione a discesa nell’account o nelle schede delle opportunità anziché lavorare con i singoli contatti. Aggiungi i contatti dell’account a una lista di controllo da avvisare quando i lead diventano attivi.
* **[Informazioni sulle vendite per le integrazioni CRM non native con Salesforce](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)**: Gli abbonamenti GA con integrazioni CRM Salesforce personalizzate possono installare il pacchetto Insight vendite e aiutare i team di vendita a dare la priorità e a interagire con i lead e le opportunità più promettenti.
* **[Migliori miglioramenti](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/marketo-tab/best-bets.md)**: Contatta rapidamente i lead a caldo dalla scheda Best Bets inviandoli tramite e-mail o aggiungendoli a una campagna di Marketo Engage. Visualizza un lead in Marketo Engage o aggiungilo alla lista di controllo. Le azioni collettive e le opzioni di ordinamento nella scheda Best Bets consentono di risparmiare tempo e migliorare l’efficienza del team di vendita.

## Sales Connect {#sales-connect}

![(stella)](assets/yellow-star.png)

* **Limitazione connessione e-mail (BETA)**: Migliora il recapito dei messaggi e-mail e ridimensiona la comunicazione di vendita 1:1 con la limitazione della connessione e-mail per Sales Connect. La nostra nuova tecnologia di limitazione gestisce automaticamente i tempi di invio delle e-mail per creare esperienze senza soluzione di continuità per gli utenti di Exchange e Gmail. Diminuisci o elimina l’utilizzo di applicazioni di invio in massa di e-mail di terze parti.
* **Tracciamento messaggi non recapitati connessione e-mail**: Ottieni informazioni approfondite sulla qualità dei lead e sulle prestazioni dei modelli e-mail con il nuovo rapporto non recapitato per e-mail. Gli utenti di Exchange e Gmail possono scegliere di ricevere notifiche non recapitate che passeranno a Feed live, Cartelle e-mail, Analisi dei modelli e Analytics di Campaign.
* **Configurazione della pagina del profilo**: Gestisci le preferenze utente con facilità nella nuova pagina del profilo. Modifica la password, modifica le impostazioni di geolocalizzazione e lingua e rivedi gli stati delle integrazioni in un’unica posizione.
* **Gestione dei modelli**: Organizza i modelli e-mail di vendita in categorie con una nuova funzione di trascinamento della selezione per garantire un accesso rapido ai modelli rilevanti e ridurre i tempi di ricerca.
* **Aggiornamenti all&#39;esperienza utente di Sales Connect**: Personalizzare il layout della griglia di Sales Connect ridimensionando e riordinando le colonne. Le preferenze di visualizzazione vengono salvate automaticamente.

**_Annunci ed elementi obsoleti_**

* Tutti gli utenti devono effettuare l&#39;aggiornamento alla versione più recente di Sales Insight **prima del 15 gennaio 2021**. Se non hai completato l&#39;aggiornamento, ti verrà richiesto di farlo dopo aver effettuato l&#39;accesso all&#39;applicazione. Seguire le istruzioni [in questa guida](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md). La versione aggiornata include una patch per una vulnerabilità di sicurezza identificata. La patch è stata originariamente rilasciata il 6 aprile 2016. Nota: **Versioni 1.4363 o successive** non è necessario eseguire un aggiornamento.
* Il servizio Form 1.0 diventerà obsoleto **Maggio 2021** rilascio. Il servizio Forms 1.0 diventerà completamente obsoleto, con conseguente perdita di funzionalità per tutte le risorse Forms 1.0 rimanenti ancora in uso. Inoltre, gli invii di moduli effettuati tramite metodi non supportati, ad esempio POST programmatici agli endpoint leadCapture/save e leadCapture/save2, verranno rifiutati. Per ulteriori informazioni e per la risoluzione dei problemi, consulta [il nostro post in Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-the-Marketo-Engage-Form-Platform/ta-p/306631).
* Nel 2021 Marketi Engage apporterà modifiche alla struttura URL per le risorse di pagine di destinazione, moduli, immagini e file. Per gli abbonamenti al Marketo Engage esistenti, inizieremo il rollout graduale il 1° aprile 2021. Maggiori dettagli sulla timeline del rollout saranno disponibili a marzo 2021. Per informazioni dettagliate sulle modifiche apportate a ciascun tipo di risorsa interessato, consulta [il nostro post in Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-Design-Studio-URLs/ta-p/306632).

**_Webinar sulla versione del prodotto_**

Vuoi saperne di più su queste funzioni e miglioramenti? Assicurati di [registra](https://engage.marketo.com/January_21_Release_Webinar_Registration.html) per partecipare il 21 gennaio alle 13:00 PT / 4:00 PM ET a un webinar dal vivo con il nostro team di prodotto per approfondire queste innovazioni.
