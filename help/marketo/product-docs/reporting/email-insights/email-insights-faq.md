---
unique-page-id: 10100257
description: Domande frequenti su Approfondimenti e-mail - Documenti Marketo - Documentazione del prodotto
title: Domande frequenti su Approfondimenti e-mail
exl-id: de3aca5a-08b4-4af8-ab92-675cb46dcbb2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Domande frequenti su Approfondimenti e-mail {#email-insights-faq}

## Esistono differenze tra le metriche delle proporzioni con Approfondimenti e-mail e altri rapporti e-mail di Marketo? {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

Sì. E-mail Insights mette in correlazione le metriche di coinvolgimento con le metriche di consegna corrispondenti per la stessa e-mail inviata quando si calcolano i rapporti delle metriche di coinvolgimento (tasso di apertura, tasso di clic-su-apertura, tasso di annullamento sottoscrizione). Ad esempio, in Approfondimenti e-mail, quando osservi un grafico a serie temporale nell’ultima settimana con raggruppamenti giornalieri di Click-to-Open-Rate, ora viene mostrato il rapporto effettivo e correlato degli eventi di apertura/clic/annullamento dell’abbonamento in base alle metriche di consegna corrispondenti. Questo è in contrasto con il comportamento in Revenue Explorer, che semplicemente riassume tutto. E-mail Insights offre una visualizzazione più accurata dei rapporti di coinvolgimento.

## Perché e-mail Insights supporta solo 10 Dimension personalizzati? {#why-does-email-insights-only-support-custom-dimensions}

Per molti casi d’uso, l’estensione delle dimensioni di sistema predefinite con 10 dimensioni personalizzate aggiuntive sarà più che adeguata e include dimensioni personalizzate in base a Segmenti o Tag programma. In futuro, consentiremo ai clienti di aumentare il numero di Dimension personalizzati consentiti.

## Perché non è possibile riutilizzare gli slot di Dimension personalizzati dopo che sono stati assegnati? {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

Una volta allocato uno slot di Dimension personalizzato specifico, la nuova mappatura causerebbe un errore nei dati precedenti quando vengono mescolati con un nuovo significato. Per questo motivo, è possibile che gli slot di Dimension personalizzati non vengano riutilizzati. Questo comportamento è coerente con quello di altri strumenti di analisi delle metriche, come le Google Analytics.

## E-mail Insights supporta le e-mail Marketo Sales Insight? {#does-email-insights-support-marketo-sales-insight-emails}

Sì. Tutte le e-mail inviate tramite Marketo Sales Insights sono incluse in Email Insights.

## E-mail Insights supporta le e-mail operative? {#does-email-insights-support-operational-emails}

Sì. Per impostazione predefinita, le e-mail operative sono nascoste per visualizzare e interrogare. Tuttavia, puoi modificare questa impostazione nel pannello Impostazioni personali .

## Gli approfondimenti e-mail acquisiscono i passaggi ricorrenti pianificati o rieseguiti del flusso di e-mail di Smart Campaign? {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

Sì e No. Con la versione iniziale di E-mail Insights, tutti gli eventi e-mail vengono acquisiti e accessibili per qualsiasi campagna avanzata pianificata o rieseguita periodicamente. Ma non sarai in grado di distinguere tra diverse esecuzioni di quella Smart Campaign. Stiamo aggiungendo supporto nella prossima versione per acquisire le informazioni di esecuzione di Smart Campaign per gli eventi Apri, Fai clic e Annulla sottoscrizione al fine di differenziare.

## Perché molte metriche mostrano zero quando si filtra per tipo di dispositivo o sistema operativo del dispositivo? {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

Ad eccezione di Click-to-Open-Rate, Aperture, Clic e Annulla sottoscrizione, tutte le altre metriche supportate sono eventi di consegna o rapporti derivati da eventi di consegna. Poiché il tipo di dispositivo e il sistema operativo del dispositivo si applicano solo alle metriche di coinvolgimento, non disponiamo semplicemente delle informazioni da visualizzare. Ad esempio, è una query non definita per richiedere il tasso di consegna quando viene filtrato per tipo di dispositivo = mobile, poiché Marketo non avrebbe ricevuto alcuna metrica di coinvolgimento per gli eventi di consegna e invio sottostanti. Stiamo esplorando modi per applicare il tipo di dispositivo e il sistema operativo del dispositivo dalle metriche di coinvolgimento per rapporti comprendenti sia le metriche di coinvolgimento che di consegna.

## Cosa fa Email Insights quando determinati client e-mail bloccano le immagini? {#what-does-email-insights-do-when-certain-email-clients-block-images}

Un problema comune del settore è che un numero crescente di client e-mail sta disattivando le immagini per impostazione predefinita. Il caricamento delle immagini è la base per la registrazione di Aperture . È del tutto possibile che un utente riceva un&#39;e-mail con immagini bloccate, ma con il testo e i collegamenti completamente leggibili. Se un utente ha fatto clic su un collegamento presente nell’e-mail, si finisce per avere uno scenario di un evento Click, ma non un evento Open corrispondente per tale e-mail. Marketo Email Insights genera automaticamente tutti gli eventi mancanti. La logica è identica a quella utilizzata da Marketo per il rapporto Prestazioni e-mail e per l’area Analisi e-mail in Revenue Explorer.
