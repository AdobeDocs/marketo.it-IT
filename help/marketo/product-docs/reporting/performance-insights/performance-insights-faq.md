---
unique-page-id: 12979858
description: Domande frequenti su Performance Insights - Documenti Marketo - Documentazione del prodotto
title: Domande frequenti su Performance Insights
exl-id: cee791c3-1845-4fca-b803-c0dc1c644549
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '1357'
ht-degree: 0%

---

# Domande frequenti su Performance Insights {#performance-insights-faq}

## Qual è la definizione di &quot;successo&quot; nella scheda Coinvolgimento? {#what-is-the-definition-of-success-in-the-engagement-tab}

Il successo è una misura dell&#39;interazione significativa in Marketo. Lo scopo di un programma è quello di creare un&#39;interazione significativa con la persona o il potenziale cliente. Il successo viene contrassegnato quando una persona raggiunge lo stato che raggiunge tale obiettivo. Può essere partecipare a un webinar, fare clic su un collegamento in un&#39;e-mail o compilare un modulo web. Il successo varia a seconda del canale del programma.

>[!NOTE]
>
>In un programma webinar possono essere presenti più stati, ad esempio: Invitati, registrati e presenti. Invitati o Registrati non sono interazioni significative perché le persone in realtà non guardano il webinar. In questo caso la partecipazione è considerata un successo.

## MPI funzionerà con qualsiasi CRM? {#will-mpi-work-with-any-crm}

Sì. Tecnicamente, MPI non interagisce direttamente con il CRM per la sincronizzazione dei dati. MPI utilizza i dati memorizzati nella Data Warehouse Marketo Analytics. Poiché la sincronizzazione CRM avviene nell’applicazione Gestione lead, qualsiasi CRM supportato da Marketo integrato con l’applicazione Gestione lead mostrerà correttamente i dati. Tuttavia, i campi delle opportunità di gestione delle relazioni con i clienti devono essere mappati correttamente nei campi delle opportunità di Marketo.

## Non ho altri prodotti Marketing Analytics (ARB, RCE, RCA, Program Analysis). MPI funzionerà per me? {#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

MPI è un componente aggiuntivo indipendente per l’applicazione Gestione lead. Non richiede l’utilizzo di altri prodotti di analisi.

## RCA mostra anche i dati sulle prestazioni del programma. C&#39;è una differenza tra i dati mostrati in MPI e RCA? {#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

No. MPI genera dati dallo stesso data warehouse di RCA. Pertanto, non vedrai alcuna differenza di dati tra i due. RCA ti permette di creare al volo i tuoi report. MPI consente di accedere a dashboard visivi di facile comprensione.

## Non voglio che alcuni dei miei programmi (ad esempio Operativi) vengano visualizzati in MPI. Come posso controllare la visibilità di programmi specifici? {#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

È possibile controllare la visibilità dei programmi impostando il comportamento di Analytics dei programmi su Operativo. In questo modo il programma verrà escluso dai calcoli di analisi.

>[!NOTE]
>
>Ulteriori informazioni sull&#39;impostazione del comportamento di analisi [qui](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/edit-analytics-behavior-settings.md).

## Sto eseguendo una campagna multicanale per un nuovo lancio di prodotto. Come posso visualizzare le prestazioni di questa campagna in tutti i diversi canali in un&#39;unica posizione? {#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

Per i programmi che fanno parte di una campagna di questo tipo, si consiglia di utilizzare i tag dei programmi. I tag programma vengono sincronizzati automaticamente in MPI e puoi filtrarli in tutte le dashboard MPI per visualizzare le prestazioni delle campagne multicanale.

## Posso accedere alle impostazioni di attribuzione se non ho RCA? {#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

Puoi accedere alle impostazioni di attribuzione se disponi di MPI, indipendentemente dal fatto che sia disponibile RCA o meno.

## Ricevo un avviso in MPI quando effettuo l’accesso per informarmi che le impostazioni di attribuzione non sono corrette. Cosa c&#39;è che non va? {#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

MPI calcola se tutte le opportunità vengono incluse o meno in analytics. In caso contrario, ti verrà richiesto di modificare le impostazioni di attribuzione (Esplicito, Implicito, Ibrido) per includere più opportunità.

È inoltre possibile che si verifichino delle opportunità mancanti a causa del costo del programma mancante nei programmi. Controlla il comportamento di Analytics dei tuoi programmi. Possono essere:

1. Predefinito : il comportamento predefinito è che il programma verrà incluso in MPI SOLO se vi è almeno un costo di periodo, anche uno con zero dollari assegnati.

1. Inclusivo : questa opzione assicura che il programma sia disponibile in MPI indipendentemente dal fatto che tu abbia incluso o meno un costo del periodo.

1. [Operativo](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs.md#operational-programs) - Questa opzione fa sì che il programma non venga visualizzato in MPI.

>[!NOTE]
>
>Costo del periodo **ha** da impostare per la generazione di rapporti con successo e nuovi nomi nel dashboard Coinvolgimento. Questo dashboard utilizza i dati Costo periodo per aggregare i successi e i nuovi nomi. Se Costo periodo non è impostato, il dashboard di coinvolgimento non recherà correttamente i rapporti indipendentemente dalle impostazioni di comportamento di Analytics riportate sopra.

## Perché mi mancano alcune opportunità nell&#39;MPI? {#why-am-i-missing-some-opportunities-in-mpi}

Due motivi principali per cui potresti perdere opportunità in MPI sono:

1. L’impostazione di attribuzione è impostata su Esplicito ma alle opportunità non sono assegnati ruoli di contatto
1. Il costo del periodo non è incluso nei programmi

MPI calcola se tutte le opportunità vengono incluse o meno in analytics. In caso contrario, ti verrà richiesto di modificare le impostazioni di attribuzione (Esplicito, Implicito, Ibrido) per includere più opportunità.

È inoltre possibile che si verifichino delle opportunità mancanti a causa del costo del programma mancante nei programmi. L&#39;avviso verrà lanciato ma non indica a quali programmi mancano i costi. Controlla la configurazione del programma per includere i costi, per assicurarsi che tutti i programmi e le opportunità siano inclusi in MPI.

## Perché non visualizzo i filtri Custom Fields, Opportunity Type e ABM nel dashboard di Engagement? {#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

I campi personalizzati, il tipo di opportunità e i filtri ABM sono tutti attributi relativi a un’opportunità. Il dashboard di coinvolgimento ti consente di misurare il coinvolgimento e l&#39;acquisizione principale, sia che siano associati o meno a un&#39;opportunità. Poiché il dashboard Coinvolgimento non prende in considerazione le opportunità, i campi personalizzati, il tipo di opportunità e i filtri ABM non sono applicabili.

## Voglio utilizzare un campo Opportunità Salesforce personalizzato per la generazione di rapporti sui ricavi invece del campo Importo opportunità Salesforce standard. L&#39;MPI mi permetterà di farlo? {#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

Sì. [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) è in grado di mappare nuovamente il campo Importo opportunità di Marketo in un campo Opportunità di Salesforce personalizzato, purché il tipo di campo sia valuta. Poiché MPI punta al campo Importo opportunità Marketo, MPI può utilizzare i dati del campo Salesforce personalizzato rimappato.

>[!NOTE]
>
>Dopo la nuova mappatura, MPI mostra i dati in corso. L&#39;importo storico non verrà modificato.

## Se non utilizzo opportunità, posso ancora utilizzare MPI? {#if-i-don-t-use-opportunities-can-i-still-use-mpi}

MPI è progettato per consentire di misurare le prestazioni del programma dalla parte superiore dell’imbuto fino all’impatto sui ricavi. Se non utilizzi le opportunità, sarai comunque in grado di:

* Visualizza le prestazioni dei tuoi programmi di formazione per l&#39;impegno del pubblico.
* Visualizza le prestazioni dei programmi di acquisizione lead.
* Visualizza le prestazioni delle campagne multicanale tramite i tag del programma.
* Scopri le tendenze di coinvolgimento del pubblico negli ultimi 12 mesi.
* Salvare ed esportare i dati sulle prestazioni in PowerPoint.

## Posso misurare il successo delle strategie basate su account in MPI? {#can-i-measure-the-success-of-account-based-strategies-in-mpi}

Sì. MPI si integra con [Marketo TAM](https://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview) per estrarre gli elenchi degli account ABM in MPI senza soluzione di continuità. Puoi utilizzare il filtro ABM Account List per scegliere l&#39;elenco ABM desiderato per filtrare i dati in base a.

## L’attribuzione è immediatamente disponibile quando si acquista MPI? {#is-attribution-instantly-available-when-i-purchase-mpi}

Le funzionalità di attribuzione Marketo sono disponibili per i nostri clienti quando acquistano MPI. Tuttavia, [installazione corretta](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md) è necessario per garantire che le opportunità e i dati del programma siano correttamente trasmessi in MPI.

## Cosa devo fare per impostare l’attribuzione? {#what-do-i-have-to-do-to-set-up-attribution}

1. Impostazione delle opportunità

   1. Assicurati che le opportunità siano sincronizzate con il tuo CRM
   1. Se le impostazioni di Attribuzione sono impostate su Esplicito, assicurati che i ruoli di contatto sulle opportunità siano compilati
   1. È consigliabile modificare l’impostazione di attribuzione in ibrido
   1. Configurazione del programma

      1. Includi i costi del programma nei programmi
      1. Esamina il comportamento di analisi per indicare se un programma deve essere incluso in analytics
      1. Imposta i criteri di successo per ogni canale disponibile
      1. Lega persona a programmi

         1. Assicurati che il programma di acquisizione e la data di acquisizione siano stati impostati per ciascuna persona nel database in modo che l&#39;attribuzione Primo contatto funzioni.
         1. Verificare che i programmi impostino gli stati di successo per le persone nel database

>[!TIP]
>
>Tutti i passaggi di configurazione richiesti sono descritti in [articolo](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md).

## Qual è la differenza tra MPI e Program Analyzer? {#whats-the-difference-between-mpi-and-the-program-analyzer}

Analisi programmi consente di confrontare i programmi in quattro misure. MPI consente di analizzare il canale e il contributo del programma per una metrica selezionata, come Success, New Opportunity Created, ecc. Ti consente inoltre di visualizzare la tendenza del canale a 12 mesi in base a una metrica specifica scelta.

## Qual è la differenza tra MPI e il Report Builder avanzato? {#whats-the-difference-between-mpi-and-the-advanced-report-builder}

Il Report Builder avanzato (a volte denominato RCE) è progettato per la generazione di rapporti self-service (o ad hoc), in genere eseguito dalle operazioni di marketing. MPI è progettato per consentire ai responsabili marketing e agli addetti al marketing di accedere con un solo clic all’analisi delle prestazioni. È necessaria una configurazione minima.

## Cos’è successo all’opzione &quot;Anno precedente&quot; nel filtro data di Contribution? {#what-happened-to-the-previous-year-option-in-contributions-date-filter}

Abbiamo temporaneamente rimosso la selezione &quot;Anno precedente&quot;. Puoi comunque visualizzare i dati delle prestazioni dell’intero anno utilizzando la selezione Intervallo date personalizzato .
