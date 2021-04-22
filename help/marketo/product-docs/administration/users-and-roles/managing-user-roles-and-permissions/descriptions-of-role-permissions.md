---
unique-page-id: 6848747
description: Descrizioni delle autorizzazioni del ruolo - Documenti Marketo - Documentazione del prodotto
title: Descrizioni delle autorizzazioni del ruolo
exl-id: 00963cd9-2d53-455f-bc6f-42a573468ff9
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '1144'
ht-degree: 0%

---

# Descrizioni delle autorizzazioni del ruolo {#descriptions-of-role-permissions}

Di seguito è riportato un elenco di tutte le autorizzazioni disponibili che puoi assegnare ai tuoi ruoli. Le autorizzazioni sono generalmente associate ad aree funzionali specifiche all’interno di Marketo e possono essere utili per controllare le aree e le funzionalità a cui hanno accesso diversi utenti.

Alcune informazioni aggiuntive sulle autorizzazioni:

* L&#39;autorizzazione &quot;Accesso&quot; fornisce un ruolo di autorizzazione per visualizzare e talvolta modificare tale parte dell&#39;applicazione.
* Affinché un ruolo abbia accesso alle sottoautorizzazioni (&quot;Crea&quot;, &quot;Elimina&quot;, ecc.), tale ruolo deve disporre dell’autorizzazione &quot;Accesso&quot; per quella parte dell’applicazione. Ad esempio, se desideri concedere a un utente l’autorizzazione Modifica campagna, deve disporre dell’autorizzazione complessiva per accedere alle attività di marketing.
* Puoi visualizzare azioni o risorse che non disponi dell’autorizzazione a utilizzare. Tuttavia, se tenti di accedervi, visualizzerai un messaggio di avviso sull’accesso limitato.

## Autorizzazioni disponibili {#available-permissions}

Quando [crei o modifichi un ruolo](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md), puoi selezionare le seguenti autorizzazioni per consentire tale ruolo selezionando le caselle appropriate.

![](assets/createnewrole.png)

## Amministratore di accesso {#access-admin}

Visualizza e apporta modifiche alle impostazioni nella sezione Account personale di Admin.

* Accesso a Audit Trail - Consente agli utenti di accedere sia a Asset Audit Trail che ad Admin Audit Trail
* Canali di accesso : consente agli utenti di accedere solo per modificare il tag Canale, non altri tag personalizzati
* Limite di comunicazione di accesso : consente agli utenti di abilitare un limite di comunicazione in Amministratore
* Accesso a CRM - Consente agli utenti di accedere al CRM, ad esempio Salesforce o Microsoft Dynamics, in Admin
* Accesso [Data.com](https://Data.com) - Consente agli utenti di accedere all&#39;azione di flusso Data.com
* Accedi all’amministratore e-mail : consente agli utenti di modificare le impostazioni predefinite, ad esempio i domini di annullamento della sottoscrizione e di branding
* Accedere ai partner evento : consente agli utenti di accedere a LaunchPoint in Admin
* Accesso alla gestione dei campi : consente agli utenti di accedere alla gestione dei campi in Amministratore
* Accesso al caricamento dei file : consente agli utenti di caricare immagini e file in Design Studio.
* Accesso alle pagine di destinazione : consente agli utenti di accedere alle pagine di destinazione in Admin
* Percorso di accesso : consente agli utenti di accedere alla posizione in Amministratore per impostare la lingua, le impostazioni internazionali, il fuso orario e la valuta predefiniti
* Cronologia accesso - Consente agli utenti di accedere alla cronologia degli accessi utente in Audit Trail
* Impostazioni di accesso : consente agli utenti di accedere alle impostazioni di accesso in Amministratore per le impostazioni di sicurezza, restrizioni IP e rapporti con elenchi avanzati
* Accesso ad attività personalizzate Marketo : consente agli utenti di accedere alle attività personalizzate Marketo in Admin
* Accesso a oggetti personalizzati Marketo : consente agli utenti di accedere agli oggetti personalizzati Marketo in Admin
* Access Munchkin - Gli utenti GI possono accedere a Munchkin in Admin per impostare il codice di tracciamento, il tracciamento delle persone e abilitare la configurazione API
* Accedi ad Analisi del ciclo dei ricavi : consente agli utenti di accedere ad Analisi del ciclo dei ricavi in Amministratore, per impostare Sintetico e Attribuzione
* Accesso ai ruoli : consente agli utenti di gestire e modificare i ruoli, ma non gli utenti
* Accedi a Insight vendite : consente agli utenti di gestire Insight vendite in Admin, per impostare lo stato, la configurazione API, il punteggio persona e altre impostazioni
* Accesso single sign-on : consente agli utenti di gestire il Single Sign-on in Admin, per abilitare SAML e lavorare con le impostazioni SAML e gli URL delle pagine di reindirizzamento
* Accesso a Smart Campaign : consente agli utenti di accedere a Smart Campaign in Admin, per limitare i limiti alle persone qualificate
* Accesso all’API SOAP : consente agli utenti di gestire le API SOAP nei servizi Web in Admin
* Accesso ai tag : consente agli utenti di accedere a tutti i tag personalizzati, ad eccezione del tag Canale
* Accedere al torace del tesoro - Consente agli utenti di accedere alle funzioni sperimentali nel torace del tesoro in Amministratore
* Accesso agli utenti : consente agli utenti di modificare e gestire gli utenti (ma non i ruoli) in Admin
* Accedere ai webhook - Consente agli utenti di accedere ai webhook in Amministratore per impostare dettagli e mappature di risposta
* Accesso a aree di lavoro e partizioni : consente agli utenti di creare, modificare ed eliminare aree di lavoro e partizioni in Admin

## API di accesso {#access-api}

Consente agli utenti con l&#39;accesso **Solo API** **Ruolo** alle singole API elencate di seguito.

* Approvare le risorse
* Esegui campagna
* Attività di sola lettura
* Metadati delle attività di sola lettura
* Risorse di sola lettura
* Campagna di sola lettura
* Società di sola lettura
* Oggetto personalizzato di sola lettura
* Persona di sola lettura
* Account con nome di sola lettura
* Opportunità di sola lettura
* Persona di vendita di sola lettura
* Attività di lettura-scrittura
* Metadati attività di lettura-scrittura
* Risorse di lettura-scrittura
* Campagna di lettura e scrittura
* Società di lettura-scrittura
* Oggetto personalizzato di lettura-scrittura
* Persona di lettura-scrittura
* Account con nome in lettura e scrittura
* Opportunità di lettura-scrittura
* Persona di vendita in lettura/scrittura

## Accedere ad Analytics {#access-analytics}

Consente agli utenti di accedere alle schede Analytics, a Approfondimenti e-mail, ai rapporti e ai tre elementi seguenti, a meno che non siano deselezionati.

* Access Revenue Explorer - Deselezionare questa opzione per rimuovere l&#39;accesso dell&#39;utente a Revenue Explorer
* Elimina rapporto : se si deseleziona, l’utente non potrà più eliminare i rapporti
* Esportare i dati di Analytics - Deselezionare l’opzione per rimuovere la possibilità dell’utente di esportare i dati di Analytics

## Accedi a Presentations calendario {#access-calendar-presentations}

Consente agli utenti di accedere alle presentazioni Calendario - consente la visualizzazione del pulsante Presentations in basso.

* Modifica Presentations calendario - Consente agli utenti di modificare le presentazioni nel Calendario

## Accesso a Design Studio {#access-design-studio}

Consente agli utenti di accedere alla scheda e alla visualizzazione della struttura di Design Studio, ma non ai dettagli.

* Accesso a e-mail
   * Modifica e-mail : consente agli utenti di modificare, creare e duplicare le e-mail
      * Rendi l’e-mail operativa : consente agli utenti di rendere operativa un’e-mail. Vedi: [Rendere un&#39;e-mail operativa](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)

      * Approva e-mail : consente agli utenti di approvare le e-mail.
      * Elimina e-mail : consente agli utenti di eliminare le e-mail.
      * Imposta dominio con marchio : consente agli utenti di lavorare con i domini di branding. Vedi: [Aggiungi un dominio di branding aggiuntivo](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/add-an-additional-branding-domain.md)

* Modello e-mail di accesso

   * Approva modello e-mail
   * Elimina modello e-mail
   * Modificare un modello e-mail: modificare, creare e duplicare modelli e-mail

* Modulo di accesso

   * Elimina modulo
   * Modifica modulo - Modifica, creazione e duplicazione di moduli

* Accedere all&#39;immagine

   * Elimina immagine
   * Carica immagine

* Accedi alla pagina di destinazione

   * Approva pagina di destinazione
   * Elimina pagina di destinazione
   * Modifica pagina di destinazione: modificare, creare e duplicare pagine di destinazione

* Access Landing Page Template

   * Approva modello di pagina di destinazione
   * Elimina modello pagina di destinazione
   * Modificare un modello per pagina di destinazione : modificare, creare e clonare modelli di pagina di destinazione

* Frammento di accesso

   * Approva snippet
   * Elimina frammento
   * Modifica frammento

* Accesso all&#39;app social

   * Approva app social
   * Elimina app social
   * Modifica app social

## Database di accesso {#access-database}

Visualizzare il database, nonché visualizzare e modificare gli elenchi smart/statici.

* Segmentazione dell’accesso

   * Approva segmentazione
   * Elimina segmentazione
   * Modifica segmentazione

* Importazione avanzata elenco
* Elimina persona
* Elimina elenco
* Modifica persona : evita la modifica manuale ed esegui passaggi a flusso singolo; è comunque possibile modificare le persone mediante campagne
* Esporta persona - Esporta fogli di calcolo con gli elenchi del database
* Importa oggetto personalizzato
* Importa elenco
* Unisci persone
* Esegui azioni a flusso singolo : consente agli utenti di eseguire il passaggio di flusso **Modifica valore dati** sulle persone provenienti dal database

* Visualizza dati opportunità : nasconde le informazioni sulle opportunità nella pagina dei dettagli della persona

## Accedere alle attività di marketing {#access-marketing-activities}

Visualizza la scheda Marketing Activities (Attività di marketing), le campagne e le cartelle delle campagne.

* Accedere al messaggio SMS

   * Approva messaggio SMS
   * Elimina messaggio SMS
   * Modifica messaggio SMS

* Accesso alle notifiche push

   * Approva notifica push
   * Elimina notifica push
   * Modifica notifica push

* Accessi
* Attiva campagna di attivazione
* Approva programma e-mail
* Clona risorsa di marketing
* Elimina risorsa di marketing
* Modificare le restrizioni delle campagne
* Modifica risorsa di marketing
* Programma di importazione
* Importazione elenco
* Pianificazione campagna batch

Accesso SEO

* Amministrare SEO
* SEO standard

## Targeting e personalizzazione {#targeting-and-personalization}

* Amministrare la personalizzazione web
* Editor CRE Campaign
* Avvio di CRE Campaign
* Editor web Campaign
* Avvio campagna web

Amministrazione di Workspace

* Accesso dell’amministratore per un’area di lavoro specifica (solo se l’opzione Aree di lavoro è abilitata)
* Spostare le risorse tra le aree di lavoro (solo se le aree di lavoro sono abilitate)
