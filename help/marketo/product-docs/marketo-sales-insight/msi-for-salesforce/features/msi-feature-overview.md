---
unique-page-id: 37356893
description: Panoramica delle funzioni MSI - Documentazione di Marketo - Documentazione del prodotto
title: Panoramica delle funzioni MSI
exl-id: e6cd988c-afba-44e3-b240-68258236f344
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '937'
ht-degree: 1%

---

# Panoramica delle funzioni MSI {#msi-feature-overview}

MSI dispone delle seguenti funzionalità disponibili in Salesforce Lightning e Classic.

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
* Mobile lead - Visibile nell’app mobile Salesforce
* Ponte contatti lead: visualizza il pannello MSI del contatto aggiunto nel campo ID contatto MSI

Campi:

* Ultimo momento di interesse
* Data ultimo momento di interesse
* Descrizione ultimo momento di interesse
* Sorgente ultimo momento di interesse
* Tipo ultimo momento di interesse
* Ultima attività Marketo per vendite
* Ultimo coinvolgimento Marketo per vendite
* Punteggio relativo
* Valore punteggio relativo
* Urgenza
* Valore Urgenza
* Visualizza in Marketo: fare clic su questo campo per aprire una visualizzazione non modificabile del lead in Marketo. Include: Informazioni lead, Informazioni società, Informazioni lead SFDC, Campi personalizzati SFDC, Registro attività
* ID contatto MSI: aggiungi un contatto Salesforce a questo campo e includi il pannello &quot;Ponte di contatto lead&quot; nel layout del lead per visualizzare il pannello MSI del contatto

## Layout contatto {#contact-layout}

Pagine Visualforce:

* Contatto: include l’opzione per fare clic su hyper &quot;Vai alla lista completa&quot;, verrai indirizzato a una nuova scheda in Salesforce dove il pannello MSI sarà visibile in un layout di pagina intera
* Elenco completo contatti - Non include l’opzione &quot;Vai all’elenco completo&quot;
* Contatto Mobile - Visibile nell’app mobile Salesforce
* Pagina di contatto Aggiungi a Marketo Campaign: la funzione Aggiungi a Marketo Campaign è disponibile in questo pannello

Campi:

* Ultimo momento di interesse
* Data ultimo momento di interesse
* Descrizione ultimo momento di interesse
* Sorgente ultimo momento di interesse
* Tipo ultimo momento di interesse
* Ultima attività Marketo per vendite
* Punteggio relativo
* Valore punteggio relativo
* Urgenza
* Valore Urgenza
* Visualizza in Marketo: fare clic su questo campo per aprire una visualizzazione non modificabile del lead in Marketo. Include: Informazioni lead, Informazioni società, Informazioni lead SFDC, Campi personalizzati SFDC, Registro attività
* Punteggio lead Mkto
* Informazioni sulla vendita: apre la pagina dell’elenco completo dei contatti

## Layout account {#account-layout}

Pagine Visualforce:

* Account: include l’opzione per fare clic su hyper &quot;Vai alla lista completa&quot;, verrai inviato a una nuova scheda in Salesforce dove il pannello MSI sarà visibile in un layout di pagina intera
* Elenco completo account - Non include l’opzione &quot;Vai all’elenco completo&quot;
* Account Mobile - Visibile nell’app mobile Salesforce

Campi:

* Informazioni sulla vendita: apre la pagina dell’elenco completo dei contatti

Azioni:

* Aggiungi a Marketo Campaign
* Invia e-mail Marketo
* Aggiungi/Rimuovi da elenco di controllo

Le seguenti funzioni sono **non disponibile** nella pagina Layout account:

* Stelle e fiamme

## Layout opportunità {#opportunity-layout}

Pagine Visualforce:

* Opportunità: include l’opzione per fare clic sull’icona &quot;Vai alla lista completa&quot;, verrai indirizzato a una nuova scheda in Salesforce dove il pannello MSI sarà visibile in un layout di pagina intera
* Elenco completo opportunità: non include l’opzione &quot;Vai all’elenco completo&quot;
* Opportunity Mobile - Visibile nell’app mobile Salesforce

Campi:

* Informazioni sulla vendita: apre la pagina dell’elenco completo dei contatti
* Analisi dell’opportunità Marketo - Apre Opportunity Influence Analyzer in Marketo

Azioni:

* Aggiungi a Marketo Campaign
* Invia e-mail Marketo
* Aggiungi/Rimuovi da elenco di controllo

Le seguenti funzioni sono **non disponibile** nella pagina Layout opportunità:

* Stelle e fiamme

## Visualizzazione elenco contatti e lead (azioni in blocco) {#lead-and-contact-list-view-bulk-actions}

Salesforce Lightning: Pulsanti di azione collettiva Aggiungi alla watchlist, Aggiungi a Marketo Campaign e Invia e-mail a Marketo nella vista Elenco contatti e lead.

Salesforce Classic: pulsanti Aggiungi alla watchlist, Aggiungi a Marketo Campaign e Invia in blocco e-mail Marketo nella vista Elenco contatti e lead.

## Scheda Marketo {#marketo-tab}

* Elementi di maggiore rilevanza

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

## Scheda Configurazione di Marketo Sales Insight {#marketo-sales-insight-configuration-tab}

* Impostazioni operative: include le credenziali API Soap &amp; Rest necessarie per configurare MSI in SFDC
* Configurazione MSI: include la configurazione della scheda Marketo e del pannello MSI visualforce
* Reset Marketo Sales Insight: include la possibilità di eliminare tutte le configurazioni

>[!MORELIKETHIS]
>
>[Scheda Configurazione di Marketo Sales Insight in Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.md)

## Rapporti sulle prestazioni di Sales Insight {#sales-insight-performance-reports}

Visualizzare le prestazioni delle e-mail inviate tramite Salesforce, Microsoft Dynamics o un plug-in Gmail o Outlook

## MSI per dispositivi mobili {#msi-for-mobile}

Le funzioni MSI sono supportate nell’app mobile Salesforce

## Supporto lingua {#language-support}

Marketo Sales Insight è memorizzato per lingua. Pertanto, se si desidera che funzioni per più lingue, è necessario immettere le credenziali separatamente per ciascuna lingua.

>[!NOTE]
>
>* Per poter essere aggiunto alla watchlist, un contatto/lead deve trovarsi nella partizione predefinita.
>
>* Il pacchetto MSI Salesforce non supporta la visualizzazione personalizzata con campi dipendenti.
