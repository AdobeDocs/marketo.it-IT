---
description: Note sulla versione - Giugno 2022 - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione - Giugno 2022
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Note sulla versione: giugno 2022 {#release-notes-june-22}

Qui sotto troverai tutte le funzioni incluse nella versione di giugno 2022. Verifica la disponibilità delle funzioni nella tua edizione di Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![stella](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

Le seguenti funzionalità inizieranno a essere rilasciate il **24 giugno 2022**, con un rollout graduale delle funzioni rimanenti nelle settimane successive (salvo diversa indicazione).

## Ambiente dati di marketing {#marketing-data-environment}

* **Esporre i campi CreatedAt/UpdatedAt per gli oggetti personalizzati**: consente di esaminare questi campi nella schermata Dettagli persona per ottenere ulteriori insight.

## Orchestrazione cross-channel {#cross-channel-orchestration}

* **Miglioramento dell&#39;usabilità di Stream Designer per[!DNL Dynamic Chat]**: aggiungere schede direttamente dall&#39;area di lavoro Stream Designer senza dover essere trascinate. È stata migliorata anche l&#39;interfaccia [!DNL Dynamic Chat] per offrire una migliore visibilità dei contenuti nelle singole schede.

* **Regole di routing degli appuntamenti avanzate per[!DNL Dynamic Chat]**: [!DNL Dynamic Chat] offre ulteriori opzioni per il routing degli appuntamenti di destinazione. Specifica gli appuntamenti dell&#39;agente da instradare in base agli attributi Marketo Engage, in modo da garantire che i lead vengano instradati agli agenti appropriati.

* **Generazione rapporti di finestre di dialogo avanzate per[!DNL Dynamic Chat]**: visualizza le prestazioni delle campagne [!DNL Dynamic Chat] in modo più dettagliato utilizzando visualizzazioni di dati completamente nuove per le metriche di coinvolgimento e conversione.

* **Annulla sincronizzazione attributi Marketo Engage inutilizzati per[!DNL Dynamic Chat]**: annulla la sincronizzazione degli attributi Marketo Engage dalla sottoscrizione [!DNL Dynamic Chat] che non vengono utilizzati, per facilitare la pulizia dei dati e consentire la sincronizzazione di attributi alternativi in base alle esigenze.

## Esperienza di nuova generazione

**Nuove visualizzazioni per commutazione**: le visualizzazioni seguenti sono ora disponibili nell&#39;esperienza di nuova generazione:

* [Visualizzazione dettagli e-mail](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [Visualizzazione elenco e-mail](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## Automazione dell’esperienza {#experience-automation}

* **Esclusioni regole di convalida campo modulo globale**: escludi moduli specifici dalle regole di convalida modulo globale in modo che i centri sottoscrizioni e altri flussi di lavoro business critical possano accettare tutti i valori.

* **Passaggi di flusso self-service**: espandi la connettività tra Marketo Engage e il resto dello stack con la possibilità di creare passaggi di flusso personalizzati da utilizzare nelle campagne avanzate. Sia gli utenti che i partner di Marketo Engage possono sfruttare questa funzionalità per consentire l’utilizzo di servizi web esterni nelle campagne Trigger, Batch ed Eseguibili, a differenza dei webhook, che possono essere utilizzati solo nelle campagne Trigger.

* **Tracciamento collegamenti agnostici del protocollo di Munchkin**: estendere il supporto per il tracciamento di `tel` e `mailto` collegamenti con Munchkin per tenere traccia di un set esteso di comportamenti Web.

* **Metodi HTTP aggiuntivi per i webhook**: specificare PUT, PATCH e DELETE come tipi di richiesta per interagire con i servizi Web.

## [!DNL Sales Insight] {#sales-insight}

![(stella)](assets/yellow-star.png)

* Set di autorizzazioni **[!DNL Sales Insight]in[!DNL Salesforce]**: gli amministratori possono fornire l&#39;accesso [!DNL Sales Insight] a un gruppo limitato di persone a livello di utente anziché a livello di profilo tramite il set di autorizzazioni dell&#39;app Marketo, che fa parte del pacchetto [!DNL Sales Insight] [!DNL Salesforce].

* **Aggiornamento sezioni di My Marketo - [!DNL Sales Insight] Azioni**: gli amministratori di Marketo (e gli utenti da essi designati) possono ora passare rapidamente alla propria istanza di [!DNL Sales Insight] azioni tramite una nuova sezione di [!DNL Sales Insight] azioni che si trova nella pagina My Marketo.

## [!DNL Sales Connect] {#sales-connect}

![(stella)](assets/yellow-star.png)

* Aggiornamento API **[!DNL Salesforce]**: con la versione estiva &#39;22 di [!DNL Salesforce], le versioni legacy API 21 -30 non saranno più supportate da [!DNL Salesforce]. Con questa versione di Marketo Engage, tutte le richieste [!DNL Sales Connect] che utilizzano versioni API legacy sono state aggiornate per rimanere all&#39;interno di una versione supportata. Per informazioni complete sui piani di ritiro API [!DNL Salesforce], fare clic [qui](https://help.salesforce.com/s/articleView?language=en_US&type=1&id=000354473){target="_blank"}.

## Miglioramenti API {#api-enhancements}

* **Nuove funzionalità di filtro per API di estrazione membri programma in blocco**: consente di filtrare in base allo stato di appartenenza al programma, a UpdateAt, alla cadenza o al contenuto esaurito per perfezionare il set di dati estratto.

* **Miglioramento dell&#39;API di estrazione membri programma in blocco**: specificare fino a 10 programmi durante la creazione di processi per migliorare la velocità effettiva.

## Annunci {#announcements}

* **Deprecazione di Forms - Forms 1.0, endpoint di acquisizione/salvataggio lead e versioni senza script dei moduli**: il supporto per le risorse di Forms 1.0 verrà rimosso completamente da Marketo Engage entro ottobre 2022. Tutte le risorse Forms 1.0 esistenti cesseranno di funzionare. Marketo Engage forms richiederà il caricamento di JavaScript su pagine di destinazione e siti Web.

**_Webinar sulla versione del prodotto_**

[Webinar sulla versione di Marketo Engage di giugno e agosto 2022](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
