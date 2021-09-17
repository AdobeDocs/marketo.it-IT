---
unique-page-id: 12983280
description: Note sulla versione - Autunno 2017 - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione - Autunno 2017
exl-id: 329022e6-f388-4ff9-9724-62aeed76c0b9
source-git-commit: cbfa6110e85c185a5b65342052f168d9715f2f6a
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---

# Note sulla versione: Autunno 17 {#release-notes-fall}

Le seguenti funzionalità sono incluse nella versione autunnale del 17. Per informazioni sulla disponibilità delle funzioni, consulta la tua edizione Marketo .

Fai clic sui collegamenti del titolo per visualizzare gli articoli dettagliati per ciascuna funzione. Nota: Alcune delle funzioni incluse in questa versione non hanno articoli associati. Se un argomento ha più sottotitoli, i collegamenti vengono posizionati in tale punto.

## Affidabilità del sistema {#system-reliability}

Abbiamo apportato ulteriori miglioramenti all&#39;infrastruttura Marketo di base, tra cui una migliore sequenza, meno incongruenze e una maggiore stabilità Munchkin.

## Prestazioni di sincronizzazione SFDC {#sfdc-sync-performance}

Sfrutta la sincronizzazione più completa e rapida tra Marketo e Salesforce. Le modifiche ai dati che richiedono aggiornamenti in blocco su account o lead possono essere suddivise in code parallele per evitare backlog. Anche gli eventi e le attività ora si sincronizzano più rapidamente del 50%.

## Miglioramenti delle prestazioni di Analytics {#analytics-performance-improvements}

I recenti miglioramenti dell&#39;infrastruttura offrono tempi di attività e stabilità maggiori all&#39;interno degli strumenti di reporting e analisi di Marketo, consentendo di creare report ad hoc più rapidamente.

## [Fuso orario destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md) {#recipient-time-zone}

Con questa nuova funzione, ora puoi tenere e consegnare e-mail in base ai fusi orari locali. I programmi e-mail e di coinvolgimento possono essere configurati in modo da essere consegnati nei fusi orari dei destinatari, eliminando la necessità di creare più programmi: invia una volta e Marketo manterrà automaticamente l’e-mail fino all’ora locale corretta. Incrementa le metriche delle e-mail, osserva le pratiche locali e risparmia tempo utilizzando un singolo programma a livello globale.

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>Se non puoi ancora abilitare il fuso orario dei destinatari nelle tue e-mail e nei tuoi programmi di coinvolgimento, non farti prendere dal panico! Questa funzione viene gradualmente abilitata per tutti i clienti.

## [Rivedi e-mail di esempio per segmento](/help/marketo/product-docs/email-marketing/general/creating-an-email/send-a-sample-email.md) {#review-sample-emails-by-segment}

Marketo ha una nuova opzione per scegliere un segmento quando invia e-mail di esempio per la revisione. Non è più necessario determinare manualmente a quale segmento appartiene un lead, facilitando l’invio di e-mail contenenti contenuto dinamico a segmenti diversi.

## [Domande personalizzate di linkedIn Lead Gen](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md) {#linkedin-lead-gen-custom-questions}

Personalizza i moduli LinkedIn Lead Gen per raccogliere gli attributi personalizzati del lead. È ora possibile porre fino a tre domande personalizzate per modulo, scegliere tra un testo a riga singola o domande a scelta multipla e mappare nuovamente i campi lead Marketo.

## Integrazione Slack {#slack-integration}

Sono state rilasciate due funzionalità nell&#39;ambito della nuova integrazione di Slack:

* Notifiche di sistema: Ottieni notifiche di Slack relative a eventi importanti nella tua istanza Marketo, come avvisi sugli stati della campagna corrente e su qualsiasi problema che richieda un’attenzione immediata.
* Momenti interessanti: Quando Marketo Insight viene attivato da un individuo noto da un account di vendita, i proprietari lead possono essere informati tramite Slack. Le notifiche includono informazioni sui lead e dettagli sull’account di vendita.

## Miglioramenti di ABM {#abm-enhancements}

**[Mostra account senza contatti](https://docs.marketo.com/x/fKCt)**

Marketo ABM ora sincronizza e visualizza gli account CRM senza contatti. Includi nuovi account senza precedenti vendite o cronologia di marketing e monitora l&#39;avanzamento confrontando i lead successivi agli account.

## Analisi di ContentAI {#contentai-analytics}

**[Nuovo filtro elenco account ABM](https://docs.marketo.com/x/1BPG)**

Visualizza e confronta le prestazioni del contenuto negli elenchi account ABM per ottimizzare il contenuto esistente. ContentAI mostra quanto segue:

* contenuto principale visualizzato
* contenuto convertito principale
* Contenuto consigliato basato sull’intelligenza artificiale per attività di marketing

## Miglioramenti alla personalizzazione web {#web-personalization-enhancements}

**[Token per campagne web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

I token sono ora disponibili per l’utilizzo all’interno di campagne web. Utilizza i token per inviare messaggi e contenuti personalizzati per aumentare il coinvolgimento nelle campagne web.

![](assets/image2017-11-16-11-3a25-3a7.png)

**[Immagini di Design Studio nell’editor di Web Campaign](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Risparmia tempo riutilizzando risorse creative e immagini su più canali in Marketo.

![](assets/image2017-11-16-11-3a26-3a10.png)

## Integrazione  {#integration}

**[API di anteprima e-mail](https://developers.marketo.com/rest-api/assets/emails/)**

Ora puoi visualizzare in anteprima e-mail in remoto al di fuori di Marketo, semplificando il processo di localizzazione dei contenuti e-mail e riducendo gli errori.

**[Sostituire l’API HTML](https://developers.marketo.com/rest-api/assets/emails/)**

Gli sviluppatori possono aggiornare il contenuto HTML delle risorse e-mail in modo remoto, consentendo loro di lavorare all’interno di un singolo sistema per mantenere le risorse.
