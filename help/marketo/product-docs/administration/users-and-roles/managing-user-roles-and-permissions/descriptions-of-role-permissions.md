---
unique-page-id: 6848747
description: Descrizioni delle autorizzazioni dei ruoli - Documenti Marketo - Documentazione del prodotto
title: Descrizioni delle autorizzazioni dei ruoli
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '1154'
ht-degree: 0%

---


# Descrizioni delle autorizzazioni dei ruoli {#descriptions-of-role-permissions}

Di seguito è riportato un elenco di tutte le autorizzazioni disponibili che potete assegnare ai vostri ruoli. Le autorizzazioni sono generalmente associate ad aree funzionali specifiche all&#39;interno di Marketo e possono essere utili per controllare le aree e le funzionalità a cui hanno accesso i diversi utenti.

Alcune informazioni aggiuntive sulle autorizzazioni:

* L&#39;autorizzazione &quot;Accesso&quot; consente a un ruolo di visualizzare e a volte modificare tale parte dell&#39;applicazione.
* Affinché un ruolo abbia accesso alle autorizzazioni secondarie (&quot;Create&quot;, &quot;Delete&quot;, ecc.), tale ruolo deve disporre dell&#39;autorizzazione &quot;Access&quot; per quella parte dell&#39;applicazione. Ad esempio, se desiderate dare a un utente l&#39;autorizzazione per la modifica di campagne, deve disporre dell&#39;autorizzazione globale per accedere alle attività di marketing.
* Potete visualizzare azioni o risorse che non disponete dell’autorizzazione a utilizzare. Tuttavia, se tentate di accedervi, compare un messaggio di avviso relativo all’accesso limitato.

## Autorizzazioni disponibili {#available-permissions}

Quando [create o modificate un ruolo](../../../../product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md), potete selezionare le seguenti autorizzazioni per consentire tale ruolo selezionando le caselle appropriate.

![](assets/createnewrole.png)

## Accesso amministratore  {#access-admin}

Visualizza e apporta modifiche alle impostazioni nella sezione Account personale dell&#39;amministratore.

* Accesso alla traccia di audit - Consente agli utenti di accedere sia alla traccia di audit delle risorse che alla traccia di audit dell&#39;amministratore
* Canali di accesso: consente agli utenti di accedere solo per modificare il tag Canale, non altri tag personalizzati
* Limite di comunicazione di accesso: consente agli utenti di abilitare un limite di comunicazione in Amministratore
* Accesso a CRM: consente agli utenti di accedere a CRM, ad esempio Salesforce o Microsoft Dynamics, in Amministratore
* Access [Data.com](http://Data.com) - Fornisce agli utenti l&#39;accesso all&#39;azione di flusso Data.com
* Accedi all’amministratore delle e-mail: offre agli utenti l’amministratore delle e-mail, per modificare le impostazioni predefinite, ad esempio i domini di annullamento della sottoscrizione e del marchio
* Accesso ai partner dell&#39;evento - Consente agli utenti di accedere a LaunchPoint in Admin
* Accesso a Gestione dei campi - Consente agli utenti di accedere a Gestione dei campi in Amministratore
* Accesso al caricamento dei file - Consente agli utenti di caricare immagini e file in Design Studio
* Accesso alle pagine di destinazione - Consente agli utenti di accedere alle pagine di destinazione in Amministratore
* Percorso di accesso: consente agli utenti di accedere a Posizione in Amministratore per impostare la lingua, le impostazioni internazionali, il fuso orario e la valuta predefinite
* Cronologia di accesso: consente agli utenti di accedere alla cronologia di accesso dell&#39;utente nella traccia di controllo
* Impostazioni di accesso: consente agli utenti di accedere alle impostazioni di accesso in Amministratore per le impostazioni Protezione, Limitazioni IP e Rapporto elenco avanzato
* Accesso alle attività personalizzate di Marketo - Consente agli utenti l&#39;accesso alle attività personalizzate di Marketo in Amministratore
* Accesso all&#39;oggetto personalizzato Marketo - Consente agli utenti di accedere agli oggetti personalizzati Marketo in Amministratore
* Accesso Munchkin - Gli utenti GIves hanno accesso a Munchkin in Amministratore, per impostare il codice di tracciamento, il tracciamento delle persone e abilitare la configurazione API
* Access Revenue Cycle Analytics - Fornisce agli utenti l&#39;accesso a Revenue Cycle Analytics in Admin, per impostare Sync Summary and Attribution
* Ruoli di accesso: consente agli utenti di gestire e modificare i ruoli, ma non agli utenti
* Accesso a Sales Insight: consente agli utenti di gestire Sales Insight in Admin, per impostare lo stato, la configurazione API, il punteggio della persona e altre impostazioni
* Accesso single sign-on: consente agli utenti di gestire Single Sign-On in Amministratore, per abilitare SAML e utilizzare le impostazioni SAML e gli URL di pagina di reindirizzamento
* Accesso a Smart Campaign: consente agli utenti di accedere a Smart Campaign in Amministratore, per limitare i limiti alle persone qualificate
* Accesso alle API SOAP - Consentono agli utenti di gestire le API SOAP in Servizi Web in Amministratore
* Tag di accesso - Consente agli utenti di accedere a tutti i tag personalizzati eccetto il tag Canale
* Accesso al petto del tesoro - Consente agli utenti di accedere alle funzioni sperimentali nel petto del tesoro in Amministratore
* Accesso agli utenti - Consente agli utenti di modificare e gestire gli utenti (ma non i ruoli) in Amministratore
* Accesso ai webhooks - Consente agli utenti di accedere ai webhooks in Amministratore, per impostare i dettagli e le mappature delle risposte
* Accesso a aree di lavoro e partizioni: consente agli utenti di creare, modificare ed eliminare aree di lavoro e partizioni in Amministratore

## API Access  {#access-api}

Fornisce agli utenti l&#39;accesso **API Only** **Role** (Solo API) alle singole API elencate di seguito.

* Approva risorse
* Esegui campagna
* Attività in sola lettura
* Metadati attività di sola lettura
* Risorse di sola lettura
* Campagna di sola lettura
* Società di sola lettura
* Oggetto personalizzato di sola lettura
* Persona di sola lettura
* Account con nome di sola lettura
* Opportunità di sola lettura
* Persona di vendita di sola lettura
* Attività di lettura/scrittura
* Metadati attività di lettura/scrittura
* Lettura/scrittura delle risorse
* Campagna di lettura/scrittura
* Società di lettura/scrittura
* Oggetto personalizzato Lettura/scrittura
* Persona di lettura/scrittura
* Account con nome in lettura/scrittura
* Opportunità di lettura/scrittura
* Persona di vendita in lettura/scrittura

Accesso ad Analytics

Consente agli utenti di accedere alle schede Analisi, Approfondimenti e-mail, ai rapporti e ai tre elementi sottostanti, a meno che non siano deselezionati.

* Esplora entrate di Access - L&#39;annullamento della verifica rimuove l&#39;accesso dell&#39;utente a Esplora entrate
* Elimina rapporto: l&#39;annullamento della verifica rimuove la possibilità dell&#39;utente di eliminare i rapporti
* Esporta dati di Analytics - L&#39;annullamento della verifica rimuove la capacità dell&#39;utente di esportare i dati di Analytics

## Accedi ad Presentations calendario {#access-calendar-presentations}

Consente agli utenti di accedere alle presentazioni Calendario ??- consente di visualizzare il pulsante Presentations nella parte inferiore?

* Modifica Presentations calendario - Consente agli utenti di modificare le presentazioni nel calendario

## Access Design Studio {#access-design-studio}

Consente agli utenti di accedere alla scheda Design Studio e alla visualizzazione della struttura, ma non ai dettagli.

* E-mail di accesso

   * Modifica e-mail: consente agli utenti di modificare, creare e duplicare e-mail

      * Rendi e-mail operativa: consente agli utenti di rendere operativa un&#39;e-mail. Vedere: [Impostazione di un&#39;e-mail](../../../../product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)
   * Approva e-mail: consente agli utenti di approvare le e-mail.
   * Elimina e-mail: consente agli utenti di eliminare i messaggi e-mail.
   * Imposta dominio con brand: consente agli utenti di lavorare con i domini di branding. Vedere: [Aggiungi più domini di branding](http://docs.marketo.com/display/docs/add+multiple+branding+domains)


* Modello e-mail di accesso

   * Approva modello e-mail
   * Elimina modello e-mail
   * Modifica modello e-mail - Modifica, creazione e duplicazione di modelli e-mail

* Modulo di accesso

   * Elimina modulo
   * Modifica modulo - Modifica, creazione e duplicazione di moduli

* Immagine di accesso

   * Elimina immagine
   * Carica immagine

* Pagina di destinazione di accesso

   * Approva pagina di destinazione
   * Elimina pagina di destinazione
   * Modifica pagina di destinazione - Modifica, creazione e duplicazione di pagine di destinazione

* Modello pagina di destinazione di accesso

   * Approva modello pagina di destinazione
   * Elimina modello pagina di destinazione
   * Modifica modello pagina di destinazione - Modifica, creazione e duplicazione di modelli di pagina di destinazione

* Snippet di accesso

   * Approva snippet
   * Elimina snippet
   * Modifica snippet

* Accesso all&#39;app Social

   * Approva app social
   * Elimina app social
   * Modifica app social

## Database di Access {#access-database}

Visualizzare il database, nonché visualizzare e modificare gli elenchi smart/statici.

* Segmentazione di accesso

   * Approva segmentazione
   * Elimina segmentazione
   * Modifica segmentazione

* Importazione elenco avanzata
* Elimina persona
* Elimina elenco
* Modifica persona - Impedisce la modifica manuale e l&#39;esecuzione di singoli passaggi di flusso; è ancora possibile modificare le persone eseguendo campagne contro di esse
* Esporta persona - Esporta fogli di calcolo con gli elenchi del database
* Importa oggetto personalizzato
* Importa elenco
* Unisci persone
* Esecuzione di azioni di flusso singolo - Consente agli utenti di eseguire il passaggio **Modifica flusso valore** dati sulle persone provenienti dal database

* Visualizza dati opportunità - Nasconde le informazioni sull&#39;opportunità nella pagina dei dettagli della persona

## Accesso alle attività di marketing {#access-marketing-activities}

Visualizzare la scheda Attività marketing, le campagne e le cartelle delle campagne.

* Accesso a SMS

   * Approva messaggio SMS
   * Elimina messaggio SMS
   * Modifica messaggio SMS

* Notifica push di accesso

   * Approva notifica push
   * Elimina notifica push
   * Modifica notifica push

* Premi di accesso
* Attiva campagna di attivazione
* Approva programma e-mail
* Clona risorsa di marketing
* Elimina risorsa marketing
* Modifica limitazioni campagna
* Modifica risorsa di marketing
* Programma di importazione
* Importa elenco
* Pianificazione campagna batch

Accesso SEO

* Amministrazione SEO
* SEO standard

## Targeting e personalizzazione {#targeting-and-personalization}

* Amministra personalizzazione Web
* CRE Campaign Editor
* Avvio campagna CRE
* Editor campagne Web
* Avvio campagna Web

Amministrazione area di lavoro

* Accesso dell’amministratore a un’area di lavoro specifica (solo se l’area di lavoro è abilitata)
* Spostare le risorse tra le aree di lavoro (solo se le aree di lavoro sono abilitate)

Accesso all&#39;applicazione mobile
