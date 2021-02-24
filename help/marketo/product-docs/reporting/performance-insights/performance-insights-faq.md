---
unique-page-id: 12979858
description: Domande frequenti sulle prestazioni - Documenti Marketo - Documentazione prodotto
title: Domande frequenti sulle prestazioni
translation-type: tm+mt
source-git-commit: cb7df3dd38275837f8ab05ce846c2c68ab78462f
workflow-type: tm+mt
source-wordcount: '1357'
ht-degree: 0%

---


# Domande frequenti sulle prestazioni {#performance-insights-faq}

## Qual è la definizione di &quot;successo&quot; nella scheda Partecipazione? {#what-is-the-definition-of-success-in-the-engagement-tab}

Il successo è una misura dell&#39;interazione significativa in Marketo. Lo scopo di un programma è quello di creare un&#39;interazione significativa con la persona o il potenziale. Il successo è indicato quando una persona raggiunge lo stato che raggiunge tale obiettivo. Può trattarsi della partecipazione a un webinar, di un clic su un collegamento in un messaggio e-mail o di una compilazione di un modulo Web. Il successo varia a seconda del canale del programma.

>[!NOTE]
>
>In un programma webinar possono essere presenti più stati, ad esempio: Invitati, Registrati e Partecipati. Invitati o Registrati non sono interazioni significative perché le persone non guardano il webinar. Partecipato è considerato un successo in questo caso.

## MPI funziona con CRM? {#will-mpi-work-with-any-crm}

Sì. Tecnicamente, MPI non interagisce direttamente con CRM per la sincronizzazione dei dati. MPI utilizza i dati memorizzati nell’Data Warehouse di Marketing Cloud Analytics. Poiché la sincronizzazione CRM avviene nell&#39;applicazione Gestione lead, qualsiasi CRM supportato da Marketo integrato con l&#39;applicazione Gestione lead mostrerà correttamente i dati. Tuttavia, i campi delle opportunità CRM devono essere mappati correttamente sui campi delle opportunità Marketo.

## Non dispongo di altri prodotti Marketing Analytics (ARB, RCE, RCA, Program Analysis). MPI funzionerà per me? {#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

MPI è un componente aggiuntivo indipendente per l’applicazione Gestione lead. Non richiede l&#39;utilizzo di altri prodotti di analisi.

## RCA mostra anche i dati sulle prestazioni del programma. Esiste una differenza tra i dati visualizzati in MPI e RCA? {#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

No. MPI origini dati dallo stesso data warehouse di RCA. Pertanto, non verranno visualizzate differenze di dati tra i due. RCA consente di creare rapporti personalizzati al volo. L&#39;MPI consente di accedere a dashboard visivi di facile comprensione.

## Non voglio che alcuni dei miei programmi (ad es. operativi) vengano visualizzati in MPI. Come posso controllare la visibilità di programmi specifici? {#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

Potete controllare la visibilità dei programmi impostando il comportamento di Analytics dei programmi su Operativo. In questo modo il programma verrà escluso dai calcoli di analisi.

>[!NOTE]
>
>Ulteriori informazioni sull&#39;impostazione del comportamento di analisi [qui](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/edit-analytics-behavior-settings.md).

## Sto eseguendo una campagna multi-canale per un nuovo lancio di prodotto. Come è possibile visualizzare le prestazioni di questa campagna su tutti i diversi canali in un&#39;unica posizione? {#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

Per i programmi che fanno parte di tale campagna, si consiglia di utilizzare i tag dei programmi. I tag del programma vengono sincronizzati automaticamente in MPI e potete filtrarli in tutte le dashboard MPI per visualizzare le prestazioni delle campagne multicanale.

## Posso accedere alle impostazioni di attribuzione se non ho RCA? {#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

Se disponete di MPI, potete accedere alle impostazioni di attribuzione, indipendentemente dal fatto che possiate RCA o meno.

## Quando si effettua l’accesso, viene visualizzato un avviso in MPI in cui viene indicato che le impostazioni di attribuzione non sono corrette. Cosa c&#39;è che non va? {#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

MPI calcola se tutte le opportunità vengono incluse nell&#39;analisi. In caso contrario, verrà richiesto di modificare le impostazioni di attribuzione (Explicit, Implicit, Hybrid) per includere ulteriori opportunità.

Potrebbero mancare anche le opportunità a causa del costo del programma mancante nei programmi. Controlla il comportamento di Analytics dei tuoi programmi. Possono essere:

1. Impostazione predefinita: il comportamento predefinito è che il programma viene incluso in MPI SOLO se è presente almeno un costo periodo, anche uno con zero dollari assegnati.

1. Inclusivo: questa opzione garantisce che il programma sia disponibile in MPI indipendentemente dal fatto che abbiate incluso o meno un costo periodo.

1. [Operativo](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs.md#operational-programs)  - Questa opzione fa sì che il programma non venga visualizzato in MPI.

>[!NOTE]
>
>Costo periodo **ha** da impostare per il reporting Success e New Names nel pannello Partecipazione. Questo dashboard utilizza i dati Costo periodo per aggregare i successi e i nuovi nomi. Se Costo periodo non è impostato, il dashboard di coinvolgimento non reagirà correttamente indipendentemente dalle impostazioni di comportamento di Analytics riportate sopra.

## Perché sto perdendo alcune opportunità in MPI? {#why-am-i-missing-some-opportunities-in-mpi}

Due motivi principali per cui potrebbero mancare opportunità in MPI sono:

1. L&#39;impostazione di attribuzione è impostata su Esplicito, ma alle opportunità non è assegnato alcun ruolo di contatto
1. Il costo del periodo non è incluso nei programmi

MPI calcola se tutte le opportunità vengono incluse nell&#39;analisi. In caso contrario, verrà richiesto di modificare le impostazioni di attribuzione (Explicit, Implicit, Hybrid) per includere ulteriori opportunità.

Potrebbero mancare anche le opportunità a causa del costo del programma mancante nei programmi. L&#39;avviso verrà lanciato ma non indica a quali programmi mancano i costi. Verificare la configurazione del programma per includere i costi, per assicurarsi che tutti i programmi e le opportunità siano inclusi in MPI.

## Perché non visualizzo i filtri Custom Fields, Opportunity Type e ABM nel dashboard Engagement? {#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

Campi personalizzati, Tipo opportunità e Filtri ABM sono tutti attributi relativi a un’opportunità. Il pannello Partecipazione consente di misurare il coinvolgimento e l&#39;acquisizione principale, indipendentemente dal fatto che siano associati o meno a un&#39;opportunità. Poiché il pannello Partecipazione non prende in considerazione l&#39;opportunità, i campi personalizzati, il tipo di opportunità e i filtri ABM non si applicano.

## Desidero utilizzare un campo Opportunità Salesforce personalizzata per la generazione di rapporti sulle entrate invece del campo Importo opportunità Salesforce standard. L&#39;MPI mi permetterà di farlo? {#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

Sì. [Il ](https://nation.marketo.com/t5/Support/ct-p/Support) supporto marketing consente di rimappare il campo Importo opportunità di Marketo in un campo Opportunità Salesforce personalizzata, purché il tipo di campo sia valuta. Poiché MPI punta al campo Importo opportunità marketing, MPI può utilizzare i dati del campo Salesforce personalizzato modificato.

>[!NOTE]
>
>Dopo la modifica, MPI mostrerà i dati in corso. L&#39;importo storico non verrà modificato.

## Se non utilizzo le opportunità, posso comunque utilizzare MPI? {#if-i-don-t-use-opportunities-can-i-still-use-mpi}

MPI è progettato per consentire di misurare le prestazioni del programma dalla parte superiore dell&#39;imbuto fino all&#39;impatto sulle entrate. Se non usi le opportunità, potrai comunque:

* Visualizzare le prestazioni dei programmi di formazione per il coinvolgimento del pubblico.
* Visualizza le prestazioni dei tuoi programmi di acquisizione principali.
* Visualizzare le prestazioni delle campagne multicanale tramite i tag dei programmi.
* Scopri le tendenze di coinvolgimento del pubblico negli ultimi 12 mesi.
* Salvare ed esportare i dati sulle prestazioni in PowerPoint.

## Posso misurare il successo delle strategie basate sugli account in MPI? {#can-i-measure-the-success-of-account-based-strategies-in-mpi}

Sì. MPI si integra con [Marketo TAM](https://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview) per inserire gli elenchi degli account ABM in MPI senza soluzione di continuità. Potete utilizzare il filtro ABM Account List per scegliere l&#39;elenco ABM desiderato per filtrare i dati in base a.

## L&#39;attribuzione è immediatamente disponibile quando si acquista MPI? {#is-attribution-instantly-available-when-i-purchase-mpi}

Le funzionalità di attribuzione marketing sono disponibili per i nostri clienti quando acquistano MPI. Tuttavia, [la corretta configurazione](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md) è necessaria per garantire che le opportunità e i dati del programma vengano immessi correttamente in MPI.

## Cosa devo fare per impostare l&#39;attribuzione? {#what-do-i-have-to-do-to-set-up-attribution}

1. Impostazione opportunità

   1. Assicurati che le opportunità siano sincronizzate con CRM
   1. Se le impostazioni Attribuzione sono impostate su Esplicito, accertati che i ruoli di contatto sulle opportunità siano compilati
   1. Consigliamo di modificare l&#39;impostazione Attribuzione in Ibrido
   1. Impostazione programma

      1. Includere i costi del programma nei programmi
      1. Controllare il comportamento di analisi per indicare se un programma deve essere incluso nell&#39;analisi
      1. Impostare i criteri di successo per ogni canale
      1. Lega persona ai programmi

         1. Accertati che il programma di acquisizione e la data di acquisizione siano stati impostati per ogni persona presente nel tuo database al fine di poter utilizzare la funzione First Touch Attribution.
         1. Verificare che i programmi impostino gli stati di successo per gli utenti nel database

>[!TIP]
>
>Tutti i passaggi di configurazione richiesti sono descritti in [questo articolo](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md).

## Qual è la differenza tra MPI e Program Analyzer? {#whats-the-difference-between-mpi-and-the-program-analyzer}

Il programma Analyzer consente di confrontare i programmi in quattro misure. MPI consente di analizzare il canale e il contributo del programma per una metrica scelta, come Successo, Nuove opportunità create, ecc. Consente inoltre di visualizzare la tendenza dei canali a 12 mesi in base a una metrica specifica scelta.

## Qual è la differenza tra MPI e il Report Builder avanzato? {#whats-the-difference-between-mpi-and-the-advanced-report-builder}

Il Report Builder Avanzato (a volte denominato RCE) è progettato per la generazione di rapporti self-service (o ad hoc), solitamente eseguiti dalle Operazioni di Marketing. MPI è progettato per consentire ai leader di marketing e agli esperti di marketing di accedere con un solo clic all&#39;analisi delle prestazioni. È necessaria una configurazione minima.

## Cos’è successo all’opzione &quot;Anno precedente&quot; nel filtro data contributo? {#what-happened-to-the-previous-year-option-in-contributions-date-filter}

Abbiamo temporaneamente rimosso la selezione &quot;Anno precedente&quot;. È comunque possibile visualizzare i dati delle prestazioni dell&#39;intero anno utilizzando la selezione Intervallo date personalizzato.
