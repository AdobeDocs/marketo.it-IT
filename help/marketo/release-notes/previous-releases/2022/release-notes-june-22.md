---
description: Note sulla versione - Giugno 2022 - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione - Giugno 2022
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
source-git-commit: beafa230f067972119f1a0eb170b1339d20d3842
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# Note sulla versione: Giugno 2022 {#release-notes-june-22}

Di seguito sono elencate tutte le funzioni incluse nella versione del 22 giugno. Per informazioni sulla disponibilità delle funzioni, consulta la tua edizione Adobe Marketo Engage .

>[!AVAILABILITY]
>
>Caratteristiche indicate da una stella (![stella](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

Le seguenti funzionalità inizieranno a essere rilasciate il **24 giugno 2022**, con un rollout graduale delle funzioni rimanenti nelle settimane successive (se non specificato diversamente).

## Ambiente dati di marketing {#marketing-data-environment}

* **Esponi campi CreatedAt/UpdatedAt per oggetti personalizzati**: Consente di controllare questi campi nella schermata Dettagli persona per ottenere ulteriori informazioni.

## Orchestrazione tra canali {#cross-channel-orchestration}

* **Miglioramento dell’usabilità di Stream Designer per la chat dinamica**: Aggiungi le schede direttamente dall’area di lavoro di Stream Designer senza dover trascinare. L’interfaccia Dynamic Chat è stata migliorata per offrire una migliore visibilità del contenuto nelle singole schede.

* **Regole avanzate di instradamento degli appuntamenti per chat dinamica**: La chat dinamica offre più opzioni per il routing degli appuntamenti di destinazione. Specifica quali appuntamenti dell&#39;agente devono essere instradati in base agli attributi del Marketo Engage, garantendo che i lead vengano instradati agli agenti appropriati.

* **Reporting avanzato delle finestre di dialogo per la chat dinamica**: Visualizza le prestazioni delle campagne Dynamic Chat in modo più dettagliato utilizzando nuove visualizzazioni di dati per le metriche di coinvolgimento e conversione.

* **Attributi di Marketo Engage non utilizzati non sincronizzati per la chat dinamica**: Annullare la sincronizzazione degli attributi di Marketo Engage dalla sottoscrizione Dynamic Chat che non vengono utilizzati, facilitando la pulizia dei dati e consentendo la sincronizzazione degli attributi alternativi in base alle esigenze.

## Esperienza di nuova generazione

**Nuova visualizzazione alternata**: Le visualizzazioni seguenti sono ora disponibili nell’esperienza di nuova generazione:

* [Visualizzazione dettagli e-mail](/help/marketo/product-docs/marketo-engage-next-generation-experience/toggle-switch.md#email-details-view){target=&quot;_blank&quot;}
* [Visualizzazione a elenco e-mail](/help/marketo/product-docs/marketo-engage-next-generation-experience/toggle-switch.md#email-list-view){target=&quot;_blank&quot;}

## Automazione delle esperienze {#experience-automation}

* **Esclusioni di regole di convalida dei campi modulo globali**: Escludere moduli specifici dalle regole di convalida dei moduli globali in modo che i centri di abbonamento e gli altri flussi di lavoro aziendali critici possano accettare tutti i valori.

* **Passaggi di flusso self-service**: Espandi la connettività tra il Marketo Engage e il resto della pila con la possibilità di creare passaggi di flusso personalizzati da utilizzare in Smart Campaigns. Sia gli utenti che i partner del Marketo Engage possono sfruttare questa funzionalità per consentire l’utilizzo di servizi Web esterni in Trigger, Batch e Campagne eseguibili, a differenza di Webhooks, che può essere utilizzato solo in Campagne trigger.

* **Tracciamento dei collegamenti Agnostico protocollo Munchkin**: Estendi il supporto per il tracciamento `tel` e `mailto` collegamenti con Munchkin per tenere traccia di un set esteso di comportamenti web.

* **Metodi HTTP aggiuntivi per i webhook**: Specifica PUT, PATCH e DELETE come tipi di richiesta per interagire con i servizi web.

## Approfondimenti vendite {#sales-insight}

![(stella)](assets/yellow-star.png)

* **Set di autorizzazioni Insight vendite a Salesforce**: Gli amministratori possono fornire l’accesso a Sales Insight a un set limitato di persone a livello di utente anziché di profilo tramite il set di autorizzazioni Marketo App, che fa parte del pacchetto Salesforce Insight Vendite.

* **Aggiornamento della sezione Marketo personale - Azioni Approfondimenti vendite**: Gli amministratori di Marketo (e gli utenti designati) possono ora passare rapidamente alla propria istanza di azione Approfondimenti vendite tramite una nuova sezione Azioni Approfondimenti vendite che si trova nella pagina Marketo personale.

## Sales Connect {#sales-connect}

![(stella)](assets/yellow-star.png)

* **Aggiornamento API Salesforce**: Con la versione di Salesforce Estate 22, le versioni precedenti dell’API 21-30 non saranno più supportate da Salesforce. Con questa versione di Marketo Engage, tutte le richieste di vendita Connect che utilizzano versioni API legacy sono state aggiornate per rimanere all’interno di una versione supportata. Per informazioni complete sui piani di ritiro dell&#39;API Salesforce, fai clic su [qui](https://help.salesforce.com/s/articleView?language=en_US&amp;type=1&amp;id=000354473){target=&quot;_blank&quot;}.

## Miglioramenti API {#api-enhancements}

* **Nuove funzionalità di filtro per l&#39;API di estrazione dei membri del programma in blocco**: Filtrare per stato di appartenenza al programma, aggiornamento di At, cadenza o contenuto esaurito per perfezionare il set di dati estratti.

* **Miglioramento API dell’estrazione dei membri del programma in blocco**: Specifica fino a 10 programmi durante la creazione di processi per migliorare la velocità effettiva.

## Annunci {#announcements}

* **Forms Deprecation - Forms 1.0, endpoint per l’acquisizione/il salvataggio di lead e versioni non basate su script dei moduli**: Il supporto per le risorse Forms 1.0 verrà rimosso completamente dal Marketo Engage entro ottobre 2022. Tutte le risorse Forms 1.0 esistenti cesseranno di funzionare. I moduli di Marketo Engage richiedono il caricamento di JavaScript su pagine di destinazione e siti web.

**_Webinar sulla versione del prodotto_**

[Webinar sul rilascio del Marketo Engage giugno e agosto 2022](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target=&quot;_blank&quot;}
