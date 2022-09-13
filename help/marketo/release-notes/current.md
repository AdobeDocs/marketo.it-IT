---
description: Note sulla versione corrente - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione corrente
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: d26428137e9b99d04fef67a3b21b74d150f693e7
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# Note sulla versione: Ottobre 2022 {#release-notes-oct-22}

Di seguito sono elencate tutte le funzioni incluse nella versione del 22 ottobre. Per informazioni sulla disponibilità delle funzioni, consulta la tua edizione Adobe Marketo Engage .

>[!AVAILABILITY]
>
>Caratteristiche indicate da una stella (![stella](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

Le seguenti funzionalità inizieranno a essere rilasciate il **14 ottobre 2022**, con un rollout graduale delle funzioni rimanenti nelle settimane successive (se non specificato diversamente). Le funzioni di rilascio e le date esatte sono soggette a modifiche.

## Orchestrazione tra canali {#cross-channel-orchestration}

* **Flusso di dialogo di disposizione automatica per chat dinamica**: Migliora la tua area di dialogo affollata organizzando tutto sulla tela in un formato pulito e facile da leggere con la pressione di un pulsante attraverso Auto Arrange.

* **Supporta tipi di dati aggiuntivi per la chat dinamica**: Tre nuovi tipi di dati (booleano, intero, mobile) ti consentono di sfruttare più campi di Marketo Engage esistenti nella chat dinamica per elementi come il targeting basato su punteggi o fare ai visitatori domande sì/no.

* **Collegamenti riunione per chat dinamiche**: Opzione per includere automaticamente un collegamento Team o Meeting per Google e Outlook in ogni invito del calendario inviato ai visitatori.

* **Notifiche di riunione pianificate per chat dinamica**: I rappresentanti di vendita ricevono notifiche e-mail automatizzate relative alle riunioni programmate e a qualsiasi informazione pertinente sull&#39;interazione del chatbot del visitatore.

* **Ruoli e autorizzazioni per la chat dinamica**: Gli amministratori possono utilizzare autorizzazioni granulari per controllare la visibilità e l’utilizzo dell’applicazione e creare ruoli utente personalizzati.

   * Accesso completo: gli utenti possono sfruttare appieno la funzione (ad esempio, finestre di dialogo di pubblicazione, schema di colori di modifica, ecc.)
   * Accesso in sola lettura : gli utenti possono visualizzare le informazioni ma non possono apportare modifiche (ad esempio, consulta Criteri di pubblico o Progettazione flussi, ma non modificare)
   * Accesso limitato: gli utenti non possono visualizzare o accedere alle sezioni Configurazione o Integrazioni

## Esperienza di nuova generazione {#next-generation-experience}

* **Schermi aggiornati nell’esperienza di nuova generazione**: Nell’esperienza di nuova generazione, offriamo schermi aggiuntivi e aggiornati che offrono un design aggiornato e miglioramenti all’usabilità accessibili tramite interruttore:

   * Dettagli modello pagina di destinazione
   * Elenco modelli e-mail

* **Miglioramento utilizzato dalla scheda nei dettagli del modello e-mail**: Nella nuova esperienza, vedrai ulteriori informazioni sulle risorse utilizzando il modello e-mail, tra cui Stato risorsa, Ultima modifica e Ultima modifica di. Puoi anche eseguire ricerche, ordinare e filtrare l’elenco delle risorse utilizzate.

* **Riporta moduli filtro risorse**: Nuova progettazione per i modelli di configurazione dei rapporti che visualizzano una nuova struttura delle risorse nel menu di configurazione e un filtro per Data di creazione e modifica.

## Ambiente dati di marketing {#marketing-data-environment}

* **Integrazione di Adobe Privacy Service**: Armonizza con Privacy Service per automatizzare la conformità alle normative sulla privacy dei dati tra i prodotti Experience Cloud. Al momento, questo servizio è disponibile solo per i clienti del Marketo Engage che hanno effettuato l’accesso al [Adobe Identity Management](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md)Sistema {target=&quot;_blank&quot;}.

* **Sincronizzazione campi personalizzati membri del programma**: Possibilità di sincronizzare bidirezionalmente i campi estensibili acquisiti per un membro del programma (ad esempio, preferenze dei partecipanti durante la registrazione dell&#39;evento come cibo, sessioni, tracce, ecc.)

## Miglioramenti API {#api-enhancements}

* **Importazione in serie di lead: Associazione dei venditori**: Parità con l’API REST lead per poter associare i lead ai venditori durante il processo di importazione in serie per lead, riducendo la complessità e il numero di chiamate API richieste.

## Annunci {#announcements}

* **Forms 1.0**: La versione 1.0 di Forms diventerà obsoleta con la versione di ottobre. Le risorse Forms 1.0 non saranno più in grado di inviare dati al Marketo Engage e restituiranno errori se tentati.

* **Forms senza script**: Forms non funzionerà più quando JavaScript è disabilitato nel browser. Per l’invio del modulo è necessario abilitare Javascript.
