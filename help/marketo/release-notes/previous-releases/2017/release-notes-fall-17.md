---
unique-page-id: 12983280
description: Note sulla versione -Autunno '17 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Autunno '17
exl-id: 329022e6-f388-4ff9-9724-62aeed76c0b9
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---

# Note sulla versione: Autunno &#39;17 {#release-notes-fall}

Le seguenti funzioni sono incluse nella versione di autunno del 1917. Verifica la disponibilità delle funzioni nella tua edizione di Marketo.

Fai clic sui collegamenti del titolo per visualizzare articoli dettagliati per ciascuna funzione. Nota: ad alcune funzioni incluse in questa versione non sono associati articoli. Se un argomento ha più sottotitoli, i collegamenti sono posizionati lì.

## Affidabilità del sistema {#system-reliability}

Abbiamo apportato ulteriori miglioramenti all&#39;infrastruttura Marketo di base, tra cui una migliore sequenza, meno incongruenze e una maggiore stabilità di Munchkin.

## Prestazioni di sincronizzazione SFDC {#sfdc-sync-performance}

Sfrutta una sincronizzazione più ricca e veloce tra Marketo e Salesforce. Le modifiche ai dati che richiedono aggiornamenti in blocco su account o lead possono essere suddivise in code parallele per evitare backlog. Gli eventi e le attività ora si sincronizzano anche fino al 50% più rapidamente.

## Miglioramenti delle prestazioni di Analytics {#analytics-performance-improvements}

I recenti miglioramenti dell’infrastruttura offrono tempi di attività e stabilità più elevati all’interno degli strumenti di reporting e analisi di Marketo, consentendo di creare report ad hoc in modo più rapido.

## [Fuso orario destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md) {#recipient-time-zone}

Con questa nuova funzione, ora è possibile conservare e consegnare le e-mail in base ai fusi orari locali. I programmi di e-mail e coinvolgimento possono essere configurati per essere consegnati nei fusi orari dei destinatari, eliminando la necessità di creare più programmi: invia una volta e Marketo manterrà automaticamente l’e-mail fino all’ora locale corretta. Aumenta le metriche delle e-mail, osserva le pratiche locali e risparmia tempo utilizzando un singolo programma a livello globale.

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>Se non riesci ancora ad abilitare il Fuso orario del destinatario nei tuoi programmi di e-mail e coinvolgimento, non farti prendere dal panico. Questa funzione viene gradualmente attivata per tutti i clienti.

## [Rivedi e-mail di esempio per segmento](/help/marketo/product-docs/email-marketing/general/creating-an-email/send-a-sample-email.md) {#review-sample-emails-by-segment}

Marketo ha una nuova opzione per scegliere un segmento quando si inviano e-mail di esempio per la revisione. Non è più necessario determinare manualmente a quale segmento appartiene un lead, semplificando l’invio di e-mail contenenti contenuto dinamico a segmenti diversi.

## [Domande personalizzate sulla generazione lead di linkedIn](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md) {#linkedin-lead-gen-custom-questions}

Personalizza i moduli LinkedIn Lead Gen per raccogliere gli attributi del lead personalizzati. È ora possibile porre fino a tre domande personalizzate per modulo, scegliere tra un&#39;immissione di testo a riga singola o domande a scelta multipla e mappare i campi lead di Marketo.

## Integrazione Slack {#slack-integration}

Sono state rilasciate due funzioni come parte della nuova integrazione di Slack:

* Notifiche di sistema: ottieni notifiche di Slack relative a eventi importanti nell’istanza di Marketo, ad esempio avvisi sugli stati attuali delle campagne e su eventuali problemi che richiedono attenzione immediata.
* Momenti interessanti: quando un oggetto Marketo Insight è stato attivato da un utente noto da un account di vendita, i proprietari dei lead possono ricevere una notifica tramite Slack. Le notifiche includono informazioni sul lead e dettagli sul conto vendite.

## Miglioramenti ABM {#abm-enhancements}

**[Mostra account senza contatti](https://docs.marketo.com/x/fKCt)**

Marketo ABM ora sincronizza e visualizza gli account CRM senza contatti. Includi nuovi account senza cronologia di vendita o marketing precedente e tieni traccia dell’avanzamento confrontando i lead successivi con gli account.

## Analytics di ContentAI {#contentai-analytics}

**[Nuovo filtro elenco account ABM](https://docs.marketo.com/x/1BPG)**

Visualizza e confronta le prestazioni dei contenuti negli elenchi di account ABM per ottimizzare i contenuti esistenti. ContentAI mostra:

* contenuto principale visualizzato
* contenuto convertito principale
* Contenuti suggeriti basati sull’intelligenza artificiale per le attività di marketing

## Miglioramenti alla personalizzazione web {#web-personalization-enhancements}

**[Token per campagne web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

I token sono ora disponibili per l’utilizzo nelle campagne web. Sfrutta i token per inviare messaggi e contenuti personalizzati per aumentare il coinvolgimento nelle campagne web.

![](assets/image2017-11-16-11-3a25-3a7.png)

**[Immagini di Design Studio nell’Editor di campagne web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Risparmia tempo riutilizzando le risorse creative e le immagini su più canali in Marketo.

![](assets/image2017-11-16-11-3a26-3a10.png)

## Integrazione  {#integration}

**[API di anteprima e-mail](https://developers.marketo.com/rest-api/assets/emails/)**

Ora è possibile visualizzare in anteprima e-mail in remoto al di fuori di Marketo, semplificando il processo di localizzazione dei contenuti e-mail e riducendo gli errori.

**[Sostituisci API HTML](https://developers.marketo.com/rest-api/assets/emails/)**

Gli sviluppatori possono aggiornare il contenuto HTML delle risorse e-mail in remoto, consentendo loro di lavorare all’interno di un singolo sistema per mantenere le risorse.
