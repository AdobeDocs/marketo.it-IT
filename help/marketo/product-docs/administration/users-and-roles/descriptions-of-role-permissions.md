---
unique-page-id: 6848747
description: Descrizioni delle autorizzazioni per il ruolo - Documentazione di Marketo - Documentazione del prodotto
title: Descrizioni delle autorizzazioni per il ruolo
exl-id: 00963cd9-2d53-455f-bc6f-42a573468ff9
feature: Users and Roles
source-git-commit: c79de5b87d75c26aeec5f8d39252dc303dabeac8
workflow-type: tm+mt
source-wordcount: '1448'
ht-degree: 0%

---

# Descrizioni delle autorizzazioni per il ruolo {#descriptions-of-role-permissions}

Di seguito è riportato un elenco di tutte le autorizzazioni disponibili che puoi assegnare ai tuoi ruoli. Le autorizzazioni sono generalmente associate ad aree funzionali specifiche all’interno di Marketo e possono aiutarti a controllare le aree e le funzionalità a cui i diversi utenti hanno accesso.

Alcune informazioni aggiuntive sulle autorizzazioni:

* L&#39;autorizzazione di accesso consente a un ruolo di visualizzare e talvolta modificare tale parte dell&#39;applicazione.
* Affinché un ruolo possa accedere alle autorizzazioni secondarie (&quot;Crea&quot;, &quot;Elimina&quot;, ecc.), deve disporre dell&#39;autorizzazione &quot;Accesso&quot; per quella parte dell&#39;applicazione. Ad esempio, se desideri concedere a un utente l’autorizzazione Modifica campagne, deve disporre dell’autorizzazione complessiva per accedere alle attività di marketing.
* Potresti essere in grado di visualizzare azioni o risorse per le quali non disponi delle autorizzazioni necessarie. Tuttavia, se tenti di accedervi, visualizzerai un messaggio di avviso relativo all’accesso limitato.

## Autorizzazioni disponibili {#available-permissions}

Quando [crei o modifichi un ruolo](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md), puoi selezionare quale delle seguenti autorizzazioni consentire per quel ruolo selezionando le caselle appropriate.

![](assets/descriptions-of-role-permissions-1.png)

## Accedi ad Admin  {#access-admin}

Visualizza e modifica le impostazioni nella sezione Account personale dell’amministratore.

* Accedere ad Adobe Connect: consente agli utenti di accedere alla schermata Adobe Connect
* Accedi a Adobe Experience Manager&#42; - Consente agli utenti di accedere alla schermata Adobe Experience Manager
* Accedi a Mapping organizzazione Adobe&#42; - Consente agli utenti di accedere alla schermata Mapping organizzazione Adobe
* Accesso Admin Audit Trail&#42; - Consente agli utenti di accedere alla schermata Admin Audit Trail
* Accesso alla prova di verifica dell&#39;accesso&#42; - Consente agli utenti di accedere alla prova di verifica dell&#39;accesso
* Accedi a Audit Trail: consente agli utenti di accedere sia ad Asset Audit Trail che ad Admin Audit Trail
* Accedere a CAPTCHA: accedere alla schermata CAPTCHA
* Accesso ai canali: consente agli utenti di accedere solo per modificare il tag Canale, non altri tag personalizzati
* Limite di comunicazione di accesso: consente agli utenti di abilitare un limite di comunicazione in Admin
* Accesso al CRM - Consente agli utenti di accedere al CRM, ad esempio [!DNL Salesforce] o [!DNL Microsoft Dynamics], in Admin
* Accesso [[!DNL Data.com]](https://data.com) - Consente agli utenti di accedere all&#39;azione di flusso Data.com
* Accedi a Amministrazione e-mail: consente agli utenti di accedere a Amministrazione e-mail per modificare le impostazioni predefinite, ad esempio i domini di annullamento dell’abbonamento e di branding
* Accesso ai partner eventi: consente agli utenti di accedere a LaunchPoint in Admin
* Accedere a Condivisione pubblico di Experience Cloud: consente agli utenti di sincronizzare un pubblico da Adobe Experience Cloud al Marketo Engage
* Accesso alla gestione dei campi: consente agli utenti di accedere alla gestione dei campi in Admin
* Caricamento file di accesso: consente agli utenti di caricare immagini e file in Design Studio
* Accedere alle pagine di destinazione: consente agli utenti di accedere alle pagine di destinazione in Admin
* Posizione di accesso: consente agli utenti di accedere alla posizione in Amministratore per impostare lingua, lingua, fuso orario e valuta predefiniti
* Cronologia accesso - Consente agli utenti di accedere alla Cronologia accesso utente in Audit Trail
* Impostazioni di accesso - Consente agli utenti di accedere alle impostazioni di accesso in Amministratore per sicurezza, restrizioni IP e impostazioni dei rapporti degli elenchi avanzati
* Accedi alla nuova esperienza&#42; - Consente agli utenti di accedere alla schermata Nuova esperienza
* Accedi all’attività personalizzata di Marketo: consente agli utenti di accedere alle attività personalizzate di Marketo in Amministratore
* Accedi a oggetto personalizzato Marketo: consente agli utenti di accedere a oggetti personalizzati Marketo in Amministrazione
* Accesso a [!DNL Munchkin]: gli utenti GIves accedono a [!DNL Munchkin] in Admin per impostare il codice di tracciamento, il tracciamento delle persone e abilitare la configurazione API
* Accedi a Predictive Audiences&#42; - Consente agli utenti di accedere alla schermata Predictive Audiences
* Accedere ad Analytics per il ciclo dei ricavi: consente agli utenti di accedere ad Analytics per il ciclo dei ricavi in Admin, per impostare Riepilogo sincronizzazione e Attribuzione
* Ruoli di accesso: consente agli utenti di gestire e modificare i ruoli, ma non gli utenti
* Accedi a Sales Insight: consente agli utenti di gestire Sales Insight in Admin (Amministrazione) per impostare lo stato, la configurazione API, il punteggio persona e altre impostazioni
* Accesso Single Sign-on: consente agli utenti di gestire il Single Sign-On in Admin, per abilitare SAML e lavorare con le impostazioni SAML e gli URL di pagina di reindirizzamento
* Accedi a Smart Campaign: consente agli utenti di accedere a Smart Campaign in Admin, per limitare i limiti alle persone qualificate
* Accesso all’API SOAP: consente agli utenti di gestire le API SOAP nei servizi web in Admin
* Accedi ai tag: consente agli utenti di accedere a tutti i tag personalizzati eccetto il tag Canale
* Accedi a Treasure Chest: consente agli utenti di accedere alle funzioni sperimentali di Treasure Chest in Admin
* Accesso agli utenti: consente agli utenti di modificare e gestire gli utenti (ma non i ruoli) in Amministratore
* Accedi ai webhook: consente agli utenti di accedere ai webhook in Admin, per impostare dettagli e mappature di risposta
* Accesso alle aree di lavoro e alle partizioni: consente agli utenti di creare, modificare ed eliminare aree di lavoro e partizioni in Admin

_&#42;Per evitare interruzioni per gli utenti esistenti, questa autorizzazione viene introdotta in modalità passiva ed è visibile ma non accessibile in questo momento. Comunicheremo come implementarlo quando diventerà attivo a metà del 2024._

## API di accesso  {#access-api}

Consente agli utenti con **Solo API** **Ruolo** di accedere alle singole API elencate di seguito.

* Approva Assets
* Esegui campagna
* Attività di sola lettura
* Metadati attività di sola lettura
* Assets di sola lettura
* Campagna di sola lettura
* Società di sola lettura
* Oggetto personalizzato di sola lettura
* Persona di sola lettura
* Account denominato di sola lettura
* Opportunità di sola lettura
* Venditore di sola lettura
* Attività di lettura/scrittura
* Metadati attività di lettura/scrittura
* Assets di lettura/scrittura
* Campagna di lettura/scrittura
* Società di lettura/scrittura
* Oggetto personalizzato di lettura/scrittura
* Persona di lettura/scrittura
* Account denominato di lettura-scrittura
* Opportunità di lettura/scrittura
* Persona di vendita di lettura/scrittura

## Accedere ad Analytics {#access-analytics}

Consente agli utenti di accedere alle schede di Analytics, a Informazioni e-mail, ai rapporti e ai tre elementi seguenti, a meno che non siano deselezionati.

* Accesso a Gestione ricavi: l&#39;annullamento della selezione comporta la rimozione dell&#39;accesso dell&#39;utente a Gestione ricavi
* Crea report&#42; - Consente agli utenti di creare, clonare, leggere, aggiornare e spostare le risorse report in Analytics e nelle attività di marketing, nonché le risorse Modeler del ciclo dei ricavi
* Elimina rapporto: se si deseleziona, viene rimossa la possibilità dell’utente di eliminare rapporti
* Esporta dati di Analytics: se si deseleziona, viene rimossa la possibilità dell’utente di esportare dati di Analytics

_&#42;Per evitare interruzioni per gli utenti esistenti, questa autorizzazione viene introdotta in modalità passiva ed è visibile ma non accessibile in questo momento. Comunicheremo come implementarlo quando diventerà attivo a metà del 2024._

## Accedi a Calendar Presentations {#access-calendar-presentations}

Consente agli utenti di accedere alle presentazioni del Calendario: consente la visualizzazione del pulsante Presentations nella parte inferiore.

* Modifica calendario Presentations: consente agli utenti di modificare le presentazioni nel calendario

## Accedere a Design Studio {#access-design-studio}

Consente agli utenti di accedere alla scheda Design Studio e alla visualizzazione della struttura, ma non ai dettagli.

* Accedi all’e-mail
   * Modifica e-mail: consente agli utenti di modificare, creare e clonare le e-mail
      * Rendi operativa l’e-mail: consente agli utenti di rendere operativa un’e-mail. Vedere: [Rendere operativa un&#39;e-mail](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)

      * Approva e-mail: consente agli utenti di approvare le e-mail.
      * Elimina e-mail: consente agli utenti di eliminare le e-mail.
      * Imposta dominio con marchio: consente agli utenti di lavorare con i domini di branding. Vedere: [Aggiungi un dominio di branding aggiuntivo](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/add-an-additional-branding-domain.md)

* Accedi al modello di e-mail

   * Approva modello e-mail
   * Elimina modello e-mail
   * Modifica modello e-mail: modifica, crea e clona modelli e-mail

* Modulo di accesso

   * Approva modulo
   * Elimina modulo
   * Modifica modulo: modificare, creare e clonare moduli

* Accedi a immagine

   * Elimina immagine
   * Carica immagine

* Accedi alla pagina di destinazione

   * Approva pagina di destinazione
   * Elimina pagina di destinazione
   * Modifica pagina di destinazione: modifica, crea e clona le pagine di destinazione

* Accedi al modello della pagina di destinazione

   * Approva modello pagina di destinazione
   * Elimina modello pagina di destinazione
   * Modifica modello pagina di destinazione: modifica, crea e clona modelli di pagina di destinazione

* Snippet di accesso

   * Approva snippet
   * Elimina snippet
   * Modifica snippet

* Accedi all’app social

   * Approva app social
   * Elimina app social
   * Modifica app social

## Database di Access {#access-database}

Visualizzare il database e visualizzare e modificare gli elenchi smart/static.

* Segmentazione degli accessi

   * Approva segmentazione
   * Elimina segmentazione
   * Modifica segmentazione

* Elimina persona
* Crea elenco&#42;
   * Accesso per creare una risorsa elenco nelle attività di database e marketing
   * Accesso per creare una risorsa di elenco avanzato in attività di database e marketing
* Elimina elenco
* Modifica persona: impedisce la modifica manuale e l’esecuzione di passaggi a flusso singolo; è comunque possibile modificare le persone eseguendo campagne su di esse
* Esporta persona - Esporta fogli di calcolo con dagli elenchi del database
* Importa oggetto personalizzato
* Importa elenco
* Unisci persone
* Esegui azioni a flusso singolo: consente agli utenti di eseguire il passaggio di flusso **Modifica valore dati** sulle persone dal database

* Visualizza dati opportunità: nasconde le informazioni sull’opportunità nella pagina dei dettagli della persona.

_&#42;Per evitare interruzioni per gli utenti esistenti, questa autorizzazione viene introdotta in modalità passiva ed è visibile ma non accessibile in questo momento. Comunicheremo come implementarlo quando diventerà attivo a metà del 2024._

## Accedere alle attività di marketing {#access-marketing-activities}

Visualizza la scheda Attività di marketing, le campagne e le cartelle delle campagne.

* Accedi al messaggio SMS

   * Approva messaggio SMS
   * Elimina messaggio SMS
   * Modifica messaggio SMS

* Accedi alle notifiche push

   * Approva notifica push
   * Elimina notifica push
   * Modifica notifica push

* Riconoscimenti accesso
* Attiva campagna trigger
* Approva programma e-mail
* Clona risorsa di marketing
* Elimina risorsa di marketing
* Modifica restrizioni campagna
* Modifica risorsa marketing
* Esporta attività campagna&#42;
* Importa programma
* Importazione elenco
* Pianifica campagna batch

Accedere a SEO

* Amministrare SEO
* SEO standard

_&#42;Per evitare interruzioni per gli utenti esistenti, questa autorizzazione viene introdotta in modalità passiva ed è visibile ma non accessibile in questo momento. Comunicheremo come implementarlo quando diventerà attivo a metà del 2024._

## Targeting e Personalization {#targeting-and-personalization}

* Amministrare Web Personalization
* Editor campagna CRE
* Modulo di avvio campagna CRE
* Editor campagna web
* Modulo di avvio campagna web

Amministrazione Workspace

* Accesso amministratore per un Workspace specifico (solo se sono state abilitate le aree di lavoro)
* Spostare le risorse tra le aree di lavoro (solo se sono state abilitate le aree di lavoro)
