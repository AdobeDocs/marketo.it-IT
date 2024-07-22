---
unique-page-id: 37355826
description: Note sulla versione -Feb '20 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Febbraio 20
exl-id: 6216b405-69c6-422b-a78c-7df0e8d271e9
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# Note sulla versione: febbraio 20 {#release-notes-feb}

Le seguenti funzioni sono incluse nella versione di febbraio 2020. Verifica la disponibilità delle funzioni nella tua edizione di Marketo.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella ( ![(stella)](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

**_Versioni trimestrali_** Le seguenti funzionalità sono state rilasciate il **21 febbraio 2020**.

## Marketo Engage core {#core-marketo-engage}

* **Azione di flusso &quot;Cambia proprietario in Microsoft&quot; di Microsoft Dynamics**: mantiene il controllo dei dati di Microsoft Dynamics CRM con la possibilità di modificare il proprietario di lead/contatti direttamente dal Marketo Engage. Questo è un miglioramento della funzionalità di integrazione CRM nativa.
* **API per la gestione degli utenti**: gestione automatizzata di utenti e ruoli tramite sistemi esterni di gestione delle identità e delle organizzazioni. Questo è un miglioramento della funzionalità Chiamate API.
* **API per schemi di oggetti personalizzati**: gestisci ed esegui il provisioning automatico degli schemi di oggetti personalizzati tra le istanze nel Marketo Engage per mantenere coerenza dei modelli di dati tra gli strumenti di vendita e marketing. Con questa API, puoi definire e testare gli oggetti personalizzati in una sandbox o in un centro di eccellenza ed eseguire il provisioning di tutte le istanze necessarie. Questo è un miglioramento della funzionalità Chiamate API. Contatta il rappresentante del Marketo Engage per scoprire come accedere a questo miglioramento.
* **API per le regole di reindirizzamento delle pagine di destinazione**: gestione automatizzata delle regole di reindirizzamento delle pagine di destinazione. Questo è un miglioramento della funzionalità Chiamate API.
* **Memorizzazione in cache dei descrittori dei moduli**: stiamo riducendo il tempo di caricamento dei moduli incorporati e migliorando la stabilità complessiva dell&#39;applicazione memorizzando nella cache i moduli come risorse. Le approvazioni ai moduli incorporati possono richiedere fino a quattro minuti per essere visualizzate sul Web. Questo è un miglioramento della funzionalità Landing Pages e Forms.

<br> 

**_Rilascio nel corso del trimestre_**

Le seguenti funzioni sono in un ciclo non trimestrale e verranno rilasciate nei prossimi mesi.

## Bizible {#bizible}

![(stella)](assets/yellow-star.png)

* **Segmentazione basata sull&#39;account**: analizza l&#39;attribuzione a livello di account con la possibilità di creare segmenti e filtri per le bacheche Discover in base agli attributi dell&#39;account. Utilizza questi segmenti per approfondire le prestazioni di marketing basate sull’account.
* **Salvataggio filtri**: salva filtri specifici per dashboard specifici di ogni utente per analizzare i dashboard in modo rapido e coerente.
* **Esporta in PDF**: condividi informazioni importanti nell&#39;organizzazione esportando dashboard Bizible come PDF.

## Sales Connect {#sales-connect}

* **Aggiornamenti finestra composizione**: il processo di selezione dei modelli e l&#39;invio di e-mail tramite Sales Connect è stato semplificato. Utilizza la finestra Componi nel nostro client web e Salesforce come punto di riferimento per i venditori, con la possibilità di salvare categorie di modelli, pianificare le e-mail, inviare le e-mail in blocco e inviare e-mail con visualizzazione e tracciamento dei clic.
* **Aggiornamenti al centro di comando**: è in corso la ricostruzione del centro di comando Sales Connect per fornire ai venditori informazioni dettagliate su tutte le e-mail, le chiamate e le attività avviate da Sales Connect. Possono inoltre visualizzare informazioni quali il coinvolgimento e-mail e il recapito messaggi dal Command Center.

<br> 

## Annunci {#announcements}

* **Success Center del Marketo Engage**: verrà avviato il Success Center di Marketo a febbraio 2020. Success Center è un centro di assistenza interno al prodotto che consente di effettuare ricerche nei documenti sui prodotti e nella community, avviare guide pratiche, accedere a contenuti di adozione come Marketo University, video sulle best practice per i colleghi e altro ancora direttamente dall’istanza del Marketo Engage. **Nota**: questa funzionalità verrà avviata come versione beta in Australia e Nuova Zelanda e verrà implementata in Nord America in un secondo momento nel corso del trimestre.

## Obsoleti {#deprecations}

* **Parametro &quot;_method&quot; di Asset API**: dopo settembre 2020, Asset API Endpoints non accetterà più &quot;_method&quot; per passare i parametri di query nel corpo di un POST per aggirare le limitazioni relative alla lunghezza degli URI. Per soddisfare le richieste che richiedevano questo parametro, il limite URI per le API Asset verrà aumentato da 6KiB a 65KiB, in modo da poter inviare URI di richiesta lunghi.
* **Supporto Internet Explorer**: a partire dalla versione di luglio del 31 luglio 2020, Internet Explorer non supporterà più l&#39;interfaccia utente del Marketo Engage.

**_Webinar sulla versione del prodotto_** [Unisciti a noi](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) il 3 marzo alle 11:00AM PT / 2:00PM ET per un webinar live ospitato dal nostro team di prodotto e ulteriori informazioni sulle funzioni incluse in questa versione.
