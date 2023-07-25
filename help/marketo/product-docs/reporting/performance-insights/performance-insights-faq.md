---
unique-page-id: 12979858
description: Domande frequenti su Performance Insights - Documentazione di Marketo - Documentazione del prodotto
title: Domande frequenti su Performance Insights
exl-id: cee791c3-1845-4fca-b803-c0dc1c644549
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1357'
ht-degree: 0%

---

# Domande frequenti su Performance Insights {#performance-insights-faq}

## Qual è la definizione di &quot;successo&quot; nella scheda Coinvolgimento? {#what-is-the-definition-of-success-in-the-engagement-tab}

Il successo è una misura dell’interazione significativa in Marketo. Lo scopo di un programma è quello di creare un’interazione significativa con la persona o il potenziale cliente. Il successo è contrassegnato quando una persona raggiunge lo stato che raggiunge tale obiettivo. Può essere la partecipazione a un webinar, il clic su un link in un messaggio e-mail o la compilazione di un modulo web. Il successo dipende dal canale del programma.

>[!NOTE]
>
>In un programma di webinar possono essere presenti più stati, ad esempio Invitato, Registrato e Partecipato. Invitato o Registrato non sono interazioni significative perché le persone non guardano effettivamente il webinar. In questo caso, partecipare è considerato un successo.

## MPI funzionerà con qualsiasi CRM? {#will-mpi-work-with-any-crm}

Sì. Tecnicamente, MPI non interagisce direttamente con il sistema CRM per la sincronizzazione dei dati. MPI utilizza i dati memorizzati nella Data Warehouse di Marketo Analytics. Poiché la sincronizzazione CRM si verifica nell&#39;applicazione Gestione lead, qualsiasi CRM supportato da Marketo integrato nell&#39;applicazione Gestione lead visualizzerà correttamente i dati. Tuttavia, i campi dell’opportunità di gestione delle relazioni con i clienti devono essere mappati correttamente ai campi dell’opportunità di Marketo.

## Non ho altri prodotti di analisi di marketing (ARB, RCE, RCA, analisi del programma). L&#39;MPI funzionerà per me? {#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

MPI è un componente aggiuntivo indipendente per l&#39;applicazione Gestione lead. Non richiede l’uso di altri prodotti di analisi.

## RCA mostra anche i dati sulle prestazioni del programma. C&#39;è una differenza tra i dati mostrati in MPI e RCA? {#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

No. Origini MPI dati provenienti dallo stesso data warehouse di RCA. Pertanto, non vedrai alcuna differenza di dati tra i due. RCA consente di creare rapporti personalizzati al volo. MPI consente di accedere a dashboard visivi di facile comprensione.

## Non voglio che alcuni dei miei programmi (ad es. Operativi) vengano visualizzati in MPI. Come si controlla la visibilità di programmi specifici? {#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

Puoi controllare la visibilità dei programmi impostando il comportamento Analytics dei programmi su Operativo. In questo modo il programma verrà escluso dai calcoli di Analytics.

>[!NOTE]
>
>Ulteriori informazioni sull’impostazione del comportamento di analisi [qui](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/edit-analytics-behavior-settings.md).

## Sto eseguendo una campagna multicanale per il lancio di un nuovo prodotto. Come posso visualizzare le prestazioni per questa campagna tra tutti i diversi canali in un’unica posizione? {#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

Per i programmi che fanno parte di una campagna di questo tipo, è consigliabile utilizzare i tag dei programmi. I tag del programma vengono sincronizzati automaticamente con MPI e puoi filtrarli in tutte le dashboard MPI per visualizzare le prestazioni della campagna multicanale.

## Posso accedere alle impostazioni di attribuzione se non dispongo di RCA? {#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

Puoi accedere alle impostazioni di attribuzione se disponi di MPI, indipendentemente dal fatto che tu disponga di RCA o meno.

## All’accesso ricevo un avviso in MPI che indica che le impostazioni di attribuzione non sono corrette. Cosa c&#39;è che non va? {#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

MPI calcola se includere o meno tutte le opportunità in Analytics. In caso contrario, ti verrà chiesto di considerare la possibilità di modificare le impostazioni di attribuzione (Esplicita, Implicita, Ibrida) per includere più opportunità.

Potresti anche perdere delle opportunità a causa del costo del programma mancante nei tuoi programmi. Controlla il comportamento Analytics dei tuoi programmi. Possono essere:

1. Predefinito: il comportamento predefinito è che il programma viene incluso solo in MPI se è presente almeno un costo periodo, anche uno a cui è assegnato zero dollari.

1. Inclusivo: questa opzione garantisce che il programma sia disponibile in MPI indipendentemente dal fatto che sia stato incluso o meno un costo del periodo.

1. [Operativo](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs.md#operational-programs) - Con questa opzione il programma non viene visualizzato in MPI.

>[!NOTE]
>
>Costo periodo **ha** da configurare per la generazione di rapporti di successo e nuovi nomi nel dashboard Coinvolgimento. Questo pannello di controllo utilizza i dati relativi al costo periodo per aggregare i successi e i nuovi nomi. Se non è impostato il costo del periodo, il dashboard di coinvolgimento non genererà rapporti corretti indipendentemente dalle impostazioni di comportamento di Analytics riportate sopra.

## Perché mi mancano alcune opportunità in MPI? {#why-am-i-missing-some-opportunities-in-mpi}

Due motivi principali per cui potresti non avere opportunità in MPI sono:

1. L&#39;impostazione di attribuzione è impostata su Esplicito, ma alle opportunità non sono assegnati ruoli di contatto
1. Il costo del periodo non è incluso nei programmi

MPI calcola se includere o meno tutte le opportunità in Analytics. In caso contrario, ti verrà chiesto di considerare la possibilità di modificare le impostazioni di attribuzione (Esplicita, Implicita, Ibrida) per includere più opportunità.

Potresti anche perdere delle opportunità a causa del costo del programma mancante nei tuoi programmi. L&#39;avviso viene visualizzato ma non indica a quali programmi mancano i costi. Rivedi la configurazione del programma per includere i costi, in modo che tutti i programmi e le opportunità siano inclusi in MPI.

## Perché non vedo i filtri Campi personalizzati, Tipo di opportunità e ABM nel dashboard Coinvolgimento? {#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

I campi personalizzati, il tipo di opportunità e i filtri ABM sono tutti attributi correlati a un’opportunità. Il dashboard Coinvolgimento consente di misurare il coinvolgimento e l’acquisizione dei lead, indipendentemente dal fatto che siano associati o meno a un’opportunità. Poiché il dashboard Coinvolgimento non prende in considerazione l’opportunità, i campi personalizzati, il tipo di opportunità e i filtri ABM non sono applicabili.

## Desidero utilizzare un campo personalizzato Opportunità Salesforce per la generazione di rapporti sui ricavi anziché il campo standard Importo opportunità Salesforce. L&#39;MPI mi permette di farlo? {#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

Sì. [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) è in grado di rimappare il campo Importo opportunità di Marketo in un campo personalizzato Opportunità Salesforce, purché il tipo di campo sia valuta. Poiché MPI punta al campo Importo opportunità Marketo, può utilizzare i dati del campo personalizzato Salesforce ricampionato.

>[!NOTE]
>
>Dopo la nuova mappatura, MPI mostrerà i dati in corso. La quantità storica non verrà modificata.

## Se non utilizzo le opportunità, posso comunque utilizzare MPI? {#if-i-don-t-use-opportunities-can-i-still-use-mpi}

MPI è progettato per consentire di misurare le prestazioni del programma dall’alto del funnel fino all’impatto sui ricavi. Se non utilizzi le opportunità, potrai comunque:

* Visualizza le prestazioni dei tuoi programmi di crescita per il coinvolgimento del pubblico.
* Visualizza le prestazioni dei programmi di acquisizione lead.
* Visualizza le prestazioni delle campagne multicanale tramite i tag del programma.
* Guarda le tendenze di coinvolgimento del pubblico negli ultimi 12 mesi.
* Salvataggio ed esportazione dei dati sulle prestazioni in PowerPoint.

## Posso misurare il successo delle strategie basate su account in MPI? {#can-i-measure-the-success-of-account-based-strategies-in-mpi}

Sì. MPI si integra con [MARKETO TAM](https://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview) per richiamare facilmente gli elenchi di account ABM in MPI. È possibile utilizzare il filtro Elenco account ABM per scegliere l&#39;elenco ABM desiderato in base al quale filtrare i dati.

## L’attribuzione è immediatamente disponibile quando acquisto MPI? {#is-attribution-instantly-available-when-i-purchase-mpi}

Le funzionalità di attribuzione Marketo sono disponibili per i nostri clienti quando acquistano MPI. Tuttavia, [configurazione corretta](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md) è necessario per garantire che le opportunità e i dati del programma fluiscano correttamente in MPI.

## Cosa devo fare per impostare l’attribuzione? {#what-do-i-have-to-do-to-set-up-attribution}

1. Configurazione dell’opportunità

   1. Assicurati che le opportunità siano sincronizzate con il CRM
   1. Se le impostazioni di attribuzione sono impostate su Esplicito, assicurati che i ruoli di contatto nelle opportunità siano popolati
   1. È consigliabile modificare l’impostazione di attribuzione in Ibrida
   1. Configurazione del programma

      1. Includi il costo del programma nei programmi
      1. Esamina il comportamento di Analytics per indicare se un programma deve essere incluso nell’analisi
      1. Impostare i criteri di successo per ogni canale
      1. Collega persona a programmi

         1. Assicurati che il programma di acquisizione e la data di acquisizione siano stati impostati per ogni persona nel database affinché l’attribuzione del primo contatto funzioni.
         1. Verificare che i programmi impostino gli stati di successo per le persone nel database

>[!TIP]
>
>Tutti i passaggi di configurazione richiesti sono descritti in [questo articolo](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md).

## Qual è la differenza tra MPI e Program Analyzer? {#whats-the-difference-between-mpi-and-the-program-analyzer}

L’analizzatore di programmi consente di confrontare i programmi di fino a quattro misure. MPI consente di analizzare il contributo del canale e del programma verso una metrica selezionata, ad esempio successo, nuove opportunità create e così via. Consente inoltre di visualizzare la tendenza del canale a 12 mesi in base a una metrica specifica scelta.

## Qual è la differenza tra MPI e il Report Builder avanzato? {#whats-the-difference-between-mpi-and-the-advanced-report-builder}

Il Report Builder avanzato (talvolta indicato come RCE) è progettato per la generazione di rapporti self-service (o ad hoc), in genere eseguiti dalle operazioni di marketing. MPI è progettato per fornire ai leader di marketing e agli esperti di marketing l’accesso con un solo clic all’analisi delle prestazioni. È richiesta una configurazione minima.

## Cos’è successo all’opzione &quot;Anno precedente&quot; nel filtro data del contributo? {#what-happened-to-the-previous-year-option-in-contributions-date-filter}

La selezione &quot;Anno precedente&quot; è stata temporaneamente rimossa. Puoi comunque visualizzare i dati sulle prestazioni dell’intero anno utilizzando la selezione Intervallo date personalizzato.
