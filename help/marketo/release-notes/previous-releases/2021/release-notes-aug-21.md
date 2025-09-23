---
description: Note sulla versione - Agosto 2021 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - agosto 2021
exl-id: 4aec4e0b-520e-4786-a110-8e68f1bf9950
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 1%

---

# Note sulla versione - Agosto 2021 {#release-notes-aug-21}

Le seguenti funzioni sono incluse nella versione di agosto 2021. Verifica la disponibilità delle funzioni nella tua edizione di Marketo Engage.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da un asterisco (![](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Adobe Marketo Engage.

**_Versioni trimestrali_**

Le seguenti funzionalità saranno rilasciate il **20 agosto 2021**.

## Automazione dell’esperienza {#experience-automation}

* **Autenticazione utente di Marketo Engage tramite Adobe Identity**: a breve, i nuovi utenti di Marketo Engage con pacchetti Enterprise verranno integrati utilizzando le credenziali utente di Adobe ID. La migrazione degli attuali utenti al sistema di identità integrato non avverrà fino alla metà del 2022 e non è richiesta alcuna azione fino a nuovo avviso. L’autenticazione utente di Adobe identity consente agli amministratori IT/della sicurezza di gestire più istanze di prodotto Marketo Engage insieme ad altre soluzioni Experience Cloud, nonché di configurare il SSO tramite una console comune. Gli amministratori possono gestire in modo semplice gruppi di utenti e adesioni utente in un’unica posizione.

* **Nidificazione campagna eseguibile**: le campagne eseguibili possono ora chiamare anche altre campagne eseguibili, consentendo di nidificarle fino a tre livelli di profondità. Ciò consente un ulteriore consolidamento dei flussi operativi comuni e migliora la gestione intelligente di Campaign.

* **Singola azione di flusso nella pagina dei dettagli della persona** (disponibile dal 9 settembre): esegui azioni di flusso come l&#39;invio di e-mail, la modifica del proprietario della persona o qualsiasi altra azione di smart campaign su singoli utenti dalla pagina dei dettagli della persona tramite il menu dell&#39;azione di flusso senza passare alla visualizzazione griglia del database.

* **[Esportazione attività personalizzate](/help/marketo/product-docs/administration/marketo-custom-activities/custom-activity-metadata-export.md)**: l&#39;esportazione dei metadati ora supporta tutti gli oggetti e i rispettivi metadati che possono essere utilizzati per condividere, analizzare e progettare il modello di dati della sottoscrizione.

## Miglioramenti API {#api-enhancements}

* **Invia API modulo**: quando un indirizzo e-mail viene duplicato in due o più record Lead, viene aggiornato il record &quot;ultimo aggiornamento&quot; invece di saltare del tutto. Fornisce parità con l’API di Forms 2.0.

* **API e-mail**: recupera le risorse e-mail campione o sfidante. Recupera le risorse e-mail utilizzando il filtro dell’intervallo di date.

**_Rilascio nel corso del trimestre_**

Le seguenti funzioni sono in un ciclo non trimestrale e verranno rilasciate nei prossimi mesi.

## [!DNL Sales Insight] {#sales-insight}

![(stella)](assets/yellow-star.png)

* **Visibilità migliorata delle attività di lead, contatti, account e opportunità per gli utenti di Salesforce CRM**: l&#39;impegno con i potenziali clienti durante lunghi cicli di vendita è più informato a causa di un numero maggiore di record di coinvolgimento in [!DNL Sales Insight]. Le schede dei momenti interessanti, dell’attività web, delle e-mail e dei punteggi mostrano fino a 400 attività tra gli oggetti Lead, Contatto, Account e Opportunità.

## [!DNL Sales Connect] {#sales-connect}

![(stella)](assets/yellow-star.png)

* **Limitazione connessione e-mail (Beta)**: migliora il recapito messaggi e-mail e ridimensiona le comunicazioni di vendita personalizzate con la limitazione della connessione e-mail per Sales Connect. Questa nuova tecnologia gestisce automaticamente i tempi di invio delle e-mail per creare esperienze senza soluzione di continuità per [!DNL Exchange] e gli utenti Gmail. Diminuire o eliminare l&#39;utilizzo delle applicazioni di invio di posta elettronica in blocco di terze parti e inviare tutti i messaggi di posta elettronica da [!DNL Sales Connect] con sicurezza.

>[!NOTE]
>
>La limitazione delle e-mail è ora disponibile in Beta. [Ulteriori informazioni](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

* **Informazioni approfondite sull&#39;attività di vendita**: acquisisci e attiva il coinvolgimento personalizzato in base alle precedenti attività del team di vendita. Negli elenchi avanzati di Marketo Engage è possibile utilizzare nuovi attributi quali il collegamento di registrazione delle chiamate di vendita, il nome della campagna di vendita e l’oggetto dell’e-mail di vendita.  Queste attività possono essere esportate e segnalate tramite l’API REST di Marketo Engage o l’esportazione in blocco e sono disponibili sui filtri e sui trigger come vincoli aggiuntivi per gli elenchi avanzati.

## [!DNL Bizible] {#bizible}

![](assets/yellow-star.png)

* Integrazione di Forms **[!DNL Bizible][!DNL LinkedIn] Lead Gen**: Gli addetti al marketing possono ora eseguire l&#39;attribuzione dei ricavi sulle conversioni che si verificano quando [!DNL LinkedIn] acquisisce i moduli compilati tramite le unità pubblicitarie Forms Lead Gen. Queste informazioni possono quindi essere utilizzate per ottimizzare le prestazioni dei moduli e gli investimenti in supporti a pagamento. [!DNL LinkedIn] Lead Gen Forms è una delle offerte di paid media a più rapida crescita di [!DNL LinkedIn] e questa nuova funzionalità è inclusa nell&#39;integrazione di [!DNL LinkedIn] Ads con [!DNL Bizible].

* **Dashboard Velocity migliorato**: è stata aggiunta una nuova metrica di velocità e un nuovo filtro del dashboard per ottenere informazioni più approfondite. Questa dashboard viene utilizzata dagli esperti di marketing per comprendere la velocità di lead e opportunità di ogni fase e l’efficienza di diverse forme di coinvolgimento di marketing e vendita.

* **Nuovo dashboard del Percorso cascata per coorte**: consente agli addetti al marketing di visualizzare la progressione di una coorte selezionata attraverso un classico insieme di fasi &quot;cascata della domanda&quot;, fornendo una rapida comprensione dei tassi di conversione e della causalità della conversione implicita per ogni fase.

## Integrazione di [!DNL Bizible] con Adobe Experience Cloud {#bizible-integration-with-adobe-experience-cloud}

Questa sezione include nuove funzioni per gli utenti Bizible che hanno completato la migrazione del sistema Adobe Identity Management (IMS). Se sei stato trasferito, il nuovo Adobe ID sarà visibile nelle impostazioni di [!DNL Bizible] nella scheda Adobe ID. Tutti gli account dovrebbero essere migrati entro la fine del 2021.

* Integrazione di **[!DNL Bizible]con Adobe Privacy Service** (disponibile a settembre 2021): l&#39;integrazione di [!DNL Bizible] con Adobe Privacy Service centralizza la conformità alle normative sulla privacy dei dati critici (come il RGPD) nelle applicazioni Adobe Experience Cloud. Ora puoi sfruttare questo servizio e gestire tutte le richieste di accesso a dati personali a livello centrale in modo che le richieste di modifica provenienti da [!DNL Bizible] e altri prodotti Adobe vengano applicate a tutte le applicazioni.

* **[!DNL Bizible]su Adobe Unified Shell**: l&#39;adozione di Adobe Unified Shell da parte di [!DNL Bizible] offre agli utenti nuove funzionalità che verranno visualizzate nella barra dell&#39;intestazione dell&#39;applicazione [!DNL Bizible] e includono un migliore accesso alle risorse di supporto e al passaggio tra le applicazioni. Adobe Unified Shell consente di creare un&#39;esperienza coerente tra [!DNL Bizible] e altre applicazioni Adobe Experience Cloud.

* Proprietà e gestione automatica del dominio **[!DNL Bizible]**: [!DNL Bizible] utenti possono utilizzare Adobe Admin Console per gestire i domini di cui devono tenere traccia [!DNL Bizible]. Questa funzione consente di eseguire in autonomia un processo precedentemente manuale e offre un’esperienza coerente nella gestione della proprietà e del tracciamento dei domini nelle applicazioni Adobe Experience Cloud.

## Annunci {#announcements}

* **Aggiornamento delle impostazioni dell&#39;ID universale della sottoscrizione**: per supportare la prossima integrazione di Marketo Engage e Adobe Identity per gli utenti esistenti, tutte le sottoscrizioni di Marketo Engage saranno unificate nell&#39;abilitazione del supporto dell&#39;ID universale. Ulteriori informazioni [sono disponibili qui](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md).

**_Webinar sulla versione del prodotto_**

[Webinar sulla versione di Marketo Engage di agosto 2021](https://engage.marketo.com/August21_Release_Webinar.html)
