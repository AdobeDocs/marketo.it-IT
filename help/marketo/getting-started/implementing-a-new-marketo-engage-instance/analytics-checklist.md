---
description: Configura la sezione Analytics per la nuova istanza di Marketo Engage.
title: Best practice per le nuove istanze - Elenco di controllo di Analytics
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: 6aeb894e6a36064825a25474c67f53a291f548ab
workflow-type: tm+mt
source-wordcount: '1615'
ht-degree: 0%

---

# Best practice per le nuove istanze: elenco di controllo di Analytics {#new-instance-best-practices-analytics-checklist}

La sezione Analytics offre rapporti globali che analizzano le prestazioni delle attività di marketing. Scopri i passaggi necessari per navigarli.

Ricorda a [scaricare gli elenchi di controllo](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) e tieni traccia dei tuoi progressi.

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
    <td><li>Utilizza una convenzione di denominazione dei rapporti per distinguere i rapporti nella scheda Rapporti globali.</li>
    <ul><li>Un esempio di buona pratica per le convenzioni di denominazione è [Tipo di rapporto] [Tag globale vs. BU-Specific] [Descrizione rapporto], ad esempio [Prestazioni e-mail]-[Globale]-[Coinvolgimento e-mail di 180 giorni].</li></ul><br>
    <li>Identifica i rapporti che devono essere condivisi con diversi gruppi di utenti all’interno della tua organizzazione (ad esempio, team di vendita, direzione marketing) e organizza i rapporti per cartella all’interno della cartella Rapporti gruppo in Analytics for Global Reports.</li> 
    <li>L’archiviazione deve essere limitata alla cartella Rapporti globali, in quanto si tratta di rapporti sempre attivi.   <ul>
    <li>Limitare l'archiviazione alle modifiche organizzative, ad esempio la riduzione o l'aggiunta di unità aziendali rilevanti, se il reporting è basato su una struttura di unità aziendali.</li>
    </ul></td>
  </tr>
  <tr>
    <td>Aree di lavoro (se applicabile)</td>
    <td><li>Replica i rapporti globali e la struttura di cartelle in più aree di lavoro per mantenere coerenza nei rapporti per i team. Questi report si trovano nella cartella Report di gruppo.</li></td>
  </tr>
  <tr>
    <td>I miei report</td>
    <td><li>Identifica e crea i rapporti necessari per l’utilizzo in <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/creating-reports/understanding-my-reports-and-group-reports">I miei report</a> sezione. Utilizza questa sezione del rapporto privato come sandbox per i rapporti globali. Sono disponibili solo per l’utente che crea il rapporto.</li>
    <li>Utilizza la convenzione di denominazione della tua organizzazione per identificare il rapporto e il suo utilizzo, in modo da poter riconciliare i rapporti in I miei rapporti con i rapporti in Rapporti di gruppo.</li></td>
  </tr>
  <tr>
    <td>Rapporti sui gruppi</td>
    <td><li>I Report di gruppo sono i Report globali della tua organizzazione e devono riportare l’attività complessiva della tua organizzazione.</li>
    <li>Valuta la creazione <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/clone-a-report-to-group-reports" target="_blank">rapporti core clonabili</a> ci si aspetta che ogni unità aziendale utilizzi più spesso per ridurre il tempo necessario per estrarre il rapporto e garantire la correttezza dei dati. Vedi i dettagli in <a href="#global-reports">Tabella dei report globali di seguito</a>.
    <ul><li>Rapporto sulle prestazioni delle persone (basato su tempo e tempo) per origine, mese</li>
    <li>Rapporto Prestazioni programma (per mese di costo, in base al tempo)</li>
    <li>Rapporto sulle prestazioni delle e-mail (basato sul tempo)</li></ul>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/report-email-campaign-performance-across-workspaces" target="_blank">Attiva "Global Reporting"</a> nella scheda Configurazione del rapporto per includere i dati di tutte le aree di lavoro nei rapporti Prestazioni e-mail e Prestazioni collegamento e-mail. Se disponi di più aree di lavoro, devi abilitarle solo nell’area di lavoro predefinita.</li>
    <p><img src="assets/tip-icon.png" alt="icona nota"> SUGGERIMENTO: creare <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists" target="_blank">Elenco avanzato</a> con i filtri che si desidera includere nella maggior parte dei rapporti nella sezione Database. Se devi aggiornare i criteri dell’elenco avanzato, puoi aggiornarlo in un’unica posizione invece di aggiornarlo in tutti i rapporti globali.</td>
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
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/subscribe-to-a-basic-report">Impostare le sottoscrizioni</a> nella cadenza desiderata (giornaliera/settimanale/mensile) per il monitoraggio continuo di ciascun team. È inoltre possibile <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/manage-report-subscriptions">visualizza tutti gli abbonamenti</a> in un’unica posizione nella scheda Sottoscrizioni in Analytics.</li></td>
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
    <td><li>Crea rapporti globali a livello di area di lavoro/unità aziendale con le e-mail selezionate corrette.</li>
    <li>Crea un rapporto locale sulle prestazioni delle e-mail in tutti i modelli di programma clonabili.</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame">Utilizzare un arco temporale rilevante</a> (ad esempio YTD, ultimi 90 giorni, ecc.) affinché il rapporto fornisca una visualizzazione accurata delle metriche standard di coinvolgimento e consegna delle e-mail.</li>
    <p><img src="assets/tip-icon.png" alt="icona nota"> SUGGERIMENTO: <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/email-setup/filtering-email-bot-activity">Attivare il filtro "Attività bot" in <strong>Amministratore &gt; E-mail</strong></a> per evitare la registrazione o per identificare se la registrazione è abilitata per le attività bot. Includi il filtro solo per consentirlo <a href="https://nation.marketo.com/t5/product-documents/filtering-email-bot-activity-feature-latest-release/ta-p/324860">Attività aperte/selezionate con il vincolo "Attività bot" impostato su "False"</a> nell’elenco avanzato dei rapporti globali clonabili.</td>
  </tr>
  <tr>
    <td>Rapporto prestazioni persone</td>
    <td><img src="assets/note-icon.png" alt="icona nota"> NOTA: si consiglia di disporre di un <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags">strategia di canale e tag</a> per ogni implementazione del Marketo Engage prima di poter monitorare le persone acquisite e il ROI dei tuoi investimenti di marketing per canale.
    <p>
    <li>Determina i criteri da utilizzare per misurare le prestazioni dei programmi di acquisizione dei lead e crea i rapporti standard basati sul tempo (visualizzazione anno corrente, ultimi 12 mesi continui o 180 giorni) in base a queste metriche:</li> <ul><li>Programma di acquisizione: programma di Marketo Engage accreditato per l’acquisizione della persona.</li>
    <li>Origine persona: la categoria di origine per la modalità con cui il record è diventato noto al database (in base all’elenco di origine dei valori nel CRM)
    </li></ul>
    <li>Misura le persone create per settimana o mese. Questo report fornisce una misura del tasso di crescita del database e indica se si sta raggiungendo il limite di dimensione del database.</li>
    <li>Filtrare le metriche nei report sulle prestazioni delle persone per <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/add-custom-columns-to-a-person-report">utilizzo degli elenchi avanzati come colonne personalizzate.</a></li>
    <p><img src="assets/tip-icon.png" alt="icona nota"> SUGGERIMENTO: creare elenchi avanzati per le colonne personalizzate che si desidera aggiungere al rapporto Prestazioni persone nel database anziché alle attività di marketing, in modo da visualizzare correttamente e chiaramente il nome dell'elenco smart quando viene selezionato nel rapporto.</td>
  </tr>
  <tr>
    <td>Rapporto prestazioni programma</td>
    <td><p><img src="assets/note-icon.png" alt="icona nota"> NOTA: questo rapporto richiede che siano definiti i canali, gli stati di progressione e i passaggi di successo in <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/tags/create-a-program-channel"><strong>Amministratore</strong> &gt; <strong>Tag</strong></a>.
    <p>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report">Misura l’efficacia delle tattiche di marketing</a> all'interno di programmi selettivi.</li>
    <li>Gestisci l’iscrizione al programma (utilizzando Campagne avanzate per aggiornare il programma di acquisizione, lo stato e gli stati di successo) in base alle best practice di Marketing Activities (Attività di marketing).</li>
    <li>Misura basata sui costi per l’anno in corso e su 12 mesi consecutivi.
    <ul><li>Tenere presente che <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program">Costi periodo</a> è fondamentale per sfruttare il Rapporto sulle prestazioni del programma.</li></ul>
    <br>
    <br><img src="assets/tip-icon.png" alt="icona nota"> SUGGERIMENTO: per aggregare e visualizzare <a href="https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people">elenchi importati</a> nei Rapporti sulle prestazioni del programma, accertati che i team selezionino il programma di acquisizione appropriato per l’assegnazione di tag. Considerare <a href="https://experienceleague.adobe.com/it/docs/marketo-learn/tutorials/programs-and-campaigns/default-programs/create-and-measure-default-programs">creazione di un programma predefinito</a> da selezionare come programma di acquisizione quando gli elenchi importati non si applicano ad alcun canale. Questo assicura che ogni persona importata disponga di un programma di acquisizione valido relativo all'origine, alla Business Unit, al canale, ecc., invece di un valore vuoto.</td>
  </tr>
  <tr>
    <td>Rapporto sulle prestazioni della pagina di destinazione</td>
    <td><li>Creare <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">Rapporto sulle prestazioni della pagina di destinazione</a> come rapporto globale, per consentirti di <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/filter-a-landing-page-performance-report">filtrare ed esaminare i numeri</a> di tutte le pagine di destinazione di Design Studio/Marketing Activities in un'unica posizione.</li>
    <li>Per i programmi con pagine di destinazione, considera <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">creazione di un report locale dedicato all’interno del modello di programma</a> in modo da poter esaminare le prestazioni a livello di programma.</li></td>
  </tr>
  <tr>
    <td>Rapporto attività pagina web</td>
    <td><img src="assets/note-icon.png" alt="icona nota"> NOTA: solo le pagine web (pagine di destinazione esterne e Marketo) che hanno <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website">JavaScript Munchkin</a> abilitato sarà tracciato in questo rapporto. Prendi in considerazione il posizionamento del codice JavaScript nella piattaforma Tag Management, ad esempio <a href="https://developers.marketo.com/blog/integrating-munchkin-with-google-tag-manager/">Gestione tag Google</a>, per evitare di codificare il codice in ogni pagina web.
    <p>
    <li>Creare <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/web-page-activity-report">Rapporto attività pagina web</a> come rapporto globale che ti consente di esaminare i numeri di tutte le pagine web in un’unica posizione. Tieni presente che le attività esterne della pagina web si riflettono solo nei rapporti Attività pagina web.</li></td>
  </tr>
</tbody>
</table>

## Rapporti locali {#local-reports}

Alcuni rapporti sui Marketi Engage possono essere distribuiti come risorse locali all’interno di programmi specifici in Attività di marketing, in quanto il loro utilizzo tipico è in un set più limitato di programmi e risorse. Prendi in considerazione la creazione di rapporti di base, ad esempio:

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
    <td><li>Creare un <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report" target="_blank">Rapporto prestazioni collegamento e-mail</a> all’interno di programmi che inviano e-mail e campagne drip, per fornirti informazioni sui collegamenti che gli utenti selezionano nelle e-mail inviate.</li></td>
  </tr>
  <tr>
    <td>Rapporto sull’attività della campagna</td>
    <td><li>Creare <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/campaign-activity-report" target="_blank">Rapporto sull’attività della campagna</a> e scegli un periodo all’interno della cartella operativa in Attività di marketing.</li>
    <li>Imposta i rapporti per monitorare i trigger per ogni caso d’uso e <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/filter-a-campaign-activity-report" target="_blank">applicare i filtri della campagna</a> (ad esempio, trigger di Punteggio comportamento, trigger di qualificazione del ciclo di vita, trigger dei momenti di interesse).</li></td>
  </tr>
  <tr>
    <td>Rapporto sulle prestazioni del flusso di coinvolgimento (se applicabile)</td>
    <td><li>Creare un <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/engagement-stream-performance-report" target="_blank">Rapporto sulle prestazioni del flusso di coinvolgimento</a> per misurare l'efficacia dei contenuti e dei flussi distribuiti all'interno del programma di coinvolgimento.</li>
    <li>Valuta l’utilizzo di <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/group-email-reports-by-segmentations" target="_blank">Filtro "Segmentation" (Segmentazione) nella scheda Setup (Configurazione) del rapporto</a> e raggruppamento dei dati di reporting per <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation" target="_blank">segmento</a> (ad esempio, origine della persona o settore) utilizzato nel programma di coinvolgimento. Questo ti aiuterà a ottenere informazioni più approfondite sui pattern di coinvolgimento di ogni segmento, guidandoti verso modifiche strategiche per migliorare il tuo programma di coinvolgimento (contenuto, flusso, frequenza di flusso, ecc.).</li></td>
  </tr>
</tbody>
</table>

TABELLA CON PUNTI ELENCO FUNZIONANTI

<table>
<tbody>
<tr>
    <td>Rapporti sui gruppi</td>
    <td><img src="assets/note-icon.png" alt="icona nota"> NOTA: TESTO.
    <p>
    <li>TESTO.</li>
    <li>TESTO.
    <ul><li>TESTO</li>
    <li>TESTO</li></ul>
    <li>TESTO.</li>
    <li>TESTO.</li>
    <p><img src="assets/tip-icon.png" alt="icona nota"> SUGGERIMENTO: TESTO.</td>
  </tr>
  </tbody>
</table>

TEST FIX 1

<table>
<tbody>
<tr>
    <td>Rapporto prestazioni persone</td>
    <td><img src="assets/note-icon.png" alt="icona nota"> NOTA: si consiglia di disporre di un <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags">strategia di canale e tag</a> per ogni implementazione del Marketo Engage prima di poter monitorare le persone acquisite e il ROI dei tuoi investimenti di marketing per canale.
    <p>
    <li>Determina i criteri da utilizzare per misurare le prestazioni dei programmi di acquisizione dei lead e crea i rapporti standard basati sul tempo (visualizzazione anno corrente, ultimi 12 mesi continui o 180 giorni) in base a queste metriche:</li>
    <ul><li>Programma di acquisizione: programma di Marketo Engage accreditato per l’acquisizione della persona</li>
    <li>Origine persona: la categoria di origine per la modalità con cui il record è diventato noto al database (in base all’elenco di origine dei valori nel CRM)</li></ul>
    <li>Misura le persone create per settimana o mese. Questo report fornisce una misura del tasso di crescita del database e indica se si sta raggiungendo il limite di dimensione del database.</li>
    <li>Filtrare le metriche nei report sulle prestazioni delle persone per <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/add-custom-columns-to-a-person-report">utilizzo degli elenchi avanzati come colonne personalizzate.</a></li>
    <p><img src="assets/tip-icon.png" alt="icona nota"> SUGGERIMENTO: creare elenchi avanzati per le colonne personalizzate che si desidera aggiungere al rapporto Prestazioni persone nel database anziché alle attività di marketing, in modo da visualizzare correttamente e chiaramente il nome dell'elenco smart quando viene selezionato nel rapporto.</td>
  </tr>
  </tbody>
</table>
