---
unique-page-id: 37355826
description: Note sulla versione -Feb '20 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Febbraio 20
exl-id: 6216b405-69c6-422b-a78c-7df0e8d271e9
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 2%

---

# Note sulla versione - Febbraio 2020 {#release-notes-feb}

Le seguenti funzioni sono incluse nella versione di febbraio 2020. Verifica la disponibilità delle funzioni nella tua edizione di Marketo.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella ( ![(stella)](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

**_Versioni trimestrali_** Le seguenti funzionalità sono state rilasciate il **21 febbraio 2020**.

## Marketo Engage core {#core-marketo-engage}

* Azione di flusso **[!DNL Microsoft Dynamics]&quot;Change Owner in Microsoft&quot; di**: mantieni il controllo dei tuoi dati di gestione delle relazioni con i clienti [!DNL Microsoft Dynamics] con la possibilità di modificare un proprietario lead/contatto direttamente da Marketo Engage. Questo è un miglioramento della funzionalità di integrazione CRM nativa.
* **API per la gestione degli utenti**: gestione automatizzata di utenti e ruoli tramite sistemi esterni di gestione delle identità e delle organizzazioni. Questo è un miglioramento della funzionalità Chiamate API.
* **API per schemi di oggetti personalizzati**: gestisci ed esegui il provisioning automatico degli schemi di oggetti personalizzati tra le istanze in Marketo Engage per mantenere coerenza tra i modelli di dati degli strumenti di vendita e marketing. Con questa API, puoi definire e testare gli oggetti personalizzati in una sandbox o in un centro di eccellenza ed eseguire il provisioning di tutte le istanze necessarie. Questo è un miglioramento della funzionalità Chiamate API. Per informazioni su come ottenere l’accesso a questo miglioramento, contatta il rappresentante Marketo Engage.
* **API per le regole di reindirizzamento delle pagine di destinazione**: gestione automatizzata delle regole di reindirizzamento delle pagine di destinazione. Questo è un miglioramento della funzionalità Chiamate API.
* **Memorizzazione in cache dei descrittori dei moduli**: stiamo riducendo il tempo di caricamento dei moduli incorporati e migliorando la stabilità complessiva dell&#39;applicazione memorizzando nella cache i moduli come risorse. Le approvazioni ai moduli incorporati possono richiedere fino a quattro minuti per essere visualizzate sul Web. Questo è un miglioramento della funzionalità Landing Pages e Forms.

<br> 

**_Rilascio nel corso del trimestre_**

Le seguenti funzioni sono in un ciclo non trimestrale e verranno rilasciate nei prossimi mesi.

## [!DNL Bizible] {#bizible}

![(stella)](assets/yellow-star.png)

* **Segmentazione basata sull&#39;account**: analizza l&#39;attribuzione a livello di account con la possibilità di creare segmenti e filtri per le bacheche Discover in base agli attributi dell&#39;account. Utilizza questi segmenti per approfondire le prestazioni di marketing basate sull’account.
* **Salvataggio filtri**: salva filtri specifici per dashboard specifici di ogni utente per analizzare i dashboard in modo rapido e coerente.
* **Esporta in PDF**: condividi informazioni importanti nell&#39;organizzazione esportando dashboard Bizible come PDF.

## [!DNL Sales Connect] {#sales-connect}

* **Aggiornamenti finestra composizione**: il processo di selezione dei modelli e l&#39;invio di e-mail tramite [!DNL Sales Connect] è stato semplificato. Utilizza la finestra Componi nel nostro client web e Salesforce come punto di riferimento per i venditori, con la possibilità di salvare categorie di modelli, pianificare le e-mail, inviare le e-mail in blocco e inviare e-mail con visualizzazione e tracciamento dei clic.
* **Aggiornamenti del centro di comando**: è in corso la ricostruzione del centro di comando [!DNL Sales Connect] per consentire ai venditori insight di accedere a tutte le e-mail, le chiamate e le attività avviate da [!DNL Sales Connect]. Possono inoltre visualizzare informazioni quali il coinvolgimento e-mail e il recapito messaggi dal Command Center.

<br> 

## Annunci {#announcements}

* **Success Center di Marketo Engage**: verrà avviato il Success Center di Marketo a febbraio 2020. Success Center è un centro di assistenza interno al prodotto che consente di effettuare ricerche nei documenti sui prodotti e nella community, avviare guide pratiche, accedere a contenuti di adozione come Marketo University, video sulle best practice per i colleghi e altro ancora direttamente dall’istanza di Marketo Engage. **Nota**: questa funzionalità verrà avviata come versione beta in Australia e Nuova Zelanda e verrà implementata in Nord America in un secondo momento nel corso del trimestre.

## Funzionalità deprecate {#deprecations}

* **Parametro &quot;_method&quot; di Asset API**: dopo settembre 2020, Asset API Endpoints non accetterà più &quot;_method&quot; per passare i parametri di query nel corpo di un POST per aggirare le limitazioni relative alla lunghezza degli URI. Per soddisfare le richieste che richiedevano questo parametro, il limite URI per le API Asset verrà aumentato da 6KiB a 65KiB, in modo da poter inviare URI di richiesta lunghi.
* **Supporto Internet Explorer**: a partire dalla versione di luglio del 31 luglio 2020, l&#39;interfaccia utente di Marketo Engage non sarà più supportata in Internet Explorer.

**_Webinar sulla versione del prodotto_** [Unisciti a noi](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) il 3 marzo alle 11:00AM PT / 2:00PM ET per un webinar live ospitato dal nostro team di prodotto e ulteriori informazioni sulle funzioni incluse in questa versione.
