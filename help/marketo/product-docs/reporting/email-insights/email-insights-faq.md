---
unique-page-id: 10100257
description: Domande frequenti su Email Insights - Documentazione di Marketo - Documentazione del prodotto
title: Domande frequenti su Email Insights
exl-id: de3aca5a-08b4-4af8-ab92-675cb46dcbb2
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Domande frequenti su Email Insights {#email-insights-faq}

## Esistono differenze tra le metriche del rapporto con Email Insights e altri rapporti e-mail di Marketo? {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

Sì. Email Insights mette in correlazione le metriche di coinvolgimento con le metriche di consegna corrispondenti per la stessa e-mail inviata quando si calcolano i rapporti delle metriche di coinvolgimento (Percentuale di apertura, Percentuale di clic per apertura, Percentuale di annullamento dell’abbonamento). Ad esempio, in Email Insights, quando osservi un grafico a serie temporali nell’ultima settimana con raggruppamenti giornalieri di click-to-open-rate, ora mostriamo il rapporto effettivo correlato tra eventi di apertura, clic e annullamento dell’abbonamento in base alle metriche di consegna corrispondenti. Ciò è in contrasto con il comportamento di Esplora entrate, che semplicemente riassume tutto. Email Insights offre una visualizzazione più precisa dei rapporti di coinvolgimento.

## Perché Email Insights supporta solo 10 Dimension personalizzati? {#why-does-email-insights-only-support-custom-dimensions}

Per molti casi d’uso, l’estensione delle dimensioni di sistema predefinite con 10 dimensioni personalizzate aggiuntive sarà più che adeguata e includerà dimensioni personalizzate basate su Segmentazioni o Tag programma. In futuro, prevediamo di consentire ai clienti di aumentare il numero di Dimension personalizzati consentiti.

## Perché non è possibile riutilizzare gli slot Dimension personalizzati dopo averli assegnati? {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

Una volta allocato uno slot di Dimension personalizzato, la modifica della mappatura causerebbe la generazione di un errore nei dati precedenti in caso di fusione con un nuovo significato. Per questo motivo, gli slot di Dimension personalizzati non possono essere riutilizzati. Questo comportamento è coerente con quello di altri strumenti di analisi metrica, come le Google Analytics.

## Email Insights supporta le e-mail di Marketo Sales Insight? {#does-email-insights-support-marketo-sales-insight-emails}

Sì. Tutte le e-mail inviate tramite Approfondimenti vendite Marketo sono incluse in Approfondimenti e-mail.

## Email Insights supporta le e-mail operative? {#does-email-insights-support-operational-emails}

Sì. Per impostazione predefinita, le e-mail operative sono nascoste dalla visualizzazione e dall’esecuzione di query. Tuttavia, potete modificare questa impostazione nel pannello Impostazioni personali.

## Email Insights acquisisce i passaggi ricorrenti del flusso e-mail pianificati o rieseguiti di Smart Campaign? {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

Sì e No. Con la versione iniziale di Email Insights, tutti gli eventi e-mail vengono acquisiti e accessibili per qualsiasi campagna Smart ricorrente pianificata o rieseguita. Ma non potrai distinguere tra diverse esecuzioni di quella campagna avanzata. Nella prossima versione verrà aggiunto il supporto necessario per acquisire le informazioni di esecuzione di Smart Campaign per gli eventi Apri, Clic e Annulla iscrizione al fine di differenziarli.

## Perché molte metriche mostrano lo zero quando si filtra per tipo di dispositivo o SO del dispositivo? {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

Ad eccezione di Tasso di clic per apertura, Aperture, Clic e Annullamenti abbonamenti, tutte le altre metriche supportate sono eventi di consegna o rapporti derivati da eventi di consegna. Poiché il tipo di dispositivo e il sistema operativo del dispositivo si applicano solo alle metriche di coinvolgimento, le informazioni da visualizzare non sono disponibili. Ad esempio, si tratta di una query non definita per richiedere la Percentuale di Consegna quando viene filtrata per Tipo di Dispositivo = mobile, in quanto Marketo non avrebbe ricevuto alcuna metrica di Coinvolgimento per gli eventi di Consegna e Inviato sottostanti. Stiamo esplorando modi per applicare il tipo di dispositivo e il sistema operativo del dispositivo dalle metriche di coinvolgimento per rapporti che comprendono sia le metriche di coinvolgimento che quelle di consegna.

## Cosa fa Email Insights quando alcuni client e-mail bloccano le immagini? {#what-does-email-insights-do-when-certain-email-clients-block-images}

Un problema comune del settore è che un numero crescente di client e-mail disattivano le immagini per impostazione predefinita. Il caricamento delle immagini è la base per la registrazione delle aperture. È del tutto possibile che un utente riceva un’e-mail con immagini bloccate, ma con il testo e i collegamenti completamente leggibili. Se un utente ha avuto questa esperienza e ha fatto clic su un collegamento in quell’e-mail, si presenterà lo scenario di un evento Click, ma non il corrispondente evento Open per tale e-mail. Marketo Email Insights genererà automaticamente eventuali eventi mancanti. La logica è identica a quella utilizzata da Marketo per il rapporto Prestazioni e-mail e per l’area Analisi e-mail in Revenue Explorer.
