---
unique-page-id: 10100257
description: Domande frequenti su Email Insights - Documentazione di Marketo - Documentazione del prodotto
title: Domande frequenti su approfondimenti e-mail
exl-id: de3aca5a-08b4-4af8-ab92-675cb46dcbb2
feature: Reporting
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 1%

---

# Domande frequenti su approfondimenti e-mail {#email-insights-faq}

## Esistono differenze tra le metriche del rapporto con [!UICONTROL Email Insights] e altri rapporti e-mail di Marketo? {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

Sì.  [!UICONTROL Email Insights] mette in correlazione le metriche di coinvolgimento con le metriche di consegna corrispondenti per la stessa e-mail inviata quando si calcolano i rapporti delle metriche di coinvolgimento (Percentuale di apertura, Percentuale di clic per apertura, Percentuale di annullamento abbonamento). Ad esempio, in [!UICONTROL Email Insights], quando si esamina un grafico di serie temporali nell&#39;ultima settimana con raggruppamenti giornalieri di Click-to-Open-Rate, ora viene mostrato il rapporto effettivo correlato tra eventi di apertura, clic e annullamento dell&#39;abbonamento in base alle metriche di consegna corrispondenti. Ciò è in contrasto con il comportamento di Esplora entrate, che semplicemente riassume tutto. [!UICONTROL Email Insights] offre una visualizzazione più precisa dei rapporti di coinvolgimento.

## Perché [!UICONTROL Email Insights] supporta solo 10 dimensioni personalizzate? {#why-does-email-insights-only-support-custom-dimensions}

Per molti casi d’uso, l’estensione delle dimensioni di sistema predefinite con 10 dimensioni personalizzate aggiuntive sarà più che adeguata e includerà dimensioni personalizzate basate su Segmentazioni o Tag programma. In futuro, prevediamo di consentire ai clienti di aumentare il numero di dimensioni personalizzate consentite.

## Perché non è possibile riutilizzare gli slot delle dimensioni personalizzate dopo averli assegnati? {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

Una volta allocato un determinato slot Dimension personalizzato, la modifica della mappatura causerebbe la generazione di un errore nei dati precedenti in caso di fusione con un nuovo significato. Per questo motivo, gli slot Dimension personalizzati non possono essere riutilizzati. Questo comportamento è coerente con quello di altri strumenti di analisi metrica, come Google Analytics.

## [!UICONTROL Email Insights] supporta le e-mail di Marketo Sales Insight? {#does-email-insights-support-marketo-sales-insight-emails}

Sì.  Tutti i messaggi di posta elettronica inviati tramite Marketo Sales Insights sono inclusi in [!UICONTROL Email Insights].

## [!UICONTROL Email Insights] supporta le e-mail operative? {#does-email-insights-support-operational-emails}

Sì.  Per impostazione predefinita, le e-mail operative sono nascoste dalla visualizzazione e dall’esecuzione di query. Tuttavia, potete modificare questa impostazione nel pannello Impostazioni personali.

## [!UICONTROL Email Insights] acquisisce i passaggi ricorrenti del flusso e-mail pianificati o rieseguiti di Smart Campaign? {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

Sì e No. Con la versione iniziale di [!UICONTROL Email Insights], tutti gli eventi e-mail vengono acquisiti e accessibili per qualsiasi campagna Smart ricorrente pianificata o rieseguita. Ma non potrai distinguere tra diverse esecuzioni di quella campagna avanzata. Nella prossima versione verrà aggiunto il supporto necessario per acquisire le informazioni di esecuzione di Smart Campaign per gli eventi Apri, Clic e Annulla iscrizione al fine di differenziarli.

## Perché molte metriche mostrano lo zero quando si filtra per tipo di dispositivo o SO del dispositivo? {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

Ad eccezione di Tasso di clic per apertura, Aperture, Clic e Annullamenti abbonamenti, tutte le altre metriche supportate sono eventi di consegna o rapporti derivati da eventi di consegna. Poiché il tipo di dispositivo e il sistema operativo del dispositivo si applicano solo alle metriche di coinvolgimento, le informazioni da visualizzare non sono disponibili. Ad esempio, si tratta di una query non definita per richiedere la Percentuale di Consegna quando viene filtrata per Tipo di Dispositivo = mobile, in quanto Marketo non avrebbe ricevuto alcuna metrica di Coinvolgimento per gli eventi di Consegna e Inviato sottostanti. Stiamo esplorando modi per applicare il tipo di dispositivo e il sistema operativo del dispositivo dalle metriche di coinvolgimento per rapporti che comprendono sia le metriche di coinvolgimento che quelle di consegna.

## Cosa fa [!UICONTROL Email Insights] quando alcuni client di posta elettronica bloccano le immagini? {#what-does-email-insights-do-when-certain-email-clients-block-images}

Un problema comune del settore è che un numero crescente di client e-mail disattivano le immagini per impostazione predefinita. Il caricamento delle immagini è la base per la registrazione delle aperture. È del tutto possibile che un utente riceva un’e-mail con immagini bloccate, ma con il testo e i collegamenti completamente leggibili. Se un utente ha avuto questa esperienza e ha fatto clic su un collegamento in quell’e-mail, si presenterà lo scenario di un evento Click, ma non il corrispondente evento Open per tale e-mail. Marketo Email Insights genererà automaticamente eventuali eventi mancanti. La logica è identica a quella utilizzata da Marketo per il rapporto Prestazioni e-mail e per l’area Analisi e-mail in Revenue Explorer.
