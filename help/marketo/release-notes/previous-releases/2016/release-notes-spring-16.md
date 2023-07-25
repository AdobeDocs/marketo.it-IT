---
unique-page-id: 11370952
description: Note sulla versione - Primavera del 1916 - Documentazione di Marketo - Documentazione del prodotto
title: Note sulla versione - Primavera 2016
exl-id: 0ca26acf-2ac2-418e-bc4e-9820f483fa71
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 0%

---

# Note sulla versione: Primavera del &#39;16 {#release-notes-spring}

Le seguenti funzioni sono incluse nella versione di primavera del 1916. Fai clic sui collegamenti del titolo per visualizzare articoli dettagliati per ciascuna funzione.

## [Email Insights](/help/marketo/product-docs/reporting/email-insights/email-insights-overview.md) {#email-insights}

Email Insights è una nuovissima esperienza di analisi dei dati aggregati e-mail, riprogettata end-to-end per prestazioni incredibilmente veloci come parte di Project Orion. Offre un design dell’interfaccia utente completamente nuovo, ottimizzato per soddisfare le esigenze e il flusso di lavoro degli esperti di e-mail marketing.

>[!NOTE]
>
>A partire dal 3 giugno lanceremo Email Insights per i clienti in batch. Il nostro obiettivo è quello di completarlo nei prossimi mesi. Ti invieremo una notifica via e-mail quando sarai abilitato.

![](assets/two.png)

## [Selettore modello e-mail](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-picker-overview.md) {#email-template-picker}

Crea splendide e-mail utilizzando i nostri nuovi modelli Starter! Inoltre, individua rapidamente i modelli dalle miniature live.

>[!NOTE]
>
>L’editor e-mail 2.0 (con il selettore di modelli) verrà introdotto gradualmente a partire dal 3 giugno. Il rollout verrà completato entro il 30 giugno. A differenza di Email Insights, non riceverai una notifica quando disporrai dell’accesso. Per vedere se è così, segui i passaggi descritti in [questo articolo](/help/marketo/product-docs/email-marketing/general/email-editor-2/transitioning-to-email-editor-2-0.md).

![](assets/5-29-home-starter-templates.png)

## [Modifica delle e-mail: nuova immagine](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-editing-re-imagined}

Esatto, un editor e-mail completamente nuovo! Utilizza la funzionalità di trascinamento della selezione per aggiungere e riordinare i contenuti. I nuovi elementi, tra cui immagini, video, variabili e moduli, migliorano sicuramente l’esperienza di modifica. Consulta anche l’editor di codice aggiornato, il visualizzatore di anteprime e il supporto della preintestazione.

![](assets/17a-29-modules-next.png)

## [Messaggi in-app mobili](/help/marketo/product-docs/mobile-marketing/in-app-messages/understanding-in-app-messages.md) {#mobile-in-app-messages}

Crea straordinari messaggi in-app per la tua app direttamente in Marketo. Definisci esattamente chi deve visualizzarlo e quando con il programma di messaggi in-app. Monitora facilmente le sue prestazioni con la dashboard del programma.

![](assets/pasted-image-at-2016-05-24-09-45-am.png)

## [Nessun frammento bozza](/help/marketo/product-docs/administration/users-and-roles/enable-no-draft-for-snippets.md) {#no-draft-snippets}

Sono finiti i giorni in cui devi riapprovare tutto ogni volta che uno snippet viene aggiornato. Con Nessuna bozza, tutte le e-mail e le pagine di destinazione che utilizzano uno snippet riceveranno gli aggiornamenti dello snippet e manterranno i loro stati precedenti. Ogni volta che approvate uno snippet, potete scegliere se eseguire No-Draft (Nessuna bozza) e aggiornare tutto o creare delle bozze. Sta a te! Nessuna bozza sarà disponibile per tutti i clienti e controllata da una nuova autorizzazione in Amministratore.

![](assets/image2016-5-16-15-3a41-3a17.png)

## [Pagina di destinazione, modello della pagina di destinazione e API modulo](https://developers.marketo.com/blog/spring-2016-updates/) {#landing-page-landing-page-template-and-form-apis}

Le API REST di Marketo ora supportano il controllo sulle pagine di destinazione, i modelli di pagina di destinazione e i moduli di Marketo. Gli utenti possono ora creare, aggiornare il contenuto, approvare ed eliminare queste risorse direttamente tramite l’API REST di Marketo.

## [IP in Inserita nell&#39;elenco Consentiti dell’accesso API](/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md) {#ip-allowlisting-for-api-access}

Analogamente alla funzione di inserire nell&#39;elenco Consentiti dell’IP per gli accessi degli utenti Marketo, ora gli amministratori di Marketo possono impostare un elenco Consentiti di indirizzi IP che possono accedere alle API SOAP e REST di Marketo, bloccando in tal modo l’accesso da indirizzi IP non autorizzati. Questo offre un ulteriore livello di sicurezza all’istanza Marketo e garantisce che l’accesso API sia possibile solo dall’interno della rete dell’organizzazione. I dettagli sulla configurazione sono disponibili sul sito [Sito della documentazione di Marketo](/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md).

## [Nuovo connettore di sincronizzazione per Microsoft Dynamics ad alta velocità](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md) {#new-high-speed-microsoft-dynamics-sync-connector}

Progettato sulla base dell&#39;architettura Orion, il nuovo connettore dinamico ad alta velocità offre velocità fino a 20 volte superiori per la sincronizzazione iniziale e fino a 5 volte superiori per la sincronizzazione incrementale. Tutti i nuovi clienti effettueranno l’onboarding a questo connettore alla data di rilascio e lo distribuiremo gradualmente ai clienti esistenti nel periodo di rilascio estivo.

**Aggiorna dati per nuovi campi**: ora puoi abilitare nuovi campi di sincronizzazione in qualsiasi momento e tutti i valori dei dati per quel campo verranno aggiornati da Dynamics CRM in Marketo. Nessun ulteriore problema sulla necessità di selezionare tutti i campi durante la configurazione iniziale. Se si disattiva un campo di sincronizzazione esistente e lo si riattiva in un secondo momento, tutti i valori dei dati per tale campo verranno aggiornati da Dynamics CRM in Marketo.

**Sincronizza lead come contatto**: l’azione di flusso Sincronizza lead in Microsoft dispone di una nuova opzione per la sincronizzazione come lead o contatto.

![](assets/image2016-5-19-8-3a59-3a9.png)

**Scheda Amministrazione errori di sincronizzazione**: consente di sfogliare, cercare o esportare lead (e altri oggetti) che non sono stati sincronizzati con dettagli quali operazione, direzione, codice di errore e messaggio di errore.

![](assets/sync-errors.png)

**Microsoft Dynamics 2016**: il connettore è completamente certificato per le versioni online e on-premise di Dynamics 2016.

**Gli aggiornamenti dei plug-in sono ora documentati:** Consulta la [articolo della documentazione sugli aggiornamenti dei plug-in](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/marketo-plugin-releases-for-microsoft-dynamics.md).

## [Nome istanza intuitivo](/help/marketo/product-docs/administration/settings/edit-subscription-settings.md) {#friendly-instance-name}

Attualmente è difficile distinguere tra istanze di Marketo, ad esempio istanze sandbox e di produzione. Questa funzione consente di sapere su quali istanze stai lavorando.

![](assets/image2016-5-16-15-3a57-3a14.png)

## [Accesso limitato nel tempo per gli abbonamenti](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md) {#limited-time-access-for-subscriptions}

Oggi, gli utenti sono invitati a iscriversi a Marketo per un periodo di tempo indefinito. Questa funzione consente agli amministratori di invitare gli utenti agli abbonamenti per un periodo di tempo limitato, ad esempio 2 settimane o 1 mese.

![](assets/image2016-5-16-15-3a59-3a52.png)

## [Griglia oggetti personalizzati](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) {#custom-objects-grid}

Ora è possibile visualizzare il numero di record e campi per tutti gli oggetti personalizzati pubblicati.

![](assets/custom-objects-grid.png)

## Attività personalizzate {#custom-activities}

Gli amministratori di Marketo possono ora definire e gestire i propri tipi di attività personalizzati tramite il modellatore di definizione di attività personalizzata di Marketo. Simile (e in combinazione con) a Marketo Custom Object Modeler, ora gli amministratori possono estendere il modello dati in base alle proprie esigenze aziendali specifiche. I dettagli sull’utilizzo di questa funzionalità sono disponibili sul sito [Sito della documentazione di Marketo](/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md).
