---
unique-page-id: 37356893
description: Panoramica delle funzioni MSI - Documentazione di Marketo - Documentazione del prodotto
title: Panoramica delle funzioni MSI
exl-id: e6cd988c-afba-44e3-b240-68258236f344
feature: Marketo Sales Insights
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 0%

---

# Panoramica delle funzioni MSI {#msi-feature-overview}

In [!DNL Salesforce] Lightning e Classic sono disponibili le seguenti funzionalità di MSI.

>[!NOTE]
>
>Per visualizzare tutti i dati disponibili, assicurati che lo zoom del browser sia impostato su un valore non superiore al 125% quando utilizzi Windows e al 150% sul sistema operativo Mac.

## Pannello Visualforce {#visualforce-panel}

Il pannello MSI Visualforce include le seguenti funzionalità:

* Schede

   * [Dashboard approfondimenti](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)
   * Momenti di interesse
   * Attività web
   * E-mail
   * Punteggio

* Azioni

   * Aggiungi a Marketo Campaign
   * Invia e-mail Marketo
   * Aggiungi/Rimuovi da elenco di controllo

* Stelle e fiamme

## Layout lead {#lead-layout}

Pagine Visualforce:

* Lead: include l’opzione per fare clic su hyper &quot;Vai alla lista completa&quot;, verrai inviato a una nuova scheda in Salesforce dove il pannello MSI sarà visibile in un layout di pagina intera
* Elenco completo lead: non include l’opzione &quot;Vai all’elenco completo&quot;
* Mobile lead: visibile nell’app mobile Salesforce
* Bridge contatto lead: visualizza il pannello MSI del contatto aggiunto nel campo ID contatto MSI

Campi:

* Ultimo momento di interesse
* Data ultimo momento di interesse
* Descrizione ultimo momento di interesse
* Ultimo momento di interesse Source
* Tipo ultimo momento di interesse
* Ultima attività Marketo per vendite
* Ultimo coinvolgimento Marketo per vendite
* Punteggio relativo
* Valore punteggio relativo
* Urgenza
* Valore Urgenza
* Visualizza in Marketo: fare clic su questo campo per aprire una visualizzazione non modificabile del lead in Marketo. Include: Informazioni lead, Informazioni società, Informazioni lead SFDC, Campi personalizzati SFDC, Registro attività
* ID contatto MSI: aggiungi un contatto Salesforce a questo campo e includi il pannello &quot;Contatto lead Bridge&quot; nel layout del lead per visualizzare il pannello MSI del contatto

## Layout contatto {#contact-layout}

Pagine Visualforce:

* Contatto: include l’opzione per fare clic su hyper &quot;Vai alla lista completa&quot;, verrai inviato a una nuova scheda in Salesforce dove il pannello MSI sarà visibile in un layout di pagina intera
* Elenco completo contatti - Non include l’opzione &quot;Vai all’elenco completo&quot;
* Contatto Mobile - Visibile nell’app mobile Salesforce
* Pagina di contatto Aggiungi a Marketo Campaign: la funzione Aggiungi a Marketo Campaign è disponibile in questo pannello

Campi:

* Ultimo momento di interesse
* Data ultimo momento di interesse
* Descrizione ultimo momento di interesse
* Ultimo momento di interesse Source
* Tipo ultimo momento di interesse
* Ultima attività Marketo per vendite
* Punteggio relativo
* Valore punteggio relativo
* Urgenza
* Valore Urgenza
* Visualizza in Marketo: fare clic su questo campo per aprire una visualizzazione non modificabile del lead in Marketo. Include: Informazioni lead, Informazioni società, Informazioni lead SFDC, Campi personalizzati SFDC, Registro attività
* Punteggio lead Mkto
* [!DNL Sales Insight] - Apre la pagina dell&#39;elenco completo contatti

## Layout account {#account-layout}

Pagine Visualforce:

* Account: include l’opzione per fare clic su hyper &quot;Vai alla lista completa&quot;, verrai inviato a una nuova scheda in Salesforce dove il pannello MSI sarà visibile in un layout di pagina intera
* Elenco completo account - Non include l’opzione &quot;Vai all’elenco completo&quot;
* Account Mobile - Visibile nell’app mobile Salesforce

Campi:

* [!DNL Sales Insight] - Apre la pagina dell&#39;elenco completo contatti

Azioni:

* Aggiungi a Marketo Campaign
* Invia e-mail Marketo
* Aggiungi/Rimuovi da elenco di controllo

Le seguenti funzionalità sono **non disponibili** nella pagina Layout account:

* Stelle e fiamme

## Layout opportunità {#opportunity-layout}

Pagine Visualforce:

* Opportunità: include l’opzione per fare clic sull’icona &quot;Vai all’elenco completo&quot;, che verrà inviata a una nuova scheda in Salesforce dove il pannello MSI sarà visibile in un layout di pagina intera
* Elenco completo opportunità: non include l’opzione &quot;Vai all’elenco completo&quot;
* Opportunità mobile: visibile nell’app mobile Salesforce

Campi:

* [!DNL Sales Insight] - Apre la pagina dell&#39;elenco completo contatti
* Analisi dell’opportunità Marketo - Apre Opportunity Influence Analyzer in Marketo

Azioni:

* Aggiungi a Marketo Campaign
* Invia e-mail Marketo
* Aggiungi/Rimuovi da elenco di controllo

Le seguenti funzionalità sono **non disponibili** nella pagina Layout opportunità:

* Stelle e fiamme

## Visualizzazione elenco contatti e lead (azioni in blocco) {#lead-and-contact-list-view-bulk-actions}

[!DNL Salesforce Lightning]: pulsanti Aggiungi alla watchlist, Aggiungi a Marketo Campaign e Invia e-mail a Marketo nella visualizzazione elenco contatti e lead.

[!DNL Salesforce Classic]: pulsanti Aggiungi alla watchlist, Aggiungi a Marketo Campaign e Invia e-mail a Marketo nella visualizzazione elenco contatti e lead.

## Scheda Marketo {#marketo-tab}

* [!DNL Best Bets]

   * Include la possibilità di creare e modificare le viste. Possibilità di nascondere gli elementi di maggiore rilevanza a seconda della configurazione dell’opzione &quot;Nascondi predefinito&quot; nella pagina Configurazione di Marketo
   * Colonne - Nome, Account, Ultimo momento di interesse, Intestazione di stato, Coinvolgimento (stelle e fiamme), Nascondi

* Il mio elenco di controllo

   * Include la possibilità di creare e modificare le viste
   * Colonne - Nome, Account, Ultimo momento di interesse, Intestazione di stato, Coinvolgimento (stelle e fiamme), Rimuovi

* Attività web

   * Include la possibilità di creare e modificare le viste, la funzionalità filtro per intervalli di tempo
   * Colonna: visualizzazione pagina, nome, account, ultima visita

* Attività Web anonima

   * Include la possibilità di creare e modificare le viste, la funzionalità filtro per intervalli di tempo
   * Colonne - Visualizzazione pagina, Società, Ultima visita, Ricerca (apre la pagina LinkedIn dell’azienda)

* E-mail

   * Include la possibilità di creare e modificare le viste
   * Colonne: Nome, Account, Oggetto, Data, Apri, Fai clic su

* Feed lead: include la possibilità di iscriversi a momenti interessanti, il feed RSS nella pagina Configurazione deve essere abilitato per utilizzare questa funzione

   * Lead/Contatto che ha avuto questo momento interessante
   * Tipo di momento di interesse (web, e-mail o milestone) e descrizione
   * Nome account
   * Ora in cui si è verificato questo momento interessante
   * Opzione di abbonamento per ricevere notifiche e-mail per questo tipo di evento
   * Icona ad alta priorità per mostrare che questa persona è l&#39;elemento di maggiore rilevanza

## Scheda Configurazione [!DNL Marketo Sales Insight] {#marketo-sales-insight-configuration-tab}

* Impostazioni operative: include le credenziali API Soap &amp; Rest necessarie per configurare MSI in SFDC
* Configurazione MSI: include la configurazione della scheda Marketo e del pannello MSI visualforce
* Reimposta [!DNL Marketo Sales Insight]: include la possibilità di eliminare tutte le configurazioni

>[!MORELIKETHIS]
>
>[[!DNL Marketo Sales Insight] Scheda Configurazione in [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.md)

## [!DNL Sales Insight] report prestazioni {#sales-insight-performance-reports}

Visualizza le prestazioni delle e-mail inviate tramite [!DNL Salesforce], [!DNL Microsoft Dynamics] o un plug-in Gmail o [!DNL Outlook]

## MSI per dispositivi mobili {#msi-for-mobile}

Le funzionalità MSI sono supportate nell&#39;applicazione mobile [!DNL Salesforce]

## Supporto lingua {#language-support}

[!DNL Marketo Sales Insight] è archiviato per lingua. Pertanto, se si desidera che funzioni per più lingue, è necessario immettere le credenziali separatamente per ciascuna lingua.

>[!NOTE]
>
>* Per poter essere aggiunto alla watchlist, un contatto/lead deve trovarsi nella partizione predefinita.
>
>* Il pacchetto MSI [!DNL Salesforce] non supporta la visualizzazione personalizzata con campi dipendenti.
