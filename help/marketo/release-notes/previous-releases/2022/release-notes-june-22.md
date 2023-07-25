---
description: Note sulla versione - Giugno 2022 - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione - Giugno 2022
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 0%

---

# Note sulla versione: giugno 2022 {#release-notes-june-22}

Qui sotto troverai tutte le funzioni incluse nella versione di giugno 2022. Verifica la disponibilità delle funzioni nella tua edizione di Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Caratteristiche contrassegnate da una stella (![stella](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

Le seguenti funzioni inizieranno ad essere rilasciate il **24 giugno 2022**, con un rollout graduale delle funzioni rimanenti nelle settimane successive (salvo diversa indicazione).

## Ambiente dati di marketing {#marketing-data-environment}

* **Esposizione dei campi CreatedAt/UpdatedAt per gli oggetti personalizzati**: consente di esaminare questi campi nella schermata Dettagli persona per ottenere ulteriori informazioni.

## Orchestrazione cross-channel {#cross-channel-orchestration}

* **Miglioramento della facilità d&#39;uso di Stream Designer per il Dynamic Chat**: aggiungi le schede direttamente dall’area di lavoro di Progettazione flussi senza dover essere trascinate. È stata migliorata anche l’interfaccia di Dynamic Chat per offrire una migliore visibilità dei contenuti nelle singole schede.

* **Regole di instradamento degli appuntamenti avanzate per il Dynamic Chat**: il Dynamic Chat offre più opzioni per il routing mirato degli appuntamenti. Specificare gli appuntamenti dell&#39;agente da instradare in base agli attributi di Marketo Engage, garantendo che i lead vengano instradati agli agenti appropriati.

* **Generazione di rapporti per finestre di dialogo avanzate per Dynamic Chat**: visualizza le prestazioni delle campagne di Dynamic Chat in modo più dettagliato utilizzando visualizzazioni di dati completamente nuove per le metriche di coinvolgimento e conversione.

* **Annulla sincronizzazione attributi di Marketo Engage non utilizzati per il Dynamic Chat**: dissincronizza gli attributi di Marketo Engage non utilizzati dalla sottoscrizione del Dynamic Chat, per facilitare la pulizia dei dati e consentire la sincronizzazione di attributi alternativi in base alle esigenze.

## Esperienza di nuova generazione

**Nuovo/i interruttore/interruttore di visualizzazione**: le visualizzazioni seguenti sono ora disponibili nell’esperienza di nuova generazione:

* [Visualizzazione dettagli e-mail](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [Visualizzazione elenco e-mail](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## Automazione dell’esperienza {#experience-automation}

* **Esclusioni regole di convalida campo modulo globale**: escludi moduli specifici dalle regole globali di convalida dei moduli in modo che i centri di abbonamento e altri flussi di lavoro business critical possano accettare tutti i valori.

* **Passaggi del flusso self-service**: espandi la connettività tra il Marketo Engage e il resto dello stack con la possibilità di creare passaggi di flusso personalizzati da utilizzare nelle campagne avanzate. Sia gli utenti del Marketo Engage che i partner possono sfruttare questa funzionalità per consentire l’utilizzo di servizi web esterni nelle campagne Trigger, Batch ed Eseguibili, a differenza dei webhook, che possono essere utilizzati solo nelle campagne Trigger.

* **Tracciamento collegamenti agnostici del protocollo Munchkin**: estensione del supporto per il tracciamento di `tel` e `mailto` collegamenti con Munchkin per tenere traccia di un set esteso di comportamenti web.

* **Metodi HTTP aggiuntivi per i webhook**: specifica PUT, PATCH e DELETE come tipi di richiesta per interagire con i servizi web.

## Insight sulle vendite {#sales-insight}

![(stella)](assets/yellow-star.png)

* **Autorizzazioni di Sales Insight impostate in Salesforce**: gli amministratori possono fornire l’accesso a Sales Insight a un gruppo limitato di persone a livello di utente anziché a livello di profilo tramite il set di autorizzazioni dell’app Marketo, che fa parte del pacchetto Sales Insight Salesforce.

* **Aggiornamento sezioni di My Marketo - Azioni di approfondimento sulle vendite**: gli amministratori di Marketo (e gli utenti da essi designati) possono ora passare rapidamente alla propria istanza di Sales Insight Actions (Azioni approfondimento sulle vendite) tramite una nuova sezione Sales Insight Actions (Azioni approfondimento sulle vendite) che si trova sulla pagina My Marketo (Il mio).

## Sales Connect {#sales-connect}

![(stella)](assets/yellow-star.png)

* **Aggiornamento API Salesforce**: con la versione Salesforce Summer &#39;22, le versioni legacy API 21 -30 non saranno più supportate da Salesforce. Con questa versione di Marketo Engage, tutte le richieste di Sales Connect che utilizzano versioni API legacy sono state aggiornate per rimanere all’interno di una versione supportata. Per informazioni complete sui piani di ritiro API di Salesforce, fai clic su [qui](https://help.salesforce.com/s/articleView?language=en_US&amp;type=1&amp;id=000354473){target="_blank"}.

## Miglioramenti API {#api-enhancements}

* **Nuove funzionalità di filtro per l’API Bulk Program Member Extract**: filtra per stato di iscrizione al programma, contenuto aggiornatoAlle, cadenza o esaurito per perfezionare il set di dati estratto.

* **Miglioramento dell’API di estrazione dei membri del programma in blocco**: specifica fino a 10 programmi durante la creazione di posti di lavoro per migliorare la produttività.

## Annunci {#announcements}

* **Deprecazione di Forms: Forms 1.0, endpoint di acquisizione/salvataggio lead e versioni dei moduli senza script**: il supporto per le risorse Forms 1.0 verrà completamente rimosso dal Marketo Engage entro ottobre 2022. Tutte le risorse Forms 1.0 esistenti cesseranno di funzionare. I moduli di Marketo Engage richiederanno il caricamento di JavaScript sulle pagine di destinazione e sui siti web.

**_Webinar sulla versione del prodotto_**

[Webinar sulla versione del Marketo Engage di giugno e agosto 2022](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
