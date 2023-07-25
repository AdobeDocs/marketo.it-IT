---
description: Note sulla versione - Agosto 2021 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Agosto 2021
exl-id: 4aec4e0b-520e-4786-a110-8e68f1bf9950
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# Note sulla versione: agosto 2021 {#release-notes-aug-21}

Le seguenti funzioni sono incluse nella versione di agosto 2021. Verifica la disponibilità delle funzioni nella tua edizione del Marketo Engage.

>[!AVAILABILITY]
>
>Caratteristiche contrassegnate da una stella (![](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Adobe Marketo Engage.

**_Versioni trimestrali_**

Le seguenti funzioni verranno rilasciate il **20 agosto 2021**.

## Automazione dell’esperienza {#experience-automation}

* **Autenticazione utente Marketo Engage tramite identità Adobe**: a breve, i nuovi utenti del Marketo Engage con pacchetti Enterprise verranno integrati utilizzando le credenziali utente di Adobe ID. La migrazione degli attuali utenti al sistema di identità integrato non avverrà fino alla metà del 2022 e non è richiesta alcuna azione fino a nuovo avviso. L’autenticazione utente dell’identità di Adobe consente agli amministratori IT/della sicurezza di gestire più istanze di prodotto di Marketo Engage insieme ad altre soluzioni di Experience Cloud, nonché di configurare il SSO tramite una console comune. Gli amministratori possono gestire in modo semplice gruppi di utenti e adesioni utente in un’unica posizione.

* **Nidificazione campagna eseguibile**: le campagne eseguibili possono ora chiamare anche altre campagne eseguibili, consentendo di nidificarle fino a tre livelli di profondità. Ciò consente un ulteriore consolidamento dei flussi operativi comuni e migliora la gestione intelligente di Campaign.

* **Azione flusso singolo nella pagina Dettagli persona** (Disponibile dal 9 settembre): esegui azioni di flusso come invio di e-mail, modifica il proprietario della persona o qualsiasi altra azione di smart campaign su singole persone dalla pagina dei dettagli della persona utilizzando il menu dell’azione di flusso senza passare alla vista griglia del database.

* **[Esportazione attività personalizzata](/help/marketo/product-docs/administration/marketo-custom-activities/custom-activity-metadata-export.md)**: l’esportazione dei metadati ora supporta tutti gli oggetti e i rispettivi metadati, che possono essere utilizzati per condividere, analizzare e progettare il modello di dati dell’abbonamento.

## Miglioramenti API {#api-enhancements}

* **Invia API modulo**: quando un indirizzo e-mail viene duplicato in due o più record Lead, aggiorna il record &quot;ultimo aggiornamento&quot; invece di saltare del tutto. Fornisce parità con l’API di Forms 2.0.

* **API e-mail**: recupera le risorse e-mail campione o sfidante. Recupera le risorse e-mail utilizzando il filtro dell’intervallo di date.

**_Rilascio nel corso del trimestre_**

Le seguenti funzioni sono in un ciclo non trimestrale e verranno rilasciate nei prossimi mesi.

## Insight sulle vendite {#sales-insight}

![(stella)](assets/yellow-star.png)

* **Maggiore visibilità sulle attività di lead, contatti, account e opportunità per gli utenti CRM Salesforce**: il coinvolgimento con i potenziali clienti durante lunghi cicli di vendita è più informato a causa di un numero maggiore di record di coinvolgimento in Sales Insight. Le schede dei momenti interessanti, dell’attività web, delle e-mail e dei punteggi mostrano fino a 400 attività tra gli oggetti Lead, Contatto, Account e Opportunità.

## Sales Connect {#sales-connect}

![(stella)](assets/yellow-star.png)

* **Limitazione della connessione e-mail (Beta)**: migliora il recapito messaggi e-mail e ridimensiona le comunicazioni di vendita personalizzate con la limitazione della connessione e-mail per Sales Connect. Questa nuova tecnologia gestisce automaticamente la tempistica di invio delle e-mail per creare esperienze ottimizzate per gli utenti di Exchange e Gmail. Diminuisci o elimina l&#39;utilizzo di applicazioni di invio di e-mail in blocco di terze parti e invia tutte le tue e-mail da Sales Connect in tutta sicurezza.

>[!NOTE]
>
>La limitazione delle e-mail è ora disponibile in versione beta. [Ulteriori informazioni](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

* **Approfondimenti attività di vendita migliorate**: acquisisci e attiva un coinvolgimento personalizzato in base alle precedenti attività del team di vendita. Negli elenchi smart del Marketo Engage è possibile utilizzare nuovi attributi quali il collegamento di registrazione delle chiamate di vendita, il nome della campagna di vendita e l’oggetto dell’e-mail di vendita.  Queste attività possono essere esportate e segnalate tramite l’API REST di Marketo Engage o l’esportazione in blocco e sono disponibili su filtri e attivatori come vincoli aggiuntivi per gli elenchi avanzati.

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Integrazione Forms Bizible LinkedIn Lead Gen**: gli addetti al marketing possono ora eseguire l’attribuzione dei ricavi sulle conversioni che si verificano quando LinkedIn acquisisce i moduli compilati tramite le unità pubblicitarie Forms di generazione lead. Queste informazioni possono quindi essere utilizzate per ottimizzare le prestazioni dei moduli e gli investimenti in supporti a pagamento. LinkedIn Lead Gen Forms è una delle soluzioni LinkedIn a pagamento in più rapida crescita e questa nuova funzionalità è inclusa nell&#39;integrazione LinkedIn Ads con Bizible.

* **Dashboard Velocity migliorato**: abbiamo aggiunto una nuova metrica di velocità e un filtro del dashboard per informazioni più approfondite. Questa dashboard viene utilizzata dagli esperti di marketing per comprendere la velocità di lead e opportunità di ogni fase e l’efficienza di diverse forme di coinvolgimento di marketing e vendita.

* **Nuovo dashboard Percorso a cascata per coorte**: questo consente agli esperti di marketing di visualizzare la progressione di una coorte selezionata attraverso un classico insieme di stadi &quot;cascata della domanda&quot;, fornendo una rapida comprensione dei tassi di conversione e della causalità della conversione implicita stadio per stadio.

## Integrazione Bizible con Adobe Experience Cloud {#bizible-integration-with-adobe-experience-cloud}

Questa sezione include nuove funzioni per gli utenti Bizible che hanno completato la migrazione Adobe Identity Management System (IMS). Se hai eseguito la migrazione, il nuovo Adobe ID verrà visualizzato in Impostazioni Bizible nella scheda Adobe ID. Tutti gli account dovrebbero essere migrati entro la fine del 2021.

* **Integrazione Bizible con Adobe Privacy Service** (disponibile a settembre 2021): l’integrazione di Bizible con Adobe Privacy Service centralizza la conformità alle normative sulla privacy dei dati (come il GDPR) nelle applicazioni Adobe Experience Cloud. Ora puoi sfruttare questo servizio e gestire tutte le richieste di accesso a dati personali a livello centrale in modo che le richieste di modifica ricevute da Bizible e da altri prodotti Adobe vengano applicate a tutte le applicazioni.

* **Bizible su interfaccia Adobe Experience Cloud**: l’adozione dell’interfaccia Adobe Experience Cloud da parte di Bizible offre agli utenti nuove funzionalità che verranno visualizzate nella barra dell’intestazione dell’applicazione Bizible e includono un migliore accesso alle risorse di supporto e al cambio di applicazione. L’interfaccia Experience Cloud consente di creare un’esperienza coerente tra Bizible e altre applicazioni Adobe Experience Cloud.

* **Proprietà e gestione autonoma dei domini bizible**: gli utenti Bizible possono sfruttare Adobe Admin Console per gestire i domini che desiderano monitorare. Questa funzione consente di eseguire in autonomia un processo precedentemente manuale e offre un’esperienza coerente nella gestione della proprietà e del tracciamento dei domini nelle applicazioni Adobe Experience Cloud.

## Annunci {#announcements}

* **Aggiornamento delle impostazioni dell&#39;ID universale della sottoscrizione**: per supportare la prossima integrazione di Marketi Engage e Adobe Identity per gli utenti esistenti, tutte le sottoscrizioni di Marketo Engage saranno unificate nell’abilitazione del supporto per gli ID universali. Ulteriori informazioni [si trova qui](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md).

**_Webinar sulla versione del prodotto_**

[Webinar sulla versione del Marketo Engage di agosto 2021](https://engage.marketo.com/August21_Release_Webinar.html)
