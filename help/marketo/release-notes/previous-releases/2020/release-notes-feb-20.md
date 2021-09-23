---
unique-page-id: 37355826
description: Note sulla versione - Feb '20 - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione - Febbraio 20
exl-id: 6216b405-69c6-422b-a78c-7df0e8d271e9
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# Note sulla versione: Feb. 20 {#release-notes-feb}

Le seguenti funzionalità sono incluse nella versione del 20 febbraio. Per informazioni sulla disponibilità delle funzioni, consulta la tua edizione Marketo .

>[!AVAILABILITY]
>
>Le caratteristiche indicate da una stella ( ![(star)](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

**_Versioni_** trimestraliLe seguenti funzionalità sono state rilasciate il 21  **febbraio 2020**.

## Marketo Engage principale {#core-marketo-engage}

* **Azione** di flusso &quot;Cambia proprietario in Microsoft&quot; di Microsoft Dynamics: Mantieni il controllo dei dati di Microsoft Dynamics CRM con la possibilità di modificare un proprietario di lead/contatti direttamente dal Marketo Engage. Questo è un miglioramento alla nostra funzionalità di integrazione CRM nativa.
* **API** di gestione utenti: Automazione della gestione di utenti e ruoli tramite sistemi di gestione di identità e organizzazioni esterne. Questo è un miglioramento della funzionalità delle chiamate API.
* **API** dello schema di oggetti personalizzati: Gestisci e distribuisci automaticamente schemi di oggetti personalizzati tra le istanze del Marketo Engage per mantenere coerenza dei modelli di dati tra gli strumenti di vendita e marketing. Con questa API, puoi definire e testare oggetti personalizzati in una sandbox o in un centro di eccellenza ed eseguire il provisioning per tutte le istanze necessarie. Questo è un miglioramento della funzionalità delle chiamate API. Per informazioni su come accedere a questo miglioramento, contatta il tuo rappresentante di Marketo Engage.
* **API per le regole di reindirizzamento delle pagine di destinazione**: Gestione automatizzata delle regole di reindirizzamento delle pagine di destinazione. Questo è un miglioramento della funzionalità delle chiamate API.
* **Memorizzazione in cache** del descrittore del modulo: Stiamo riducendo il tempo di caricamento dei moduli incorporati e migliorando la stabilità complessiva dell’applicazione memorizzando nella cache i moduli come risorse. Tieni presente che le approvazioni effettuate su moduli incorporati possono richiedere fino a quattro minuti per riflettere sul web. Questo è un miglioramento alla nostra funzionalità Pagine di destinazione e Forms.

<br> 

**_Rilascio in tutto il trimestre_**

Le seguenti caratteristiche sono su un ciclo non trimestrale e saranno rilasciate durante i prossimi mesi.

## Bizible {#bizible}

![(stella)](assets/yellow-star.png)

* **Segmentazione** basata su account: Analizza l’attribuzione a livello di account con la possibilità di creare segmenti e filtri per Discover boards in base agli attributi di account. Utilizza questi segmenti per approfondire le prestazioni di marketing basate sull’account.
* **Salvataggio dei filtri**: Salva filtri specifici per ogni utente per analizzare le dashboard in modo rapido e coerente.
* **Esporta in PDF**: È possibile condividere informazioni utili all’interno dell’organizzazione esportando dashboard Bizible come PDF.

## Sales Connect {#sales-connect}

* **Aggiornamenti** finestre di composizione: Abbiamo semplificato il processo di selezione dei modelli e invio di e-mail tramite Sales Connect. Utilizza la finestra Componi nel nostro client web e Salesforce come negozio unico per i venditori, con la possibilità di salvare le categorie di modelli, pianificare le e-mail, inviare e-mail in blocco e inviare e-mail con visualizzazione e tracciamento dei clic.
* **Aggiornamenti** del centro di comando: Stiamo ricostruendo il centro di comando di Sales Connect per fornire ai venditori informazioni approfondite su tutte le e-mail, le chiamate e le attività che sono state avviate da Sales Connect. Possono anche visualizzare informazioni come l&#39;impegno e il recapito di messaggi e-mail dal Centro comandi.

<br> 

## Annunci {#announcements}

* **Centro** di successo Marketo Engage: Lanceremo Marketo Success Center a febbraio 2020. Success Center è un centro di assistenza interno al prodotto che consente di cercare i documenti sui prodotti e la community, avviare guide informative, accedere ai contenuti relativi all’adozione, come Marketo University e video sulle best practice per i colleghi, e molto altro ancora, direttamente dall’istanza del Marketo Engage. **Nota**: Questa funzione verrà lanciata come versione beta in ANZ e verrà implementata in Nord America più avanti nel trimestre.

## Elementi obsoleti {#deprecations}

* **Parametro** &quot;_method&quot; della risorsa API: A partire da settembre 2020, gli endpoint API di Assets non accetteranno più &quot;_method&quot; per passare i parametri di query nel corpo di un POST per aggirare le limitazioni relative alla lunghezza degli URI. Per soddisfare le richieste che richiedevano questo parametro, il limite URI per le API di Assets verrà aumentato da 6KiB a 65KiB, in modo da poter inviare URI di richiesta lunghi.
* **Supporto di Internet Explorer obsoleto**: A partire dalla versione di luglio del 31 luglio 2020, Internet Explorer non supporterà più l’interfaccia utente del Marketo Engage.

**_Webinar_** [sul rilascio del prodottoIscriviti ](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) il 3 marzo alle 00:00 PT / 2:00PM ET per un webinar live ospitato dal nostro team di prodotti e scopri di più sulle funzioni incluse in questa versione.
