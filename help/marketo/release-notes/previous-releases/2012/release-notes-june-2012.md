---
unique-page-id: 2951114
description: Note sulla versione - Giugno 2012 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Giugno 2012
exl-id: c22eda86-da7a-4c76-9cea-1ce23ff0f3e8
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---

# Note sulla versione - Giugno 2012 {#release-notes-june}

## Miglioramenti alla gestione dei lead in Marketo {#marketo-lead-management-enhancements}

### Rinomina {#rename}

Puoi rinominare i tuoi elenchi avanzati, gli elenchi statici e le campagne. Se utilizzi queste risorse in filtri, trigger o flussi, anche qui il nome verrà aggiornato automaticamente. È sempre stato possibile rinominare e-mail, moduli e cartelle.

Inoltre, abbiamo migliorato l’inserimento e la visualizzazione del testo descrittivo delle risorse.

![](assets/image2014-9-23-10-3a23-3a10.png)

## Importa mappatura campi {#import-field-mapping}

L&#39;importazione di un elenco in Marketo è stata semplificata. Durante il processo di importazione, è possibile mappare il nome del campo Marketo al nome dell&#39;intestazione di colonna nel file di importazione. Inoltre, in [!UICONTROL Admin] è possibile impostare alias mappati al nome del campo in Marketo, assicurandosi che gli utenti selezionino ogni volta il campo corretto.

Continuando a importare e mappare i campi, Marketo ricorderà e visualizzerà le mappature durante l’importazione, per semplificarne l’utilizzo. Per semplificare ulteriormente la gestione, fai clic sull’intestazione Valore di esempio per visualizzare i diversi valori che verrebbero inseriti nel campo. Questo ti aiuta a mappare il campo corretto ogni volta.

![](assets/image2014-9-23-10-3a23-3a27.png)

## Pagina [!UICONTROL Summary] per elenchi avanzati ed elenchi statici {#summary-page-for-smart-lists-and-static-lists}

Vi siete mai chiesti dove vengono usati i vostri elenchi? Chi ha creato o modificato per ultimo l’elenco? La nuova pagina di riepilogo disponibile negli elenchi smart e statici fornirà questi importanti dettagli.

![](assets/image2014-9-23-10-3a23-3a40.png)

Nelle pagine di riepilogo esistenti di Programma e Campagna, sono state aggiunte anche le informazioni Data di creazione/Utente e Data/Utente ultima modifica.

![](assets/image2014-9-23-10-3a23-3a54.png)

## [!UICONTROL Used By] per Assets {#used-by-for-assets}

È stata aggiunta una nuova scheda alle pagine [!UICONTROL Summary] della risorsa, denominata [!UICONTROL Used By].

![](assets/image2014-9-23-10-3a24-3a5.png)

Esempio: [!UICONTROL Used By] per elenchi statici

## Griglia della pagina di destinazione {#landing-page-gridlines}

L’aggiunta della griglia della pagina di destinazione semplifica notevolmente l’allineamento di testo, elementi grafici e moduli nella pagina di destinazione. Attiva e disattiva questa funzione per tutte le pagine di destinazione e regola anche la larghezza tra le righe.

![](assets/image2014-9-23-10-3a24-3a19.png)

![](assets/image2014-9-23-10-3a24-3a33.png)

## Lead bloccati da mailing {#leads-blocked-from-mailings}

Quando pianifichi una campagna, puoi fare clic sul collegamento per visualizzare l’elenco dei lead che sono bloccati dalla tua mailing.

![](assets/image2014-9-23-10-3a24-3a51.png)

## Passaggio [!UICONTROL Wait] - Token lead e token personale {#wait-step-lead-token-and-my-token}

Nella versione di maggio sono state aggiunte opzioni avanzate al passaggio del flusso [!UICONTROL Wait]. Con queste modifiche è possibile specificare un giorno lavorativo, una data e un&#39;ora. In questa versione è stata aggiunta la possibilità di utilizzare un token nel passaggio di attesa. Ad esempio, è possibile utilizzare `{{lead.Birthday}}` per inviare un messaggio e-mail di compleanno o `{{my.Event Date}}` per inviare un promemoria finale del webinar.

![](assets/image2014-9-23-10-3a25-3a57.png)

## [!UICONTROL View] come [!UICONTROL Thumbnails] in Design Studio {#view-as-thumbnails-in-design-studio}

Passare da una visualizzazione elenco di immagini a una visualizzazione miniature.

![](assets/image2014-9-23-10-3a26-3a13.png)

Nota: a partire da questa versione, l’ordinamento precedente sulle griglie degli elenchi smart non verrà applicato al successivo elenco smart visualizzato. Ad esempio, se ordini un elenco avanzato per Nome società, il successivo elenco avanzato visualizzato dallo stesso campo non verrà ordinato automaticamente.

Promemoria: è in corso l&#39;aggiornamento del report sulle prestazioni delle e-mail.

## Miglioramenti di Marketo Revenue Cycle Analytics {#marketo-revenue-cycle-analytics-enhancements}

### Nuove metriche nell’analisi dell’opportunità del programma  {#new-metrics-in-program-opportunity-analysis}

Ora puoi ottenere informazioni sul numero medio di contatti di marketing prima che le opportunità vengano create o chiuse, nonché sul valore medio di un contatto di marketing.

![](assets/image2014-9-23-10-3a26-3a30.png)

![](assets/image2014-9-23-10-3a26-3a41.png)

## Visualizzazione di grafici multipli {#displaying-multi-charts}

La funzione a più grafici consente di visualizzare più grafici in un unico rapporto di Revenue Cycle Explorer. Ad esempio, puoi utilizzare questa funzione quando desideri visualizzare gli stessi dati in mesi diversi. Questa funzione consente inoltre di evitare la creazione di filtri e rapporti separati.

![](assets/image2014-9-23-10-3a27-3a41.png)

## Tipo di grafico a griglia di calore  {#heat-grid-chart-type}

Le griglie di calore consentono di visualizzare i dati in modo da identificare i pattern delle prestazioni di marketing. Questo tipo di visualizzazione assegnerà un colore al codice dei risultati, consentendoti di visualizzare analisi aziendali complesse in una visualizzazione di facile comprensione.

![](assets/image2014-9-23-10-3a28-3a21.png)

## Tipo di grafico a dispersione  {#scatter-chart-type}

I grafici a dispersione consentono di visualizzare i dati su più dimensioni in un unico grafico. Questo tipo di visualizzazione traccia una bolla su un grafico in base agli attributi utilizzati. Potete quindi utilizzare una misura per codificare il colore della bolla e/o una misura per specificare la dimensione della bolla.

![](assets/image2014-9-23-10-3a29-3a7.png)
