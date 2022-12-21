---
unique-page-id: 11370952
description: Note sulla versione - Primavera '16 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Primavera '16
exl-id: 0ca26acf-2ac2-418e-bc4e-9820f483fa71
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 0%

---

# Note sulla versione: Primavera &#39;16 {#release-notes-spring}

Le seguenti funzionalità sono incluse nella versione primaverile del 16. Fai clic sui collegamenti del titolo per visualizzare gli articoli dettagliati per ciascuna funzione.

## [Approfondimenti e-mail](/help/marketo/product-docs/reporting/email-insights/email-insights-overview.md) {#email-insights}

Email Insights è una nuova esperienza storica di analisi e-mail con dati aggregati: riprogettata end-to-end per prestazioni rapide fulminee come parte di Project Orion. Offre un design dell’interfaccia utente completamente nuovo e ottimizzato per soddisfare le esigenze e il flusso di lavoro degli addetti al marketing e-mail.

>[!NOTE]
>
>Stiamo avviando e-mail Insights per i clienti in batch, a partire dal 3 giugno. Il nostro obiettivo è quello di completarlo nei prossimi mesi. Una volta abilitato, riceverai una notifica via e-mail.

![](assets/two.png)

## [Selettore modello e-mail](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-picker-overview.md) {#email-template-picker}

Crea belle e-mail utilizzando i nostri nuovi modelli Starter! Inoltre, individua rapidamente i tuoi modelli dalle miniature live.

>[!NOTE]
>
>L’editor e-mail 2.0 (con il selettore dei modelli) verrà gradualmente introdotto a partire dal 3 giugno. Completeremo il rollout entro il 30 giugno. A differenza di E-mail Insights, non riceverai alcuna notifica quando disponi dell’accesso. Per verificare se lo fai, segui i passaggi descritti in [articolo](/help/marketo/product-docs/email-marketing/general/email-editor-2/transitioning-to-email-editor-2-0.md).

![](assets/5-29-home-starter-templates.png)

## [Modifica delle e-mail: riprogettata](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-editing-re-imagined}

Esatto, un nuovo editor di e-mail! Utilizza una leggera funzionalità di trascinamento per aggiungere e riordinare i contenuti. I nuovi elementi, tra cui immagini, video, variabili e moduli, miglioreranno sicuramente la tua esperienza di modifica. Controlla anche il supporto aggiornato dell&#39;editor di codice, dell&#39;anteprima e della preintestazione.

![](assets/17a-29-modules-next.png)

## [Messaggi in-app mobili](/help/marketo/product-docs/mobile-marketing/in-app-messages/understanding-in-app-messages.md) {#mobile-in-app-messages}

Crea messaggi in-app incredibili per la tua app direttamente in Marketo. Definisci esattamente chi dovrebbe visualizzarlo e quando con il programma di messaggi in-app. Il dashboard del programma consente di monitorare facilmente le prestazioni.

![](assets/pasted-image-at-2016-05-24-09-45-am.png)

## [Nessun frammento di bozza](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/enable-no-draft-for-snippets.md) {#no-draft-snippets}

Sono finiti i giorni in cui devi riapprovare tutto ogni volta che un frammento viene aggiornato! Con No-Draft, tutte le e-mail e le pagine di destinazione che utilizzano uno snippet riceveranno gli aggiornamenti dello snippet e manterranno i loro stati precedenti. Ogni volta che approvi uno snippet, avrai la possibilità di scegliere se eseguire No-Draft e aggiornare tutto oppure creare bozze. Sta a te! Nessun progetto sarà disponibile per tutti i clienti e controllato da una nuova autorizzazione in Amministratore.

![](assets/image2016-5-16-15-3a41-3a17.png)

## [API per pagina di destinazione, modello di pagina di destinazione e modulo](https://developers.marketo.com/blog/spring-2016-updates/) {#landing-page-landing-page-template-and-form-apis}

Le API REST di Marketo ora supportano il controllo sulle pagine di destinazione, sui modelli delle pagine di destinazione e sui moduli di Marketo. Gli utenti possono ora creare, aggiornare il contenuto, approvare ed eliminare queste risorse direttamente tramite l’API REST di Marketo.

## [Inserire nell&#39;elenco Consentiti IP per l’accesso API](/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md) {#ip-allowlisting-for-api-access}

Come per la funzione di  dell’inserire nell&#39;elenco Consentiti IP per gli accessi utente di Marketo, gli amministratori di Marketo possono ora impostare un inserì nell&#39;elenco Consentiti di indirizzi IP che possono accedere alle API SOAP e REST di Marketo, bloccando in tal modo l’accesso dagli indirizzi IP non autorizzati. Questo fornisce un ulteriore livello di sicurezza all’istanza Marketo e assicura che l’accesso API possa avvenire solo dall’interno della rete della tua organizzazione. I dettagli sulla configurazione sono disponibili nella sezione [Sito della documentazione Marketo](/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md).

## [Nuovo connettore Microsoft Dynamics Sync ad alta velocità](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md) {#new-high-speed-microsoft-dynamics-sync-connector}

Costruito con l&#39;architettura Orion, il nuovo connettore ad alta velocità dynamics fornisce velocità fino a 20 volte più veloci per la sincronizzazione iniziale e fino a 5 volte più veloci per la sincronizzazione incrementale. Tutti i nuovi clienti saranno collegati a questo connettore alla data di rilascio e gradualmente lo distribuiremo ai clienti esistenti nell’intervallo di tempo per il rilascio estivo.

**Aggiornare dati per i nuovi campi**: Ora puoi abilitare nuovi campi di sincronizzazione in qualsiasi momento e tutti i valori di dati per quel campo verranno aggiornati da Dynamics CRM in Marketo. Non preoccuparti più di dover selezionare tutti i campi durante la configurazione iniziale. Se disattivi un campo di sincronizzazione esistente e lo riattivi in un secondo momento, tutti i valori dei dati per quel campo verranno aggiornati da Dynamics CRM in Marketo.

**Sincronizza lead come contatto**: L’azione di flusso Sync Lead to Microsoft dispone di una nuova opzione per la sincronizzazione come lead o come contatto.

![](assets/image2016-5-19-8-3a59-3a9.png)

**Scheda Amministrazione errori di sincronizzazione**: Sfoglia, cerca o esporta i lead (e altri oggetti) che non sono stati sincronizzati con dettagli quali funzionamento, direzione, codice di errore e messaggio di errore.

![](assets/sync-errors.png)

**Microsoft Dynamics 2016**: Il connettore è certificato completamente per le versioni online e on-premise di Dynamics 2016.

**Gli aggiornamenti dei plug-in sono ora documentati:** Consulta la sezione [articolo sulla documentazione degli aggiornamenti dei plug-in](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/marketo-plugin-releases-for-microsoft-dynamics.md).

## [Nome istanza descrittivo](/help/marketo/product-docs/administration/settings/edit-subscription-settings.md) {#friendly-instance-name}

Oggi è difficile distinguere tra istanze di Marketo, ad esempio sandbox e istanze di produzione. Questa funzione ti consente di sapere su quali istanze stai lavorando.

![](assets/image2016-5-16-15-3a57-3a14.png)

## [Accesso a tempo limitato per gli abbonamenti](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md) {#limited-time-access-for-subscriptions}

Oggi, gli utenti sono invitati all&#39;abbonamento Marketo per un periodo di tempo indeterminato. Questa funzione consente agli amministratori di invitare gli utenti agli abbonamenti per un periodo di tempo limitato, ad esempio 2 settimane o 1 mese.

![](assets/image2016-5-16-15-3a59-3a52.png)

## [Griglia oggetti personalizzati](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) {#custom-objects-grid}

Ora è possibile visualizzare il numero di record e campi per tutti gli oggetti personalizzati pubblicati.

![](assets/custom-objects-grid.png)

## Attività personalizzate {#custom-activities}

Gli amministratori di Marketo possono ora definire e gestire i tipi di attività personalizzati tramite il modeler di definizione delle attività personalizzate di Marketo. Analogamente a (e in combinazione con) Marketo Custom Object Modeler, gli amministratori possono ora estendere il modello dati in base alle proprie esigenze aziendali. I dettagli sull’utilizzo di questa funzionalità sono disponibili nella sezione [Sito della documentazione Marketo](/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md).
