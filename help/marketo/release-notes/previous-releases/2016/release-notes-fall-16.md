---
unique-page-id: 11384018
description: Note sulla versione -Autunno '16 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Autunno '16
exl-id: da935951-162e-426c-acf2-12c55ff706b4
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 0%

---

# Note sulla versione: Autunno &#39;16 {#release-notes-fall}

Le seguenti funzioni sono incluse nella versione di autunno del 1916. Verifica la disponibilità delle funzioni nella tua edizione di Marketo. Fai clic sui collegamenti del titolo per visualizzare articoli dettagliati per ciascuna funzione.

## Contenuto predittivo nelle e-mail {#predictive-content-in-email}

È disponibile una nuova esperienza utente per la nostra applicazione Predictive Content che consente di monitorare, gestire e consigliare i contenuti attraverso l’apprendimento automatico e gli algoritmi predittivi nei canali web ed e-mail.

>[!NOTE]
>
>Tutti i clienti che dispongono del modulo Predictive saranno abilitati entro il 10 gennaio.

![](assets/shafe.png)

Ora puoi aggiungere contenuto predittivo all’e-mail. Quando l’e-mail viene aperta, il destinatario riceve automaticamente contenuti pertinenti e consigliati che contribuiscono ad aumentare il coinvolgimento e le conversioni dei contenuti.

![](assets/predictive.png)

## [Conversioni offline facebook](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md) {#facebook-offline-conversions}

Con l’integrazione delle conversioni offline di Facebook, i dati di conversione in Marketo (per lead di annunci) vengono automaticamente rimandati a Facebook in modo che il team pubblicitario possa ottimizzare la spesa pubblicitaria. In questo rapporto di Facebook Ad Manager, vengono evidenziate le conversioni offline.

![](assets/facebook.png)

## [ID universale](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md) {#universal-id}

Un Universal ID consente di accedere a più abbonamenti Marketo con un unico accesso e di passare rapidamente da un abbonamento all’altro. Puoi utilizzare un singolo profilo community per tutti gli abbonamenti.

![](assets/image2016-11-3-15-3a10-3a16.png)

>[!NOTE]
>
>Contatta il supporto Marketo per abilitare questa funzione.

## Miglioramenti del marketing basato su account Marketo {#marketo-account-based-marketing-enhancements}

Ora è possibile assegnare i team dell&#39;account ad account denominati in Account Based Marketing (ABM), ad esempio il proprietario dell&#39;account, il rappresentante per lo sviluppo delle vendite, il rappresentante per lo sviluppo commerciale e l&#39;account manager. Puoi anche creare elenchi di account specifici del proprietario dell’account e inviare rapporti ABM settimanali personalizzati al team dell’account.

![](assets/account-team-11-15-16.png)

**API REST**

Questa versione consente inoltre di gestire gli attributi e i punteggi degli account denominati in ABM utilizzando l’API REST di Marketo. Per ulteriori dettagli sulle operazioni API, visita il [Sito web Marketo Developers](https://developers.marketo.com/rest-api/lead-database/named-accounts).

## [Miglioramenti di Audit Trail](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) {#audit-trail-enhancements}

Audit trail fornisce una cronologia completa delle modifiche apportate all’interno dell’abbonamento Marketo. Sono state aggiunte ulteriori funzionalità di tracciamento per i programmi e sono stati evidenziati importanti dettagli di modifica per campagne intelligenti, elenchi avanzati e modifiche apportate a utenti e ruoli.

## [Nuove autorizzazioni](/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md) {#new-permissions}

**Rendi operativa l’e-mail**

Sono finiti i giorni in cui dovevi preoccuparti che gli utenti inviassero e-mail transazionali a persone del tuo database che hanno annullato l’abbonamento. Ora puoi specificare quali utenti possono rendere operativa un’e-mail o modificarne le e-mail operative.

**Modifica restrizioni campagna**

Perché impostare [restrizioni delle campagne](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) se non riesci a farle rispettare? Quando imposti Impostazioni limite campagna in modo da limitare il numero di persone nel database a cui è possibile indirizzare una singola campagna, ora puoi limitare quali utenti possono ignorare queste impostazioni durante la pianificazione di una campagna.

## [Suono per le notifiche push per dispositivi mobili](/help/marketo/product-docs/mobile-marketing/push-notifications/configure-mobile-push-notification.md) {#sound-for-mobile-push-notifications}

Rendi più ricca la tua notifica push di iOS grazie all’abilitazione dell’audio. Questa nuova funzione consente di attivare un suono quando viene visualizzata una notifica push sul dispositivo mobile.

>[!NOTE]
>
>* I proprietari dei dispositivi possono scegliere di impedire la riproduzione dei suoni nelle impostazioni del dispositivo e gli sviluppatori di app possono assegnare ai proprietari dei dispositivi opzioni all’interno dell’app per impedire la riproduzione dei suoni.
>* I suoni vengono riprodotti automaticamente quando una notifica push viene visualizzata su un dispositivo Android.

![](assets/sound-for-push-notifications.png)

## [Sales Insight compatibile con la crittografia Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) {#sales-insight-compatible-with-salesforce-encryption}

Market Sales Insight è ora compatibile con Salesforce Shield Encryption. Tutti i clienti Sales Insight devono effettuare l’aggiornamento a questo pacchetto gestito più recente (versione 1.4359.2), che è [disponibile su Appexchange](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO).

## [API degli account denominati](https://developers.marketo.com/rest-api/lead-database/named-accounts/) {#named-accounts-apis}

Con questa versione, gli utenti ABM di Marketo possono gestire account denominati tramite l’API Account denominati. Gli utenti possono creare, aggiornare ed eliminare account denominati, nonché leggere e aggiornare i punteggi degli account denominati ABM.

## [Supporto API dell’editor e-mail v2.0](https://developers.marketo.com/rest-api/assets/emails/) {#email-editor-v-api-support}

Gestisci variabili e moduli per le e-mail in formato v2.0 utilizzando l’API REST di Marketo.

## [Modifiche a Marketo Salesforce Sync](https://nation.marketo.com/docs/DOC-3840) {#changes-to-marketo-salesforce-sync}

L’integrazione di Marketo con Salesforce si sta evolvendo per migliorare il modo in cui i campi Marketo vengono sincronizzati con Salesforce. Ora, invece di dover sincronizzare un ampio gruppo di campi che potrebbero essere necessari o meno, puoi scegliere quali campi includere. Consulta la documentazione qui per ulteriori informazioni: [https://nation.marketo.com/docs/DOC-3840](https://nation.marketo.com/docs/DOC-3840).
