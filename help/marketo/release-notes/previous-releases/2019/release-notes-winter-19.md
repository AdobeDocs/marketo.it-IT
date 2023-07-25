---
unique-page-id: 17727823
description: Note sulla versione -Inverno '19 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Inverno '19
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 0%

---

# Note sulla versione: inverno 2019 {#release-notes-winter}

Le seguenti funzioni sono incluse nella versione di inverno 19. Verifica la disponibilità delle funzioni nella tua edizione di Marketo.

Fai clic sui collegamenti del titolo per visualizzare articoli dettagliati per ciascuna funzione, se disponibile.

>[!NOTE]
>
>Facebook ora richiede un account Business Manager per sfruttare l’integrazione con il pubblico personalizzato. Il servizio Facebook LaunchPoint *deve* essere associato a un account di Business Manager oppure **la tua integrazione non funzionerà più dopo il 14 gennaio 2019**. Per impostare un account di Business Manager, fare riferimento a [Guida di facebook](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>Microsoft sta spingendo tutti i clienti online all’aggiornamento alla versione più recente di Microsoft Dynamics. Se stai integrando la tua istanza di Marketo con Dynamics Online, dovrai [aggiornamento alla versione più recente della soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md) prima di **31 gennaio 2019** affinché la tua integrazione continui a funzionare.

>[!NOTE]
>
>Marketo sta aggiornando la versione OAuth per GoToWebinar da 1.0 a 2.0. Il supporto per OAuth 1.0 verrà rimosso a gennaio 2019. Se sei un cliente GoToWebinar, dovrai autenticare nuovamente i tuoi accessi tramite LaunchPoint (nell’area Amministratore) tramite **31 gennaio 2019** affinché la tua integrazione continui a funzionare. Per ulteriori informazioni, consulta la [Pagina community](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## Miglioramenti della piattaforma core {#core-platform-enhancements}

**[E-mail CC per e-mail Marketo](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Includi fino a cinque indirizzi CC per destinatario nelle e-mail inviate tramite Marketo.

**API**

* **Supporto di domini multi-branding per Asset API:** L’approvazione e la clonazione delle risorse produce gli stessi risultati nell’API e nell’interfaccia utente di.
* **Supporto di Email CC per Asset API**: gli utenti che clonano, approvano ed elaborano le e-mail tramite l’API manterranno la parità con le impostazioni dell’interfaccia utente.

**[Munchkin v155 (versione beta)](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **Modalità solo API**: gli utenti possono ora determinare quando e come tracciare i membri del proprio database consentendo alle app web a pagina singola di chiamare esplicitamente quando desiderano registrare una visita di pagina web invece di affidarsi al tracciamento automatico di Marketo.
* **Gestione degli opt-out**: gestisci facilmente le rinunce facendo corrispondere il dominio del cookie di rinuncia con il dominio del cookie di tracciamento Munchkin.
* **Parametro Decider A Livello Di Dominio**: domini a due lettere (ad esempio &quot; [website.io](https://website.io)&quot;) si tiene traccia automaticamente in Marketo senza ulteriori requisiti di configurazione.

## Marketo Sales Engage {#marketo-sales-engage}

* **Profilo personalizzato Salesforce**: Sales Engage ora supporta profili personalizzati illimitati.

* **Personalizzazione Salesforce**: rimuovendo i campi di attività personalizzati non critici, gli utenti possono impostare il coinvolgimento nelle vendite nella piattaforma di gestione delle relazioni con i clienti in modo più efficiente.
* **Servizio e-mail**: maggiore recapito messaggi, migliore tracciamento delle risposte, funzionalità e-mail pianificate e funzionalità e-mail in blocco grazie alla connessione a Microsoft Outlook (tramite Office365 o On-Prem tramite la scheda Connessione e-mail).
* **Nuove impostazioni amministratore**: sono state aggiunte due pagine di amministrazione per ottimizzare l’istanza Sales Engage

   * _Gestione team_ supporta un processo di configurazione dell’account semplice, consentendo agli amministratori di modificare gli abbonamenti e i team.
   * _Impostazioni di amministrazione Salesforce_ consente ai team di configurare la sincronizzazione SFDC in modo più rapido e semplice che mai.

* **Plug-in OWA per Windows**: con un singolo componente aggiuntivo, tutti i client Windows Office365 saranno supportati in Sales Engage, che consente di utilizzare feed live in Outlook. Il nuovo plug-in sarà disponibile in Microsoft Store.
* **Spintore attività**: sincronizza il coinvolgimento nelle vendite con la piattaforma Marketo di base per sfruttare le informazioni di marketing in tempo reale.

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>Le versioni di Marketo Sky si verificano con una frequenza più frequente. Le seguenti funzioni e miglioramenti dovrebbero essere rilasciati tra la fine del quarto trimestre e l’inizio del primo trimestre. Per ulteriori dettagli e aggiornamenti, consulta [Documentazione di Sky](https://help.marketo.com/).

* **Esperienza predefinita facoltativa**: gli utenti di Marketo possono impostare Marketo Sky come esperienza predefinita se dispongono dell’accesso di un amministratore.

* **Il mio Marketo è stato riprogettato**: personalizza la tua esperienza aggiungendo widget che forniscano informazioni critiche, notifiche e collegamenti alle aree più visitate.

* **Visualizzazioni elenco e pagine dettagli di Design Studio**: scopri un livello maggiore di organizzazione e precisione con visualizzazioni di elenchi di e-mail, pagine di destinazione e moduli filtrabili e ricercabili. Le pagine dei dettagli delle risorse forniscono informazioni chiave su ciascuna risorsa, tra cui i programmi da cui è utilizzata, il numero di snippet utilizzati e altro ancora.

* **Ricerca globale**: Marketo ora offre una funzione di ricerca globale più veloce e affidabile su tutta la piattaforma. Le query di ricerca ora vengono eseguite in tutte le aree di lavoro accessibili e possono eseguire ricerche in risorse (sia attive che archiviate), etichette, campagne e programmi. I risultati della ricerca vengono forniti tramite una sovrapposizione e ogni risultato include il percorso del file per specificare dove si trova la risorsa.

* **Interfaccia utente migliorata**: nuove icone, modali e pulsanti, oltre a una nuova palette di colori che rispecchia l’aggiornamento del marchio e rende Marketo Sky ancora più sorprendente e funzionale.

* **Miglioramenti all’usabilità del programma e-mail**: continuiamo a migliorare la parità nelle funzionalità del programma e-mail tra la nostra piattaforma classica di gestione dei lead di Marketo e la nuova esperienza di Marketo Sky.
* **Programmi Event-With-Webinar**: i programmi Event-With-Webinar sono ora disponibili in Marketo Sky (nota: in questa versione sarà supportato solo GoToWebinar, con ulteriori integrazioni stabilite nel tempo).

## Account-Based Marketing {#account-based-marketing}

**[Segmentazione e filtro basati su Persona ABM](/help/marketo/product-docs/target-account-management/using-personas.md)**

Personalizza le campagne ABM per utenti tipo specifici all’interno di account denominati. La funzione Persona ABM crea una qualifica professionale predefinita basata sulla segmentazione dei lead e consente di configurare segmentazioni utente aggiuntive.

## Analytics {#analytics}

**Bizible**

* **Campi calcolati personalizzati**: utilizza qualsiasi attributo Bizible per creare campi personalizzati che possono essere utilizzati per la generazione di rapporti e segmentazioni del dashboard.

* **Certificazione SOC II di tipo II**: la nuova certificazione di sicurezza e privacy si basa sull’accreditamento di tipo I dell’inizio di quest’anno.

## Personalizzazione web {#web-personalization}

**[Aggiungere sottodomini nelle impostazioni account](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

Per gestire in modo più efficiente domini e sottodomini, gli utenti possono ora aggiungere sottodomini alle impostazioni del proprio account RTP.

## Marketo Mobile Engagement (MME) {#marketo-mobile-engagement-mme}

**Software Development Kit (SDK) MME aggiornato per Android**

Abbiamo aggiornato l’SDK per Android a un framework più moderno, stabile e scalabile che contiene maggiore flessibilità e nuove funzioni ingegneristiche. Google Gli sviluppatori di app Android ora possono utilizzare direttamente i [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) (FCM) con questo nuovo SDK.

* [Istruzioni per gli sviluppatori](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [Domande frequenti per sviluppatori](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>Sviluppatori di app **deve** aggiornamento alla nuova versione prima del 31 marzo 2019. Se non aggiorni l’SDK entro il 31 marzo 2019, qualsiasi nuovo utente che scarichi l’app dopo tale data non potrà ricevere notifiche push fino all’aggiornamento alla versione più recente dell’SDK. L&#39;aggiornamento dell&#39;SDK non richiederà che gli utenti attuali dell&#39;app mobile scarichino nuovamente una nuova versione dell&#39;app.

## Aggiornamenti aggiuntivi {#additional-updates}

**Piattaforma di webinar estensibile**

Oltre al rilascio del prodotto, il team dei partner sta lavorando a un nuovo framework che consente ai fornitori di webinar di creare e mantenere le proprie integrazioni con Marketo, fornendo maggiore flessibilità nell’aggiornamento e nel miglioramento delle soluzioni e consentendo agli addetti al marketing di ottenere il massimo dalle integrazioni scelte.

Prevediamo di implementare la nuova piattaforma con i provider caso per caso. Per ulteriori informazioni, consulta la [dettagli del programma](https://www.marketo.com/why-marketo/partners/technology/) o contatta il tuo contatto Marketo.
