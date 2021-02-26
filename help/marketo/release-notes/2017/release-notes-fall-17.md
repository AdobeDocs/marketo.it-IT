---
unique-page-id: 12983280
description: Note sulla versione - Autunno '17 - Documenti Marketo - Documentazione prodotto
title: Note sulla versione - Autunno '17
translation-type: tm+mt
source-git-commit: b33f5ed707a1377daad51191cc6dd9f093138258
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---


# Note sulla versione: Autunno &#39;17 {#release-notes-fall}

Le seguenti funzionalità sono incluse nella release autunnale 17. Per informazioni sulla disponibilità delle funzionalità, consulta la versione di Marketo.

Fate clic sui collegamenti del titolo per visualizzare articoli dettagliati per ciascuna funzione. Nota: Alcune delle funzioni incluse in questa versione non hanno articoli associati. Se un argomento include più sottotitoli, i collegamenti vengono inseriti in tale area.

## Affidabilità del sistema {#system-reliability}

Abbiamo apportato ulteriori miglioramenti all&#39;infrastruttura principale di Marketo, tra cui una migliore sequenza, meno incongruenze e una migliore stabilità di Munchkin.

## Prestazioni sincronizzazione SFDC {#sfdc-sync-performance}

Sfruttate i vantaggi di una sincronizzazione più completa e rapida tra Marketo e Salesforce. Le modifiche dei dati che richiedono aggiornamenti in massa su account o lead possono essere suddivise in code parallele per evitare backlog. Eventi e attività ora si sincronizzano più rapidamente del 50%.

## Miglioramenti delle prestazioni di Analytics {#analytics-performance-improvements}

I recenti miglioramenti dell&#39;infrastruttura offrono tempi di attività e stabilità maggiori all&#39;interno degli strumenti di reporting e analisi di Marketo, consentendo di creare report ad hoc più rapidamente.

## [Fuso orario destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md) {#recipient-time-zone}

Con questa nuova funzione, ora puoi tenere premuto e inviare e-mail in base ai fusi orari locali. I programmi di e-mail e di coinvolgimento possono essere configurati per essere inviati nei fusi orari dei destinatari, eliminando la necessità di creare più programmi. Invia una volta e Marketo manterranno automaticamente l&#39;e-mail fino all&#39;ora locale corretta. Incrementate le metriche delle e-mail, osservate le pratiche locali e risparmiate tempo utilizzando un singolo programma a livello globale.

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>Se non puoi ancora attivare il fuso orario dei destinatari nelle tue e-mail e nei tuoi programmi di coinvolgimento, non preoccuparti! Questa funzione viene attivata gradualmente per tutti i clienti.

## [Rivedi e-mail di esempio per segmento](/help/marketo/product-docs/email-marketing/general/creating-an-email/send-a-sample-email.md) {#review-sample-emails-by-segment}

Marketo dispone di una nuova opzione per selezionare un segmento quando invia e-mail di esempio per la revisione. Non è più necessario determinare manualmente a quale segmento appartiene un lead, per inviare più facilmente e-mail contenenti contenuto dinamico a segmenti diversi.

## [Domande personalizzate LinkedIn lead Gen](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md) {#linkedin-lead-gen-custom-questions}

Personalizzate i moduli di LinkedIn Lead Gen per la raccolta di attributi lead personalizzati. È ora possibile porre fino a tre domande personalizzate per modulo, scegliere tra testo di input a riga singola o domande a scelta multipla e mappare nuovamente i campi lead Marketo.

## [Integrazione Slack ](/help/marketo/product-docs/administration/additional-integrations/add-slack-as-a-launchpoint-service.md) {#slack-integration}

Abbiamo introdotto due funzionalità nell&#39;ambito della nuova integrazione di Slack :

* Notifiche di sistema: Ricevi notifiche  Slack relative a eventi importanti nell’istanza di Marketo, come avvisi sugli stati delle campagne correnti e su eventuali problemi che richiedono un’attenzione immediata.
* Momenti interessanti: Quando un Marketo Insight è stato attivato da un individuo noto da un conto di vendita, i proprietari principali possono essere informati tramite  Slack. Le notifiche includono informazioni sui lead e dettagli sul conto di vendita.

## Miglioramenti ABM {#abm-enhancements}

**[Mostra account senza contatti](https://docs.marketo.com/x/fKCt)**

Marketo ABM ora sincronizza e visualizza gli account CRM senza contatti. Includi nuovi account senza precedenti vendite o cronologia marketing e monitora l&#39;avanzamento confrontando i lead successivi agli account.

## ContentAI Analytics {#contentai-analytics}

**[Nuovo filtro elenco account ABM](https://docs.marketo.com/x/1BPG)**

Visualizzate e confrontate le prestazioni del contenuto negli elenchi di account ABM per ottimizzare il contenuto esistente. ContentAI mostra quanto segue:

* contenuto principale visualizzato
* contenuto convertito principale
* Contenuto suggerito basato su AI per attività di marketing

## Miglioramenti della personalizzazione Web {#web-personalization-enhancements}

**[Token per campagne Web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

I token sono ora disponibili per l&#39;utilizzo all&#39;interno delle campagne Web. Sfruttate i token per inviare messaggi e contenuti personalizzati per aumentare il coinvolgimento nelle campagne Web.

![](assets/image2017-11-16-11-3a25-3a7.png)

**[Immagini di Design Studio nell&#39;editor di campagne Web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Risparmia tempo riutilizzando risorse creative e immagini su più canali in Marketo.

![](assets/image2017-11-16-11-3a26-3a10.png)

## Integrazione {#integration}

**[API di anteprima e-mail](https://developers.marketo.com/rest-api/assets/emails/)**

Ora potete visualizzare in anteprima le e-mail all&#39;esterno di Marketo, semplificando il processo di localizzazione del contenuto delle e-mail e riducendo gli errori.

**[Replace HTML API](https://developers.marketo.com/rest-api/assets/emails/)**

Gli sviluppatori possono aggiornare il contenuto HTML delle risorse e-mail in remoto, consentendo loro di lavorare all’interno di un singolo sistema per mantenere le risorse.
