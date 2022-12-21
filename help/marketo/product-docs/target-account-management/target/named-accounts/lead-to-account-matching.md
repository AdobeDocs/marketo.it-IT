---
unique-page-id: 11381156
description: Corrispondenza lead a account - Documenti Marketo - Documentazione del prodotto
title: Corrispondenza lead a conto
exl-id: 676ae500-7691-492d-abec-0cac708216b7
source-git-commit: 98388f1ed941b321449e6e8badac0153dc2245ba
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Corrispondenza lead a conto {#lead-to-account-matching}

La corrispondenza a destra conduce agli account con nome destro utilizzando la corrispondenza lead-to-account di Marketo.

>[!NOTE]
>
>**Corrispondenza lead-to-account** è una funzione integrata di Gestione account di Marketo Target. Utilizza una logica confusa per far corrispondere automaticamente i lead ai giusti account denominati in tempo quasi reale. Questi account denominati possono essere account CRM o società Marketo.

## Panoramica {#overview}

La corrispondenza lead-to-account di Marketo segue un processo in 4 fasi:

**Passaggio 1 -** Il nostro processo di corrispondenza inizia utilizzando le informazioni chiave sui record lead, ad esempio:

* Dominio e-mail (ad esempio, acme.com)
* Nome della società oggetto dell’offerta dall’indirizzo IP
* Nome società: potrebbe essere il nome dell’account CRM o l’attributo del nome della società principale (ad esempio, proveniente dalla compilazione del modulo)

**Passaggio 2 -** Normalizziamo i nomi aziendali che troviamo in base a vari attributi di lead (ad esempio, Acme Inc. e Acme Corp vengono automaticamente normalizzati in Acme). Questo passaggio ci assicura una singola rappresentazione dell’account denominato in Marketo e può visualizzare tutti i lead all’interno di un singolo account denominato.

**Passaggio 3 -** Dividi i lead abbinati in 2 blocchi: Corrispondenza forte e Corrispondenza debole.

* I lead con corrispondenza debole vengono visualizzati sugli account denominati e possono quindi essere risolti manualmente.

**Passaggio 4 -** Presentiamo un elenco di società proposte con forti e deboli corrispondenze. Quando un account denominato viene creato in base a una delle società proposte, creiamo regole di corrispondenza per associare automaticamente nuovi lead (ad esempio, lead ha compilato un modulo) andando avanti verso i giusti account denominati. In questo modo puoi preoccuparti meno della corrispondenza dei lead e più di ottenere ricavi!

Poiché la corrispondenza lead-to-account di Marketo è una funzione integrata di Gestione account di Marketo Target, la corrispondenza dei lead agli account avviene in tempo quasi reale (ad esempio, nel momento in cui un lead compila un modulo Marketo, associamo detto lead all’account con il nome giusto). Questo evento può essere utilizzato per attivare gli avvisi e avvisare i proprietari dell&#39;account dei nuovi lead che arrivano dai loro account denominati.

>[!NOTE]
>
>Se utilizzi LeanData in Salesforce per eseguire la corrispondenza lead-to-account, Marketo dispone di un’integrazione che sincronizza le corrispondenze con la tua istanza Marketo. Per abilitare questa funzione, contatta [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) Scopri come impostare LeanData di seguito.

## Utilizzo di dati magri per la corrispondenza tra lead e account {#using-leandata-for-lead-to-account-matching}

Dopo [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) ha abilitato LeanData per il tuo account, segui i passaggi seguenti per configurarlo.

1. In Salesforce, fai clic su **Pagina iniziale configurazione** nel menu di navigazione a sinistra.

1. Ancora nel menu di navigazione a sinistra, in Amministrazione, fai clic su **Utenti** then **Profili**.

1. Individua e seleziona la **Sincronizzazione Marketo** profilo.

1. Scorri verso il basso fino alla sezione Sicurezza a livello di campo e individua l’oggetto Lead. Seleziona **Visualizza**.

1. Per il nome del campo &quot;Reporting Matched Account&quot;, assicurati che la casella di controllo sia presente nel campo **Accesso in lettura** è selezionata.

1. In Marketo, vai alla pagina **Amministratore** sezione .

   ![](assets/lead-to-account-matching-1.png)

1. Seleziona **Gestione dei campi**.

   ![](assets/lead-to-account-matching-2.png)

1. Confermare la presenza del campo selezionando &quot;Reporting Matched Account&quot; (Reporting Matched Account correlato).

   ![](assets/lead-to-account-matching-3.png)

>[!MORELIKETHIS]
>
>[Scopri account](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md)
