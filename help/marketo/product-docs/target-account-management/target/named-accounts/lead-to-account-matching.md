---
unique-page-id: 11381156
description: Corrispondenza lead-account - Documentazione Marketo - Documentazione del prodotto
title: Lead per corrispondenza account
exl-id: 676ae500-7691-492d-abec-0cac708216b7
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# Lead per corrispondenza account {#lead-to-account-matching}

La corrispondenza a destra porta ad account denominati a destra utilizzando la corrispondenza lead-account di Marketo.

>[!NOTE]
>
>**Corrispondenza lead-account** è una funzionalità integrata di Gestione account di Marketo Target. Utilizza una logica fuzzy per far corrispondere automaticamente i lead agli account denominati giusti in tempo reale. Questi account denominati possono essere account CRM o società Marketo.

## Panoramica {#overview}

Marketo Lead-to-Account Matching segue un processo in 4 fasi:

**Passaggio 1 -** Il processo di corrispondenza inizia utilizzando le informazioni chiave sui record dei lead, ad esempio:

* Dominio e-mail (esempio: acme.com)
* Nome società dedotto dall’indirizzo IP
* Nome società: può essere il nome dell’account CRM o l’attributo del nome della società del lead (ad esempio, proveniente dalla compilazione del modulo)

**Passaggio 2 -** Vengono normalizzati i nomi di società trovati in base a vari attributi di lead (ad esempio, Acme Inc. e Acme Corp vengono normalizzati automaticamente in Acme). Questo passaggio garantisce che in Marketo sia presente una singola rappresentazione dell’account denominato e che tutti i lead possano essere visualizzati all’interno di un singolo account denominato.

**Passaggio 3 -** Abbiamo suddiviso i lead corrispondenti in 2 bucket: Corrispondenza forte e Corrispondenza debole.

* I lead con corrispondenza debole vengono visualizzati nei conti denominati che possono quindi essere risolti manualmente.

**Passaggio 4 -** Presentiamo un elenco di società proposte con corrispondenze forti e deboli. Quando un account con nome viene creato in base a una delle società proposte, vengono create regole di corrispondenza per associare automaticamente nuovi lead (ad esempio, lead compilato un modulo) agli account con nome corretto. In questo modo potrai preoccuparti meno di trovare i lead corrispondenti e più di ottenere profitti.

Poiché la corrispondenza lead-account di Marketo è una funzione incorporata di Gestione account di Marketo Target, la corrispondenza porta ad account si verifica quasi in tempo reale (ad esempio, nel momento in cui un lead compila un modulo di Marketo, detto lead viene associato all’account con il nome corretto). Questo evento può essere utilizzato per attivare avvisi e avvisare i proprietari dei nuovi lead che arrivano dai loro account denominati.

>[!NOTE]
>
>Se utilizzi LeanData in Salesforce per la corrispondenza lead-account, Marketo dispone di un’integrazione che sincronizzerà tali corrispondenze con l’istanza Marketo. Per abilitare questa funzionalità, contattare il [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) Per informazioni su come impostare i dati lean, vedere.

## Utilizzo di LeanData per la corrispondenza lead-account {#using-leandata-for-lead-to-account-matching}

Dopo che il [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) ha abilitato LeanData per il tuo account, segui i passaggi seguenti per configurarlo.

1. In Salesforce, fai clic su **Imposta Home** nella barra di navigazione a sinistra.

1. Sempre nella barra di navigazione a sinistra, in Amministrazione, fai clic su **Utenti** e quindi su **Profili**.

1. Individua e seleziona il profilo **Marketo Sync**.

1. Scorri verso il basso fino alla sezione Sicurezza a livello di campo e individua l’oggetto Lead. Seleziona **Visualizza**.

1. Per il nome del campo &quot;Reporting Matched Account&quot; (Segnalazione account corrispondente), accertati che la casella di controllo nella colonna **Read Access** (Accesso in lettura) sia selezionata.

1. In Marketo, vai alla sezione **Amministratore**.

   ![](assets/lead-to-account-matching-1.png)

1. Selezionare **Gestione campi**.

   ![](assets/lead-to-account-matching-2.png)

1. Conferma che il campo sia presente ricercando &quot;Reporting Matched Account&quot; (Segnalazione account corrispondente).

   ![](assets/lead-to-account-matching-3.png)

>[!MORELIKETHIS]
>
>[Individua account](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md)
