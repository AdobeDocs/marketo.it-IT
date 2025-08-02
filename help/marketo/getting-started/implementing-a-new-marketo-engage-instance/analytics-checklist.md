---
description: Configura la sezione Analytics per la nuova istanza di Marketo Engage.
title: Best practice per le nuove istanze - Elenco di controllo di Analytics
feature: Getting Started
exl-id: ddbb9bc7-d06a-4a2e-a560-9d308630ae3f
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 0%

---

# Best practice per le nuove istanze: elenco di controllo di Analytics {#new-instance-best-practices-analytics-checklist}

La sezione Analytics offre rapporti globali che analizzano le prestazioni delle attività di marketing. Scopri i passaggi necessari per navigarli.

Ricordati di [scaricare le liste di controllo](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) e tenere traccia dell&#39;avanzamento.

## Albero {#tree}

<table>
<thead>
  <tr>
    <th style="width:20%">Area</th>
    <th style="width:80%">Elementi azione</th>
    <th></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Organizzazione: denominazione, cartelle e archiviazione</td>
    <td><li>Utilizza una convenzione di denominazione dei rapporti per distinguere i rapporti nella scheda Rapporti globali.
    <ul><li>Un esempio di buona pratica per le convenzioni di denominazione è [Tipo di rapporto] [Tag globale vs. BU-Specific] [Descrizione rapporto], ad esempio [Prestazioni e-mail]-[Globale]-[Coinvolgimento e-mail di 180 giorni].</li></ul><br>
    <li>Identifica i rapporti che devono essere condivisi con diversi gruppi di utenti all’interno della tua organizzazione (ad esempio, team di vendita, direzione marketing) e organizza i rapporti per cartella all’interno della cartella Rapporti gruppo in Analytics for Global Reports.</li>
    <li>L’archiviazione deve essere limitata alla cartella Rapporti globali, in quanto si tratta di rapporti sempre attivi.   <ul><li>Limitare l'archiviazione alle modifiche organizzative, ad esempio la riduzione o l'aggiunta di unità aziendali rilevanti, se il reporting è basato su una struttura di unità aziendali.</li></ul>
    </td>
  </tr>
  <tr>
    <td>Aree di lavoro (se applicabile)</td>
    <td><li>Replica i rapporti globali e la struttura di cartelle in più aree di lavoro per mantenere coerenza nei rapporti per i team. Questi report si trovano nella cartella Report di gruppo.</li></td>
  </tr>
  <tr>
    <td>I miei report</td>
    <td><li>Identifica e crea i report necessari per l'utilizzo nella sezione <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/reporting/basic-reporting/creating-reports/understanding-my-reports-and-group-reports">I miei report</a>. Utilizza questa sezione del rapporto privato come sandbox per i rapporti globali. Sono disponibili solo per l’utente che crea il rapporto.</li>
    <li>Utilizza la convenzione di denominazione della tua organizzazione per identificare il rapporto e il suo utilizzo, in modo da poter riconciliare i rapporti in I miei rapporti con i rapporti in Rapporti di gruppo.</li></td>
  </tr>
  <tr>
    <td>Rapporti sui gruppi</td>
    <td><li>I Report di gruppo sono i Report globali della tua organizzazione e devono riportare l’attività complessiva della tua organizzazione.</li>
    <li>Prendi in considerazione la creazione di <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/clone-a-report-to-group-reports" target="_blank">report di base clonabili</a>. Prevedi che ogni unità aziendale utilizzi il più delle volte per ridurre il tempo necessario per estrarre il report e garantire la correttezza dei dati. Vedi i dettagli nella tabella <a href="#global-reports">Global Reports di seguito</a>.
    <ul><li>Rapporto sulle prestazioni delle persone (basato su tempo e tempo) per origine, mese</li>
    <li>Rapporto Prestazioni programma (per mese di costo, in base al tempo)</li>
    <li>Rapporto sulle prestazioni delle e-mail (basato sul tempo)</li></ul>
    <li><a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/report-email-campaign-performance-across-workspaces" target="_blank">Attiva "Generazione rapporti globali"</a> nella scheda Configurazione del report per includere i dati di tutte le aree di lavoro nei report Prestazioni e-mail e Prestazioni collegamento e-mail. Se disponi di più aree di lavoro, devi abilitarle solo nell’area di lavoro predefinita.</li>
    <p><img src="assets/tip-icon.png" alt="icona nota"> SUGGERIMENTO: creare l'<a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists" target="_blank">elenco avanzato</a> con i filtri che si desidera includere nella maggior parte dei report nella sezione Database. Se devi aggiornare i criteri dell’elenco avanzato, puoi aggiornarlo in un’unica posizione invece di aggiornarlo in tutti i rapporti globali.</td>
  </tr>
</tbody>
</table>

## Abbonamenti {#subscriptions}

<table>
<thead>
  <tr>
    <th style="width:20%">Area</th>
    <th style="width:80%">Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Abbonamenti</td>
    <td><li>Allinea il tuo responsabile marketing per quanto riguarda le persone che devono esaminare i risultati dei rapporti e la loro cadenza durante l’implementazione.</li> <li>Utilizza gli abbonamenti per distribuire i dati alle persone che hanno bisogno di conoscere nella tua organizzazione senza esaurire una licenza per utente con nome.</li>
    <p><img src="assets/tip-icon.png" alt="icona nota"> SUGGERIMENTO: se desideri che le persone accedano ai dati del rapporto in tempo reale, devi aggiungerli come utenti in modo che possano visualizzare il rapporto.
    <p>
    <li><a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/subscribe-to-a-basic-report">Imposta abbonamenti</a> nella cadenza desiderata (giornaliera/settimanale/mensile) per il monitoraggio continuo di ogni team. È inoltre possibile <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/manage-report-subscriptions">visualizzare tutte le sottoscrizioni</a> in un'unica posizione nella scheda Sottoscrizioni di Analytics.</li></td>
  </tr>
</tbody>
</table>

## Rapporti globali {#global-reports}

Identifica i rapporti che devono essere condivisi con diversi gruppi di utenti all’interno della tua organizzazione (ad esempio, team di vendita, leadership di marketing). Creare una struttura di cartelle appropriata per ogni team/gruppo di utenti/business unit per organizzare i report clonati all&#39;interno di Report di gruppo. Valuta la possibilità di impostare rapporti globali, ad esempio:

<table>
<thead>
  <tr>
    <th style="width:20%">Tipo di rapporto</th>
    <th style="width:80%">Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Rapporto prestazioni e-mail</td>
    <td><li>Creare rapporti globali a livello di Workspace/Business Unit con le e-mail selezionate corrette.</li>
    <li>Crea un rapporto locale sulle prestazioni delle e-mail in tutti i modelli di programma clonabili.</li>
    <li><a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame">Utilizza un periodo di tempo rilevante</a> (ad esempio, da inizio anno, ultimi 90 giorni, ecc.) per il report per fornire una visualizzazione accurata delle metriche standard di coinvolgimento e recapito messaggi e-mail.</li>
    <p><img src="assets/tip-icon.png" alt="icona nota"> SUGGERIMENTO: <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/email-setup/filtering-email-bot-activity">Attiva il filtro 'Attività bot' in <strong>Amministratore &gt; E-mail</strong></a> per evitare la registrazione o per identificare se la registrazione è abilitata per le attività bot. Includi il filtro per consentire solo <a href="https://nation.marketo.com/t5/product-documents/filtering-email-bot-activity-feature-latest-release/ta-p/324860">attività aperte/selezionate con il vincolo "Is Bot Activity" impostato su "False"</a> nell'elenco avanzato dei report globali clonabili.</td>
  </tr>
  <tr>
    <td>Rapporto prestazioni persone</td>
    <td><img src="assets/note-icon.png" alt="icona nota"> NOTA: si consiglia di disporre di una <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags">strategia per canali e tag</a> appropriata per ogni implementazione di Marketo Engage prima di poter tenere traccia delle persone acquisite e del ROI degli investimenti di marketing per canale.
    <p>
    <li>Determina i criteri da utilizzare per misurare le prestazioni dei programmi di acquisizione dei lead e crea i rapporti standard basati sul tempo (visualizzazione anno corrente, ultimi 12 mesi continui o 180 giorni) in base a queste metriche: <ul><li>Programma di acquisizione: programma Marketo Engage accreditato per l'acquisizione della persona.</li>
    <li>Source persona: la categoria di origine per la modalità con cui il record è diventato noto al database (in base all’elenco di origine dei valori nel CRM)
    </li></ul>
    <li>Misura le persone create per settimana o mese. Questo report fornisce una misura del tasso di crescita del database e indica se si sta raggiungendo il limite di dimensione del database.</li>
    <li>Filtra le metriche nei report sulle prestazioni delle persone in base a <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/add-custom-columns-to-a-person-report">utilizzando gli elenchi avanzati come colonne personalizzate.</a></li>
    <p><img src="assets/tip-icon.png" alt="icona nota"> SUGGERIMENTO: creare elenchi avanzati per le colonne personalizzate che si desidera aggiungere al rapporto Prestazioni persone nel database anziché alle attività di marketing, in modo da visualizzare correttamente e chiaramente il nome dell'elenco smart quando viene selezionato nel rapporto.</td>
  </tr>
  <tr>
    <td>Rapporto prestazioni programma</td>
    <td><p><img src="assets/note-icon.png" alt="icona nota"> NOTA: questo report richiede che i tuoi canali, stati di progressione e passaggi di successo siano definiti in <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/tags/create-a-program-channel"><strong>Amministratore</strong> &gt; <strong>Tag</strong></a>.
    <p>
    <li><a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report">Misura l'efficacia delle tue tattiche di marketing</a> all'interno dei programmi selettivi.</li>
    <li>Gestisci l’iscrizione al programma (utilizzando Campagne avanzate per aggiornare il programma di acquisizione, lo stato e gli stati di successo) in base alle best practice di Marketing Activities (Attività di marketing).</li>
    <li>Misura basata sui costi per l’anno in corso e su 12 mesi consecutivi.
    <ul><li>Tenere presente che la gestione di <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program">Costi del periodo</a> è fondamentale per sfruttare il report sulle prestazioni del programma.</li></ul></li>
    <p>
    <img src="assets/tip-icon.png" alt="icona nota"> SUGGERIMENTO: per aggregare e visualizzare eventuali <a href="https://experienceleague.adobe.com/it/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people">elenchi importati</a> nei report sulle prestazioni del programma, assicurati che i team selezionino il programma di acquisizione appropriato per l'assegnazione di tag. Considera <a href="https://experienceleague.adobe.com/it/docs/marketo-learn/tutorials/programs-and-campaigns/default-programs/create-and-measure-default-programs">la creazione di un programma predefinito</a> da selezionare come programma di acquisizione se gli elenchi importati non si applicano ad alcun canale. Questo assicura che ogni persona importata disponga di un programma di acquisizione valido relativo all'origine, alla Business Unit, al canale, ecc., invece di un valore vuoto.</td>
  </tr>
  <tr>
    <td>Rapporto sulle prestazioni della pagina di destinazione</td>
    <td><li>Crea il <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">Rapporto sulle prestazioni della pagina di destinazione</a> come rapporto globale, in modo da poter <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/filter-a-landing-page-performance-report">filtrare e rivedere i numeri</a> di tutte le pagine di destinazione di Design Studio/Marketing Activities in un'unica posizione.</li>
    <li>Per i programmi con pagine di destinazione, è consigliabile <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">creare un report locale dedicato all'interno del modello di programma</a> per esaminare le prestazioni a livello di programma.</li></td>
  </tr>
  <tr>
    <td>Rapporto attività pagina web</td>
    <td><img src="assets/note-icon.png" alt="icona nota"> NOTA: solo le pagine Web (pagine di destinazione esterne e Marketo) in cui è abilitato <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website">Munchkin JavaScript</a> verranno tracciate in questo report. È consigliabile inserire il codice JavaScript nella piattaforma Tag Management, ad esempio <a href="https://developers.marketo.com/blog/integrating-munchkin-with-google-tag-manager/">Google Tag Manager</a>, per evitare di codificare il codice in ogni pagina Web.
    <p>
    <li>Crea il <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/web-page-activity-report">report attività pagina Web</a> come report globale in modo da poter esaminare i numeri di tutte le pagine Web in un'unica posizione. Tieni presente che le attività esterne della pagina web si riflettono solo nei rapporti Attività pagina web.</li></td>
  </tr>
</tbody>
</table>

## Rapporti locali {#local-reports}

Alcuni rapporti di Marketo Engage possono essere distribuiti come risorse locali all’interno di programmi specifici nelle attività di marketing, in quanto il loro utilizzo tipico si basa su un set più limitato di programmi e risorse. Prendi in considerazione la creazione di rapporti di base, ad esempio:

<table>
<thead>
  <tr>
    <th style="width:20%">Tipo di rapporto</th>
    <th style="width:80%">Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Rapporto prestazioni collegamento e-mail</td>
    <td><li>Crea un <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report" target="_blank">Rapporto sulle prestazioni dei collegamenti e-mail</a> all'interno dei programmi che inviano e-mail e delle campagne drip per fornirti informazioni sui collegamenti su cui gli utenti fanno clic nelle e-mail inviate.</li></td>
  </tr>
  <tr>
    <td>Rapporto sull’attività della campagna</td>
    <td><li>Crea il <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/campaign-activity-report" target="_blank">Rapporto sull'attività della campagna</a> e scegli un periodo all'interno della cartella operativa in Attività di marketing.</li>
    <li>Imposta i report per monitorare i trigger per ogni caso d'uso e <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/filter-a-campaign-activity-report" target="_blank">applicare i filtri della campagna</a> (ad esempio trigger di Punteggio comportamento, trigger di qualificazione del ciclo di vita, trigger dei momenti di interesse).</li></td>
  </tr>
  <tr>
    <td>Rapporto sulle prestazioni del flusso di coinvolgimento (se applicabile)</td>
    <td><li>Crea un <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/engagement-stream-performance-report" target="_blank">report sulle prestazioni del flusso di coinvolgimento</a> per misurare l'efficacia dei contenuti e del flusso distribuiti all'interno del programma di coinvolgimento.</li>
    <li>Valuta se utilizzare il filtro <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/group-email-reports-by-segmentations" target="_blank">"Segmentation" nella scheda Configurazione del report</a> e raggruppare i dati di reporting per il <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation" target="_blank">segmento</a> (ad esempio, origine persona, settore) utilizzato nel programma di coinvolgimento. Questo ti aiuterà a ottenere informazioni più approfondite sui pattern di coinvolgimento di ogni segmento, guidandoti verso modifiche strategiche per migliorare il tuo programma di coinvolgimento (contenuto, flusso, frequenza di flusso, ecc.).</li></td>
  </tr>
</tbody>
</table>
