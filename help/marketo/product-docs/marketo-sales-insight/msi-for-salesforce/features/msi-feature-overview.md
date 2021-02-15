---
unique-page-id: 37356893
description: Panoramica delle funzioni MSI - Documenti Marketo - Documentazione del prodotto
title: Panoramica delle funzioni MSI
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---


# Panoramica delle funzioni MSI {#msi-feature-overview}

MSI dispone delle seguenti funzionalità in Salesforce Lightning e Classic.

## Pannello Visualforce {#visualforce-panel}

Il pannello MSI Visualforce include le seguenti funzionalità:

* Schede

   * [Pannello Insights](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)
   * Momento interessante
   * Attività Web
   * E-mail
   * Punteggio

* Azioni

   * Aggiungi a campagna Marketo
   * Invia e-mail Marketo
   * Aggiungi/rimuovi da elenco di controllo

* Stelle e fiamme

## Layout lead {#lead-layout}

Pagine Visualforce:

* Lead - Include l&#39;opzione di fare clic sull&#39;iper &quot;Vai a elenco completo&quot;, si verrà inviati a una nuova scheda in Salesforce dove il pannello MSI sarà visibile in un layout di pagina completo
* Elenco completo lead - Non include l’opzione &quot;Vai a elenco completo&quot;
* Mobile lead - Visibile nell’applicazione mobile Salesforce
* Lead Contact Bridge - Visualizza il pannello MSI del contatto aggiunto nel campo ID contatto MSI

Campi:

* Ultimo momento interessante
* Data ultimo momento interessante
* Ultimo interessante momento
* Ultima origine momento interessante
* Ultimo tipo di momento interessante
* Ultima attività di marketing per vendite
* Ultimo coinvolgimento marketing per vendite
* Punteggio relativo
* Valore punteggio relativo
* Urgenza
* Valore di urgenza
* Visualizza in Marketo - Fai clic su questo campo per aprire una vista non modificabile del lead in Marketo. Include: Informazioni lead, Informazioni società, Informazioni lead SFDC, Campi personalizzati SFDC, Registro attività
* ID contatto MSI - Aggiungi un contatto Salesforce a questo campo e includi il pannello &quot;Lead Contact Bridge&quot; nel layout lead per visualizzare il pannello MSI del contatto

## Layout contatto {#contact-layout}

Pagine Visualforce:

* Contatto - Include l&#39;opzione per fare clic sull&#39;iper &quot;Vai a elenco completo&quot;, si verrà inviati a una nuova scheda in Salesforce dove il pannello MSI sarà visibile in un layout di pagina completo
* Contatta elenco completo - Non include l&#39;opzione &quot;Vai a elenco completo&quot;
* Contatta mobile - Visibile nell’applicazione mobile Salesforce
* Aggiungi a pagina di contatto della campagna Marketo - Aggiungi alla campagna Marketo è disponibile in questo pannello

Campi:

* Ultimo momento interessante
* Data ultimo momento interessante
* Ultimo interessante momento
* Ultima origine momento interessante
* Ultimo tipo di momento interessante
* Ultima attività di marketing per vendite
* Punteggio relativo
* Valore punteggio relativo
* Urgenza
* Valore di urgenza
* Visualizza in Marketo - Fai clic su questo campo per aprire una vista non modificabile del lead in Marketo. Include: Informazioni lead, Informazioni società, Informazioni lead SFDC, Campi personalizzati SFDC, Registro attività
* Punteggio lead Mkto
* Informazioni sulle vendite - Apre la pagina elenco completo dei contatti

## Layout account {#account-layout}

Pagine Visualforce:

* Account - Include l&#39;opzione per fare clic su &quot;Vai a elenco completo&quot;, si verrà inviati a una nuova scheda in Salesforce dove il pannello MSI sarà visibile in un layout di pagina completo
* Elenco completo account - Non include l&#39;opzione &quot;Vai a elenco completo&quot;
* Account Mobile - Visibile nell&#39;applicazione mobile Salesforce

Campi:

* Informazioni sulle vendite - Apre la pagina elenco completo dei contatti

Le seguenti funzionalità sono **non disponibili** nella pagina Layout account:

* Azioni: Aggiungi a campagna Marketo, Invia e-mail Marketo, Aggiungi/Rimuovi da elenco di controllo
* Stelle e fiamme

## Layout opportunità {#opportunity-layout}

Pagine Visualforce:

* Opportunità - Include l&#39;opzione di fare clic sull&#39;iper &quot;Vai a elenco completo&quot;, verrà inviata a una nuova scheda in Salesforce dove il pannello MSI sarà visibile in un layout di pagina completo
* Elenco completo opportunità - Non include l&#39;opzione &quot;Vai a elenco completo&quot;
* Opportunità mobile - Visibile nell&#39;applicazione mobile Salesforce

Campi:

* Informazioni sulle vendite - Apre la pagina elenco completo dei contatti
* Analisi opportunità Marketo - Apre l&#39;analisi dell&#39;influenza opportunità in Marketo

Le seguenti funzionalità sono **non disponibili** nella pagina Layout opportunità:

* Azioni: Aggiungi a campagna Marketo, Invia e-mail Marketo, Aggiungi/Rimuovi da elenco di controllo
* Stelle e fiamme

## Visualizzazione Elenco contatti e lead (azioni di massa) {#lead-and-contact-list-view-bulk-actions}

Salesforce Lightning: Aggiungi a elenco di controllo, Aggiungi a campagna Marketo e Invia per e-mail i pulsanti delle azioni di massa di Marketo nella visualizzazione Elenco contatti e lead.

Salesforce Classic: Aggiungi a elenco di controllo, Aggiungi a campagna Marketo e Invia per e-mail i pulsanti delle azioni di massa di Marketo nella visualizzazione Elenco contatti e lead.

## Scheda Marketo {#marketo-tab}

* Best Bets

   * Include la possibilità di creare e modificare le viste. Possibilità di nascondere le migliori Scommesse a seconda della configurazione dell&#39;opzione &quot;Nascondi predefinito&quot; nella pagina Configurazione Marketo
   * Colonne - Nome, Account, Ultimo momento interessante, Intestazione stato, Coinvolgimento (Stelle e fiamme), Nascondi

* Elenco orologi personali

   * Include la possibilità di creare e modificare le viste
   * Colonne - Nome, Account, Ultimo momento interessante, Intestazione stato, Coinvolgimento (Stelle e fiamme), Rimuovi

* Attività Web

   * Include la possibilità di creare e modificare viste, la funzionalità del filtro per l&#39;intervallo di tempo
   * Colonna - Visualizzazione pagina, Nome, Account, Ultima visita

* Attività Web anonima

   * Include la possibilità di creare e modificare viste, la funzionalità del filtro per l&#39;intervallo di tempo
   * Colonne - Visualizzazioni pagina, Società, Ultima visita, Ricerche (apre la pagina LinkedIn della società)

* E-mail

   * Include la possibilità di creare e modificare le viste
   * Colonne - Nome, Account, Oggetto, Data, Apertura, Clic

* Feed lead - Include la possibilità di iscriversi a momenti interessanti, il feed RSS nella pagina di configurazione deve essere abilitato per utilizzare questa funzione

   * Lead/Contatto con questo momento interessante
   * Interessante tipo di momento (web, e-mail o pietra miliare) e descrizione
   * Nome account
   * Ora che questo momento interessante si è verificato
   * Iscriviti per ricevere le notifiche e-mail per questo tipo di evento
   * Icona ad alta priorità per mostrare a questa persona una migliore scommessa

## Scheda Configurazione analisi vendite marketing {#marketo-sales-insight-configuration-tab}

* Impostazioni operative: Include le credenziali API Soap &amp; Rest necessarie per configurare MSI in SFDC
* Configurazione MSI: Include la configurazione della scheda Marketo e del pannello delle forze visive MSI
* Reimposta analisi vendite marketing: Include la possibilità di cancellare tutte le configurazioni

>[!MORELIKETHIS]
>
>[Scheda Configurazione analisi vendite Marketo in Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.md)

## Report sulle prestazioni di Sales Insight {#sales-insight-performance-reports}

Visualizzare le prestazioni dei messaggi e-mail inviati tramite Salesforce, Microsoft Dynamics o un plug-in Gmail o Outlook

## MSI per dispositivi mobili {#msi-for-mobile}

Le funzioni MSI sono supportate nell’applicazione mobile Salesforce

## Supporto lingua {#language-support}

Marketing Sales Insight è memorizzato per lingua. Se desiderate che funzioni per più lingue, dovete immettere le credenziali separatamente per ciascuna lingua.
