---
unique-page-id: 10100257
description: Domande frequenti sulle e-mail - Documenti Marketo - Documentazione prodotto
title: Domande frequenti sugli approfondimenti e-mail
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---


# Domande frequenti sulle e-mail {#email-insights-faq}

## Esistono differenze tra le metriche delle proporzioni con le informazioni e-mail e altri rapporti e-mail di marketing? {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

Sì. Le informazioni e-mail mettono in relazione le metriche di coinvolgimento con le metriche di consegna corrispondenti per la stessa e-mail inviata quando si calcolano i rapporti delle metriche di coinvolgimento (frequenza di apertura, frequenza di clic-apertura, frequenza di annullamento della sottoscrizione). Ad esempio, in Approfondimenti e-mail, quando osserviamo un grafico a serie temporali nell&#39;ultima settimana con suddivisioni giornaliere di Click-to-Open-Rate, ora viene mostrato il rapporto reale correlato degli eventi open/click/unsubscription in base alle metriche di consegna corrispondenti. Questo è in contrasto con il comportamento in Esplora entrate, che semplicemente riassume tutto. E-mail Insights offre una visualizzazione più accurata dei rapporti di coinvolgimento.

## Perché Email Insights supporta solo 10 Dimension personalizzati? {#why-does-email-insights-only-support-custom-dimensions}

Per molti casi d’uso, l’estensione delle dimensioni predefinite del sistema con 10 ulteriori dimensioni personalizzate sarà più che sufficiente e includerà dimensioni personalizzate in base alle Segmenti o ai Tag del programma. In futuro, intendiamo consentire ai clienti di aumentare il numero di Dimension personalizzati consentiti.

## Perché non è possibile riutilizzare gli slot per Dimension personalizzati dopo che sono stati assegnati? {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

Una volta allocato uno slot per Dimension personalizzato, se si rimette, i dati precedenti genererebbero un errore se mescolati con un nuovo significato. Per questo motivo, gli slot per Dimension personalizzati potrebbero non essere riutilizzati. Questo comportamento è coerente con quello di altri strumenti di analisi delle metriche, come le Google Analytics.

## Le informazioni e-mail supportano le e-mail di analisi delle vendite Marketo? {#does-email-insights-support-marketo-sales-insight-emails}

Sì. Tutte le e-mail inviate tramite Marketing Sales Insights sono incluse in Email Insights.

## Email Insights supporta le e-mail operative? {#does-email-insights-support-operational-emails}

Sì. Per impostazione predefinita, le e-mail operative vengono nascoste dalla visualizzazione e dall’esecuzione di query. Tuttavia, potete modificare questa impostazione nel pannello Impostazioni personali.

## Email Insights acquisisce i passaggi di flusso di posta elettronica pianificati o eseguiti di nuovo da Smart Campaign? {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

Sì e No. Con la versione iniziale di E-mail Insights, tutti gli eventi e-mail vengono catturati e accessibili per qualsiasi Smart Campaign pianificato o rieseguito periodicamente. Ma non sarai in grado di distinguere tra le diverse fasi di questa Smart Campaign. Nella prossima release stiamo aggiungendo supporto per acquisire le informazioni di esecuzione di Smart Campaign per gli eventi Open, Click e Unsubscription, al fine di differenziare.

## Perché molte metriche mostrano zero quando si applica il filtro in base al tipo di dispositivo o al sistema operativo del dispositivo? {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

Ad eccezione di Click-to-Open-Rate, Open, Click e Unsubscribes, tutte le altre metriche supportate sono eventi di consegna o rapporti derivati da eventi di consegna. Dal momento che il tipo di dispositivo e il sistema operativo dispositivo si applicano solo alle metriche di coinvolgimento, semplicemente non abbiamo le informazioni da visualizzare. Ad esempio, è una query non definita per richiedere il tasso di consegna quando viene filtrato per Tipo di dispositivo = mobile, poiché Marketo non avrebbe ricevuto alcuna metrica di coinvolgimento per gli eventi di consegna e invio sottostanti. Stiamo esplorando come applicare il tipo di dispositivo e il sistema operativo del dispositivo dalle metriche di coinvolgimento per i rapporti che comprendono sia le metriche di coinvolgimento che di consegna.

## Cosa fa Email Insights quando alcuni client e-mail bloccano le immagini? {#what-does-email-insights-do-when-certain-email-clients-block-images}

Un problema comune del settore è rappresentato dal numero crescente di client e-mail che disattivano le immagini per impostazione predefinita. Il caricamento delle immagini è la base per la registrazione degli Aperture. È del tutto possibile che un utente riceva un&#39;e-mail con immagini bloccate, ma con testo e collegamenti completamente leggibili. Se un utente ha riscontrato questo problema e ha fatto clic su un collegamento contenuto nell&#39;e-mail, si conclude con uno scenario di un evento Click, ma nessun evento Open corrispondente per tale e-mail. Marketo Email Insights genererà automaticamente tutti gli eventi mancanti. La logica è identica a quella utilizzata da Marketo per il report Prestazioni e-mail, nonché per l&#39;area Analisi e-mail in Esplora entrate.
