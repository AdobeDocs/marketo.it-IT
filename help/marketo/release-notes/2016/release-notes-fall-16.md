---
unique-page-id: 11384018
description: Note sulla versione - Autunno '16 - Documenti Marketo - Documentazione prodotto
title: Note sulla versione - Autunno 2016
translation-type: tm+mt
source-git-commit: 029d8b419ba5078980b4fde9890bdb35194bf264
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---


# Note sulla versione: Autunno &#39;16 {#release-notes-fall}

Le seguenti funzionalità sono incluse nella versione autunnale del 16. Per informazioni sulla disponibilità delle funzionalità, consulta la versione di Marketo. Fate clic sui collegamenti del titolo per visualizzare articoli dettagliati per ciascuna funzione.

## Predictive Content in Email {#predictive-content-in-email}

La nostra applicazione Predictive Content offre una nuova esperienza utente per monitorare, gestire e consigliare i contenuti attraverso i nostri algoritmi di machine learning e predittivi nei canali Web ed e-mail.

>[!NOTE]
>
>Tutti i clienti con il modulo Predictive saranno attivati entro il 10 gennaio.

![](assets/shafe.png)

Ora potete aggiungere contenuto predittivo all’e-mail. Quando l&#39;e-mail viene aperta, il destinatario riceve automaticamente i contenuti pertinenti e consigliati per aumentare il coinvolgimento e le conversioni dei contenuti.

![](assets/predictive.png)

## [Conversioni offline Facebook](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md) {#facebook-offline-conversions}

Grazie all&#39;integrazione delle conversioni offline di Facebook, i dati di conversione in Marketo (per lead pubblicitari) vengono automaticamente inviati a Facebook in modo che il team pubblicitario possa ottimizzare meglio la spesa per gli annunci. In questo Rapporto Facebook Ad Manager, le conversioni offline sono evidenziate.

![](assets/facebook.png)

## [ID universale](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md) {#universal-id}

Un ID universale consente di accedere a più iscrizioni Marketo con un singolo login e di passare rapidamente da un’iscrizione all’altra. Potete utilizzare un unico profilo community per tutte le iscrizioni.

![](assets/image2016-11-3-15-3a10-3a16.png)

>[!NOTE]
>
>Per abilitare questa funzione, contattate il supporto di Marketo.

## Miglioramenti del marketing basati su account di Marketo {#marketo-account-based-marketing-enhancements}

Ora potete assegnare i team account a account denominati in ABM (Account Based Marketing), ad esempio il proprietario dell&#39;account, il rappresentante per lo sviluppo delle vendite, il rappresentante per lo sviluppo aziendale e il responsabile del successo del cliente. Potete inoltre creare elenchi di account specifici del proprietario dell&#39;account e inviare rapporti ABM settimanali personalizzati al team dell&#39;account.

![](assets/account-team-11-15-16.png)

**REST API**

Questa release consente inoltre di gestire gli attributi di account e i punteggi di account denominati in ABM tramite l&#39;API REST di Marketo. Per ulteriori dettagli sulle operazioni API, visitare il [sito Web dedicato agli sviluppatori di Marketo](https://developers.marketo.com/rest-api/lead-database/named-accounts).

## [Miglioramenti della traccia di controllo](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) {#audit-trail-enhancements}

L&#39;audit trail fornisce una cronologia completa delle modifiche apportate all&#39;interno dell&#39;iscrizione Marketo. Sono state aggiunte ulteriori funzionalità di tracciamento per i programmi e sono state presentate importanti modifiche per campagne intelligenti, elenchi smart e modifiche apportate a utenti e ruoli.

## [Nuove autorizzazioni](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/descriptions-of-role-permissions.md) {#new-permissions}

**Rendi e-mail operativa**

Sono finiti i giorni in cui era necessario preoccuparsi che gli utenti inviassero e-mail transazionali alle persone nel database che non hanno effettuato l&#39;iscrizione. È ora possibile specificare quali utenti possono rendere operativa un&#39;e-mail o modificare le e-mail operative.

**Modifica limitazioni campagna**

Perché impostare [le limitazioni della campagna](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) se non è possibile applicarle? Quando impostate Impostazioni limite campagna per limitare il numero di persone nel database per le quali è possibile eseguire il targeting con una singola campagna, ora potete limitare gli utenti che possono ignorare queste impostazioni durante la pianificazione di una campagna.

## [Audio per notifiche push mobili](/help/marketo/product-docs/mobile-marketing/push-notifications/configure-mobile-push-notification.md) {#sound-for-mobile-push-notifications}

Attribuite alla notifica push iOS maggiore ricchezza abilitando l&#39;audio. Questa nuova funzione consente di attivare un suono quando si visualizza la notifica push sul dispositivo mobile.

>[!NOTE]
>
>* I proprietari dei dispositivi possono scegliere di impedire la riproduzione dei suoni nelle impostazioni del dispositivo, e gli sviluppatori di app possono fornire ai proprietari dei dispositivi le opzioni all&#39;interno dell&#39;app per evitare la riproduzione dei suoni.
>* I suoni vengono riprodotti automaticamente quando viene visualizzata una notifica push su un dispositivo Android.


![](assets/sound-for-push-notifications.png)

## [Informazioni sulle vendite compatibili con la crittografia Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) {#sales-insight-compatible-with-salesforce-encryption}

Market Sales Insight è ora compatibile con la crittografia Salesforce Shield. Tutti i clienti di Sales Insight devono eseguire l&#39;aggiornamento a questo pacchetto gestito più recente (versione 1.4359.2), che è [disponibile in Appexchange](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO).

## [API Account denominati](https://developers.marketo.com/rest-api/lead-database/named-accounts/) {#named-accounts-apis}

Con questa release, gli utenti di Marketo ABM possono gestire gli account denominati tramite l&#39;API Account denominati. Gli utenti possono creare, aggiornare ed eliminare account denominati, nonché leggere e aggiornare i punteggi dei conti denominati in ABM.

## [Supporto API Editor e-mail v2.0](https://developers.marketo.com/rest-api/assets/emails/) {#email-editor-v-api-support}

Gestire variabili e moduli per le e-mail in formato v2.0 utilizzando l&#39;API REST di Marketo.

## [Modifiche alla sincronizzazione di Marketo Salesforce](https://nation.marketo.com/docs/DOC-3840) {#changes-to-marketo-salesforce-sync}

L’integrazione Salesforce di Marketo si sta evolvendo per migliorare il modo in cui i campi Marketo vengono sincronizzati con Salesforce. Ora, invece di dover sincronizzare un ampio gruppo di campi che potrebbe non essere necessario, potete scegliere e scegliere quali campi includere. Per maggiori informazioni, consulta la documentazione: [https://nation.marketo.com/docs/DOC-3840](https://nation.marketo.com/docs/DOC-3840).
