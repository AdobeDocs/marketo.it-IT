---
unique-page-id: 11384018
description: Note sulla versione - Autunno 2016 - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione - Autunno 2016
exl-id: da935951-162e-426c-acf2-12c55ff706b4
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# Note sulla versione: Autunno 16 {#release-notes-fall}

Le seguenti funzionalità sono incluse nella versione autunnale del 16. Per informazioni sulla disponibilità delle funzioni, consulta la tua edizione Marketo . Fai clic sui collegamenti del titolo per visualizzare gli articoli dettagliati per ciascuna funzione.

## Contenuto predittivo nell’e-mail {#predictive-content-in-email}

C&#39;è una nuova esperienza utente per la nostra applicazione Predictive Content per monitorare, gestire e consigliare i contenuti tramite il nostro apprendimento automatico e gli algoritmi predittivi attraverso i canali web ed e-mail.

>[!NOTE]
>
>Tutti i clienti con il modulo Predictive saranno abilitati entro il 10 gennaio.

![](assets/shafe.png)

Ora puoi aggiungere contenuto predittivo alla tua e-mail. Quando l’e-mail viene aperta, il destinatario riceve automaticamente contenuti pertinenti e consigliati che contribuiscono ad aumentare l’engagement e le conversioni dei contenuti.

![](assets/predictive.png)

## [Conversioni offline facebook](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md) {#facebook-offline-conversions}

Con l’integrazione delle conversioni offline di Facebook, i dati di conversione in Marketo (per i lead annuncio) vengono automaticamente rimandati a Facebook in modo che il team pubblicitario possa ottimizzare meglio la spesa pubblicitaria. In questo rapporto di Facebook Ad Manager, le conversioni offline sono evidenziate.

![](assets/facebook.png)

## [ID universale](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md) {#universal-id}

Un ID universale consente di accedere a più abbonamenti Marketo con un singolo accesso e passare rapidamente da un’iscrizione all’altra. Puoi utilizzare un unico profilo community per tutti gli abbonamenti.

![](assets/image2016-11-3-15-3a10-3a16.png)

>[!NOTE]
>
>Per abilitare questa funzione, contatta il supporto Marketo.

## Miglioramenti al marketing basati su account Marketo {#marketo-account-based-marketing-enhancements}

Ora è possibile assegnare team di account a account denominati in ABM (Account Based Marketing), ad esempio il proprietario dell&#39;account, il rappresentante per lo sviluppo delle vendite, il rappresentante per lo sviluppo aziendale e il responsabile del successo del cliente. Puoi anche creare elenchi di account specifici per il proprietario dell’account e inviare rapporti ABM settimanali personalizzati al team dell’account.

![](assets/account-team-11-15-16.png)

**API REST**

Questa versione consente inoltre di gestire gli attributi e i punteggi degli account denominati in ABM utilizzando l’API REST di Marketo. Per maggiori dettagli sulle operazioni API, visita il [Sito web Marketo Developers](https://developers.marketo.com/rest-api/lead-database/named-accounts).

## [Miglioramenti a Audit Trail](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) {#audit-trail-enhancements}

Audit trail fornisce una cronologia completa delle modifiche apportate all’interno dell’abbonamento Marketo. Sono state aggiunte funzionalità aggiuntive di tracciamento per i programmi, oltre a informazioni importanti sulle modifiche per campagne intelligenti, elenchi smart e modifiche apportate a utenti e ruoli.

## [Nuove autorizzazioni](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/descriptions-of-role-permissions.md) {#new-permissions}

**Rendi le e-mail operative**

Sono finiti i giorni in cui ci si doveva preoccupare che gli utenti inviassero e-mail transazionali alle persone nel database che hanno annullato l’abbonamento. Ora puoi specificare quali utenti possono rendere operativa un’e-mail o modificarla.

**Modificare le restrizioni delle campagne**

Perché impostare [restrizioni alle campagne](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) se non riesci a farle rispettare? Quando imposti Impostazioni limite campagna per limitare il numero di persone nel database che possono essere oggetto di targeting con una singola campagna, ora puoi limitare quali utenti possono ignorare queste impostazioni durante la pianificazione di una campagna.

## [Suono per le notifiche push per dispositivi mobili](/help/marketo/product-docs/mobile-marketing/push-notifications/configure-mobile-push-notification.md) {#sound-for-mobile-push-notifications}

Offri ai tuoi iOS Push Notification una maggiore ricchezza abilitando il suono. Questa nuova funzione consente di attivare un suono quando si visualizzano le notifiche push sul dispositivo mobile.

>[!NOTE]
>
>* I proprietari del dispositivo possono scegliere di impedire la riproduzione di suoni nelle impostazioni del dispositivo, e gli sviluppatori di app possono dare ai proprietari del dispositivo opzioni all&#39;interno dell&#39;app per evitare che i suoni vengano riprodotti.
>* I suoni vengono riprodotti automaticamente quando una notifica push viene visualizzata su un dispositivo Android.


![](assets/sound-for-push-notifications.png)

## [Insight delle vendite compatibile con la crittografia Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) {#sales-insight-compatible-with-salesforce-encryption}

Market Sales Insight è ora compatibile con la crittografia Salesforce Shield. Tutti i clienti di Sales Insight devono effettuare l’aggiornamento a questo pacchetto gestito più recente (versione 1.4359.2), ovvero [disponibile su Appexchange](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO).

## [API di account denominati](https://developers.marketo.com/rest-api/lead-database/named-accounts/) {#named-accounts-apis}

Con questa versione, gli utenti di Marketo ABM possono gestire account denominati tramite l’API Account denominati. Gli utenti possono creare, aggiornare ed eliminare account denominati, nonché leggere e aggiornare i punteggi di account con nome ABM.

## [Supporto API per l’editor di e-mail v2.0](https://developers.marketo.com/rest-api/assets/emails/) {#email-editor-v-api-support}

Gestisci variabili e moduli per le e-mail in formato v2.0 utilizzando l’API REST di Marketo.

## [Modifiche alla sincronizzazione di Marketo Salesforce](https://nation.marketo.com/docs/DOC-3840) {#changes-to-marketo-salesforce-sync}

L’integrazione Salesforce di Marketo si sta evolvendo per migliorare il modo in cui i campi Marketo vengono sincronizzati con Salesforce. Ora, invece di dover sincronizzare un ampio gruppo di campi di cui hai bisogno o meno, puoi scegliere quali campi includere. Consulta la nostra documentazione qui per ulteriori informazioni: [https://nation.marketo.com/docs/DOC-3840](https://nation.marketo.com/docs/DOC-3840).
