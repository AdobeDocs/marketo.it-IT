---
description: Note sulla versione - Giugno 2022 - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione - Giugno 2022
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
feature: Release Information
source-git-commit: cf4dcb6a316eba631ccb73a991c09e83c80b82ca
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# Note sulla versione: giugno 2022 {#release-notes-june-22}

Qui sotto troverai tutte le funzioni incluse nella versione di giugno 2022. Verifica la disponibilità delle funzioni nella tua edizione di Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![stella](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

Le seguenti funzionalità inizieranno a essere rilasciate il **24 giugno 2022**, con un rollout graduale delle funzioni rimanenti nelle settimane successive (salvo diversa indicazione).

## Ambiente dati di marketing {#marketing-data-environment}

* **Esposizione dei campi CreatedAt/UpdatedAt per gli oggetti personalizzati**: consente di esaminare questi campi nella schermata Dettagli persona per ottenere ulteriori informazioni.

## Orchestrazione cross-channel {#cross-channel-orchestration}

* **È stata migliorata la facilità di utilizzo di Stream Designer per il Dynamic Chat**: è possibile aggiungere schede direttamente dall&#39;area di lavoro di Stream Designer senza dover essere trascinate. È stata migliorata anche l’interfaccia di Dynamic Chat per offrire una migliore visibilità dei contenuti nelle singole schede.

* **Regole di routing degli appuntamenti avanzate per il Dynamic Chat**: il Dynamic Chat offre più opzioni per il routing degli appuntamenti di destinazione. Specificare gli appuntamenti dell&#39;agente da instradare in base agli attributi di Marketo Engage, garantendo che i lead vengano instradati agli agenti appropriati.

* **Generazione di rapporti per finestre di dialogo avanzate per il Dynamic Chat**: visualizza le prestazioni delle campagne di Dynamic Chat in modo più dettagliato utilizzando visualizzazioni di dati completamente nuove per le metriche di coinvolgimento e conversione.

* **Sincronizza attributi di Marketo Engage non utilizzati per il Dynamic Chat**: annulla la sincronizzazione degli attributi di Marketo Engage della sottoscrizione di Dynamic Chat non utilizzati, per facilitare la pulizia dei dati e consentire la sincronizzazione di attributi alternativi in base alle esigenze.

## Esperienza di nuova generazione

**Nuove visualizzazioni per commutazione**: le visualizzazioni seguenti sono ora disponibili nell&#39;esperienza di nuova generazione:

* [Visualizzazione dettagli e-mail](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [Visualizzazione elenco e-mail](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## Automazione dell’esperienza {#experience-automation}

* **Esclusioni regole di convalida campo modulo globale**: escludi moduli specifici dalle regole di convalida modulo globale in modo che i centri sottoscrizioni e altri flussi di lavoro business critical possano accettare tutti i valori.

* **Passaggi di flusso self-service**: espandi la connettività tra il Marketo Engage e il resto dello stack con la possibilità di creare passaggi di flusso personalizzati da utilizzare nelle campagne avanzate. Sia gli utenti del Marketo Engage che i partner possono sfruttare questa funzionalità per consentire l’utilizzo di servizi web esterni nelle campagne Trigger, Batch ed Eseguibili, a differenza dei webhook, che possono essere utilizzati solo nelle campagne Trigger.

* **Tracciamento collegamenti agnostici del protocollo Munchkin**: estendere il supporto per il tracciamento di `tel` e `mailto` collegamenti con Munchkin per tenere traccia di un set esteso di comportamenti Web.

* **Metodi HTTP aggiuntivi per i webhook**: specificare PUT, PATCH e DELETE come tipi di richiesta per interagire con i servizi Web.

## Insight sulle vendite {#sales-insight}

![(stella)](assets/yellow-star.png)

* **Set di autorizzazioni Sales Insight in Salesforce**: gli amministratori possono fornire l&#39;accesso Sales Insight a un gruppo limitato di persone a livello di utente anziché a livello di profilo tramite il set di autorizzazioni dell&#39;app Marketo, che fa parte del pacchetto Sales Insight Salesforce.

* **Aggiornamento sezioni di My Marketo - Azioni di approfondimento sulle vendite**: gli amministratori di Marketo (e gli utenti da essi designati) possono ora passare rapidamente alla propria istanza di azioni di approfondimento sulle vendite tramite una nuova sezione Azioni di approfondimento sulle vendite disponibile nella pagina My Marketo.

## Sales Connect {#sales-connect}

![(stella)](assets/yellow-star.png)

* **Aggiornamento API Salesforce**: con la versione Salesforce Summer &#39;22, le versioni legacy API 21 -30 non saranno più supportate da Salesforce. Con questa versione di Marketo Engage, tutte le richieste di Sales Connect che utilizzano versioni API legacy sono state aggiornate per rimanere all’interno di una versione supportata. Per informazioni complete sui piani di ritiro delle API Salesforce, fai clic [qui](https://help.salesforce.com/s/articleView?language=en_US&amp;type=1&amp;id=000354473){target="_blank"}.

## Miglioramenti API {#api-enhancements}

* **Nuove funzionalità di filtro per API di estrazione membri programma in blocco**: consente di filtrare in base allo stato di appartenenza al programma, a UpdateAt, alla cadenza o al contenuto esaurito per perfezionare il set di dati estratto.

* **Miglioramento dell&#39;API di estrazione membri programma in blocco**: specificare fino a 10 programmi durante la creazione di processi per migliorare la velocità effettiva.

## Annunci {#announcements}

* **Deprecazione di Forms - Forms 1.0, endpoint di acquisizione/salvataggio lead e versioni senza script dei moduli**: il supporto per le risorse di Forms 1.0 verrà rimosso completamente dal Marketo Engage entro ottobre 2022. Tutte le risorse Forms 1.0 esistenti cesseranno di funzionare. I moduli di Marketo Engage richiederanno il caricamento di JavaScript sulle pagine di destinazione e sui siti web.

**_Webinar sulla versione del prodotto_**

[Webinar sulla versione del Marketo Engage di giugno e agosto 2022](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
