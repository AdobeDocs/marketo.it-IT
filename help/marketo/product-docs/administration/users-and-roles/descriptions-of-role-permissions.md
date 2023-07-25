---
unique-page-id: 6848747
description: Descrizioni delle autorizzazioni per il ruolo - Documentazione di Marketo - Documentazione del prodotto
title: Descrizioni delle autorizzazioni per il ruolo
exl-id: 00963cd9-2d53-455f-bc6f-42a573468ff9
feature: Users and Roles
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '1137'
ht-degree: 0%

---

# Descrizioni delle autorizzazioni per il ruolo {#descriptions-of-role-permissions}

Di seguito è riportato un elenco di tutte le autorizzazioni disponibili che puoi assegnare ai tuoi ruoli. Le autorizzazioni sono generalmente associate ad aree funzionali specifiche all’interno di Marketo e possono aiutarti a controllare le aree e le funzionalità a cui i diversi utenti hanno accesso.

Alcune informazioni aggiuntive sulle autorizzazioni:

* L&#39;autorizzazione di accesso consente a un ruolo di visualizzare e talvolta modificare tale parte dell&#39;applicazione.
* Affinché un ruolo possa accedere alle autorizzazioni secondarie (&quot;Crea&quot;, &quot;Elimina&quot;, ecc.), deve disporre dell&#39;autorizzazione &quot;Accesso&quot; per quella parte dell&#39;applicazione. Ad esempio, se desideri concedere a un utente l’autorizzazione Modifica campagne, deve disporre dell’autorizzazione complessiva per accedere alle attività di marketing.
* Potresti essere in grado di visualizzare azioni o risorse per le quali non disponi delle autorizzazioni necessarie. Tuttavia, se tenti di accedervi, visualizzerai un messaggio di avviso relativo all’accesso limitato.

## Autorizzazioni disponibili {#available-permissions}

Quando [creare o modificare un ruolo](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md), è possibile selezionare una delle seguenti autorizzazioni per consentire tale ruolo selezionando le caselle appropriate.

![](assets/descriptions-of-role-permissions-1.png)

## Accedi ad Admin  {#access-admin}

Visualizza e modifica le impostazioni nella sezione Account personale dell’amministratore.

* Accedi a Audit Trail: consente agli utenti di accedere sia ad Asset Audit Trail che ad Admin Audit Trail
* Accesso ai canali: consente agli utenti di accedere solo per modificare il tag Canale, non altri tag personalizzati
* Limite di comunicazione di accesso: consente agli utenti di abilitare un limite di comunicazione in Admin
* Accesso al CRM: consente agli utenti di accedere al CRM, ad esempio [!DNL Salesforce] o [!DNL Microsoft Dynamics], in Admin
* Accesso [[!DNL Data.com]](https://Data.com) - Consente agli utenti di accedere all’azione di flusso Data.com
* Accedi ad Amministrazione e-mail: consente agli utenti di accedere ad Amministratore e-mail per modificare le impostazioni predefinite, ad esempio i domini di annullamento dell’abbonamento e di branding
* Accesso ai partner eventi: consente agli utenti di accedere a LaunchPoint in Admin
* Accesso alla gestione dei campi: consente agli utenti di accedere alla gestione dei campi in Admin
* Caricamento file di accesso: consente agli utenti di caricare immagini e file in Design Studio
* Accedere alle pagine di destinazione: consente agli utenti di accedere alle pagine di destinazione in Admin
* Posizione di accesso: consente agli utenti di accedere alla posizione in Amministratore per impostare lingua, lingua, fuso orario e valuta predefiniti
* Cronologia accesso - Consente agli utenti di accedere alla Cronologia accesso utente in Audit Trail
* Impostazioni di accesso - Consente agli utenti di accedere alle impostazioni di accesso in Amministratore per sicurezza, restrizioni IP e impostazioni dei rapporti degli elenchi avanzati
* Accedi all’attività personalizzata di Marketo: consente agli utenti di accedere alle attività personalizzate di Marketo in Amministratore
* Accedi a oggetto personalizzato Marketo: consente agli utenti di accedere a oggetti personalizzati Marketo in Amministrazione
* Accesso [!DNL Munchkin] - Accesso degli utenti di GIves a [!DNL Munchkin] in Admin, per impostare il codice di tracciamento, il tracciamento delle persone e abilitare la configurazione API
* Accedere ad Analytics per il ciclo dei ricavi: consente agli utenti di accedere ad Analytics per il ciclo dei ricavi in Admin, per impostare Riepilogo sincronizzazione e Attribuzione
* Ruoli di accesso: consente agli utenti di gestire e modificare i ruoli, ma non gli utenti
* Accedi a Sales Insight: consente agli utenti di gestire Sales Insight in Admin (Amministrazione) per impostare lo stato, la configurazione API, il punteggio persona e altre impostazioni
* Accesso Single Sign-on: consente agli utenti di gestire il Single Sign-On in Admin, per abilitare SAML e lavorare con le impostazioni SAML e gli URL di pagina di reindirizzamento
* Accedi a Smart Campaign: consente agli utenti di accedere a Smart Campaign in Admin, per limitare i limiti alle persone qualificate
* Accedere alle API SOAP: consente agli utenti di gestire le API SOAP nei servizi web in Admin
* Accedi ai tag: consente agli utenti di accedere a tutti i tag personalizzati eccetto il tag Canale
* Accedi a Treasure Chest: consente agli utenti di accedere alle funzioni sperimentali di Treasure Chest in Admin
* Accesso agli utenti: consente agli utenti di modificare e gestire gli utenti (ma non i ruoli) in Amministratore
* Accedi ai webhook: consente agli utenti di accedere ai webhook in Admin, per impostare dettagli e mappature di risposta
* Accesso alle aree di lavoro e alle partizioni: consente agli utenti di creare, modificare ed eliminare aree di lavoro e partizioni in Admin

## API di accesso  {#access-api}

Offre agli utenti le **Solo API** **Ruolo** accedere alle singole API elencate di seguito.

* Approva risorse
* Esegui campagna
* Attività di sola lettura
* Metadati attività di sola lettura
* Risorse di sola lettura
* Campagna di sola lettura
* Società di sola lettura
* Oggetto personalizzato di sola lettura
* Persona di sola lettura
* Account denominato di sola lettura
* Opportunità di sola lettura
* Venditore di sola lettura
* Attività di lettura/scrittura
* Metadati attività di lettura/scrittura
* Risorse di lettura/scrittura
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
* Elimina rapporto: se si deseleziona, viene rimossa la possibilità dell’utente di eliminare rapporti
* Esporta dati di Analytics: se si deseleziona, viene rimossa la possibilità dell’utente di esportare dati di Analytics

## Accedi a Calendar Presentations {#access-calendar-presentations}

Consente agli utenti di accedere alle presentazioni del Calendario: consente la visualizzazione del pulsante Presentations nella parte inferiore.

* Modifica calendario Presentations: consente agli utenti di modificare le presentazioni nel calendario

## Accedere a Design Studio {#access-design-studio}

Consente agli utenti di accedere alla scheda Design Studio e alla visualizzazione della struttura, ma non ai dettagli.

* Accedi all’e-mail
   * Modifica e-mail: consente agli utenti di modificare, creare e clonare le e-mail
      * Rendi operativa l’e-mail: consente agli utenti di rendere operativa un’e-mail. Consulta: [Rendere operativa un’e-mail](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)

      * Approva e-mail: consente agli utenti di approvare le e-mail.
      * Elimina e-mail: consente agli utenti di eliminare le e-mail.
      * Imposta dominio con marchio: consente agli utenti di lavorare con i domini di branding. Consulta: [Aggiungi un dominio di branding aggiuntivo](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/add-an-additional-branding-domain.md)

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
* Elimina elenco
* Modifica persona: impedisce la modifica manuale e l’esecuzione di passaggi a flusso singolo; è comunque possibile modificare le persone eseguendo campagne su di esse
* Esporta persona - Esporta fogli di calcolo con dagli elenchi del database
* Importa oggetto personalizzato
* Importa elenco
* Unisci persone
* Eseguire azioni a flusso singolo: consente agli utenti di eseguire **Modifica valore dati** passaggio di flusso sulle persone dal database

* Visualizza dati opportunità: nasconde le informazioni sull’opportunità nella pagina dei dettagli della persona.

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
* Importa programma
* Importazione elenco
* Pianifica campagna batch

Accedere a SEO

* Amministrare SEO
* SEO standard

## Targeting e personalizzazione {#targeting-and-personalization}

* Amministrare la personalizzazione web
* Editor campagna CRE
* Modulo di avvio campagna CRE
* Editor campagna web
* Modulo di avvio campagna web

Amministrazione di Workspace

* Accesso amministratore per un’area di lavoro specifica (solo se sono state abilitate aree di lavoro)
* Spostare le risorse tra le aree di lavoro (solo se sono state abilitate le aree di lavoro)
