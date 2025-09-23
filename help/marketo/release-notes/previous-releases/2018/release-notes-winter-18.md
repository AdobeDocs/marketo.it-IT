---
unique-page-id: 13795395
description: Note sulla versione -Inverno '18 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Inverno '18
exl-id: f08bdc91-86d3-4ea2-a74a-1398ed525bbb
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 2%

---

# Note sulla versione - Inverno 2018 {#release-notes-winter}

Le seguenti funzioni sono incluse nella versione invernale del 18. Verifica la disponibilità delle funzioni nella tua edizione di Marketo.

Fai clic sui collegamenti del titolo per visualizzare articoli dettagliati per ciascuna funzione. **Nota**: ad alcune funzionalità incluse in questa versione non sono associati articoli. Se un argomento ha più sottotitoli, i collegamenti sono posizionati lì.

## Miglioramenti a livello di prestazioni e velocità effettiva delle campagne {#campaign-performance-and-throughput-enhancements}

Marketo sfrutta la nostra architettura dei big data per aumentare la velocità effettiva delle campagne trigger e migliorare l’elaborazione delle attività web, in modo da poter reagire più rapidamente alle azioni del pubblico.

## Miglioramenti all&#39;integrazione CRM [!DNL Salesforce] di Marketo {#enhancements-to-marketo-s-salesforce-crm-integration}

Sono stati apportati due miglioramenti all&#39;integrazione CRM di [!DNL Salesforce]:

* [Notifiche dell&#39;amministratore di Marketo](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md) per alcuni errori di sincronizzazione CRM (credenziali scadute, limiti API raggiunti, ecc.)

* [Possibilità di disattivare le notifiche e-mail](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/turn-off-email-notifications-to-lead-owner.md) ai Proprietari lead all&#39;assegnazione del lead

Questi miglioramenti verranno implementati nel corso del 2018.

## [Informazioni sulle prestazioni di Marketo](/help/marketo/product-docs/reporting/performance-insights/performance-insights-overview.md) {#marketo-performance-insights}

>[!AVAILABILITY]
>
>[!UICONTROL Performance Insights] è un componente aggiuntivo. Contatta il tuo Customer Success Manager Marketo o Account Executive per richiedere un preventivo.

Scopri in che modo le campagne e i canali influiscono sui risultati aziendali con analisi dell’attribuzione, visualizzazioni interattive e una tabella di dati dettagliata.

![](assets/image2018-2-5-7-3a55-3a46.png)

## Miglioramenti del marketing basato sull’account {#account-based-marketing-enhancements}

**[Gerarchie ABM](/help/marketo/product-docs/target-account-management/target/named-accounts/tam-hierarchies.md)**

Per i clienti ABM con [!DNL Salesforce] o [!DNL Microsoft Dynamics], ABM erediterà automaticamente (e visualizzerà) le relazioni padre-figlio stabilite nel CRM. Potrai utilizzare queste relazioni sia nel reporting aggregato che nell’esecuzione della campagna.

## Marketing via e-mail {#email-marketing}

**[Script e-mail dinamico](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)**

Lo script Velocity è ora supportato nelle e-mail che utilizzano il contenuto dinamico. Combina velocità e contenuti dinamici basati sulla segmentazione per creare e-mail altamente personalizzate.

**Fuso orario destinatario**

* **[Cadenza dell&#39;accrescimento mensile](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)**: è stata aggiunta la possibilità di pianificare programmi di accrescimento con cadenza mensile.

* **[Interrompi consegna](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)**: ora puoi interrompere tutti gli invii rimanenti a metà dell&#39;esecuzione.

## Integrazioni di ad network {#ad-network-integrations}

**[Integrazione Customer Match Google](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-google-customer-match-as-a-launchpoint-service.md)**

Con questa integrazione, puoi inviare un pubblico Marketo a Google per il targeting utilizzando [!DNL Google AdWords], nonché rieseguire il targeting dei tipi di pubblico in [!DNL YouTube], Search e [!DNL Gmail].

**[[!DNL LinkedIn] Miglioramento API tipi di pubblico corrispondenti](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md)**

La nuova API [!DNL LinkedIn] consente ora di eseguire il targeting delle persone nel database di Marketo tra più account di [!DNL LinkedIn] Campaign Manager.

## Personalizzazione web {#web-personalization}

**Source dati giapponese per Web Personalization**

Marketo sta aggiungendo un’ulteriore origine dati giapponese per Web Personalization per migliorare l’identificazione dei visitatori web (ricerca IP inversa) e la personalizzazione per i visitatori provenienti dal Giappone. I nomi delle organizzazioni verranno visualizzati in giapponese.

**[Creare un segmento Web utilizzando elenchi statici](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-a-static-list.md)**

Il Web Personalization ora può personalizzare il contenuto per un visitatore web noto che fa parte di un elenco statico definito in Attività di marketing (MLM). Con questo miglioramento, ora puoi vendere a elenchi statici tra canali diversi e indirizzare le persone in tali elenchi con contenuti personalizzati sul tuo sito web.

## ContentAI {#contentai}

**Miglioramento dell&#39;algoritmo predittivo**

Il contenuto consigliato tramite gli algoritmi ContentAI ottimizzati di Marketo genera fino al doppio di clic rispetto al contenuto casuale.

## Integrazione {#integration}

**[Attiva/Disattiva API Campaign](https://developers.marketo.com/rest-api/assets/smart-campaigns/)**

Questa nuova API consente di attivare e disattivare in remoto le campagne di attivazione, per creare modelli di programma completamente automatizzati. Crea un modello di programma una volta, quindi automatizza la clonazione, gli aggiornamenti dei materiali di marketing e ora l’attivazione/pianificazione delle campagne intelligenti.

## [!DNL ToutApp] {#toutapp}

**Aggiornamento annullamento abbonamento**

A partire dal 1° marzo 2018, a tutte le e-mail inviate da [ToutApp.com](https://ToutApp.com) (e utilizzando il pulsante &quot;E-mail con [!DNL Tout]&quot; in [!DNL Salesforce]) verrà aggiunto in basso un collegamento per l&#39;annullamento dell&#39;iscrizione.

**Aggiornamento feed live**

Abbiamo aggiornato l&#39;aspetto delle schede Coinvolgimento e Attività per consentire ai membri delle vendite di rispondere più facilmente e più rapidamente alle attività dei clienti direttamente dal feed live.

**Aggiornamento visualizzazione dettagli persone**

La visualizzazione PDV (People Detail View) migliorata offre una visualizzazione completa dei contatti riunendo i dettagli di contatto del CRM [!DNL Tout] e [!DNL Salesforce].
