---
unique-page-id: 17727823
description: Note sulla versione -Inverno '19 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Inverno '19
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '1050'
ht-degree: 0%

---

# Note sulla versione: inverno 2019 {#release-notes-winter}

Le seguenti funzioni sono incluse nella versione di inverno 19. Verifica la disponibilità delle funzioni nella tua edizione di Marketo.

Fai clic sui collegamenti del titolo per visualizzare articoli dettagliati per ciascuna funzione, se disponibile.

>[!NOTE]
>
>[!DNL Facebook] ora richiede un account Business Manager per sfruttare l&#39;integrazione con il pubblico personalizzato. Il servizio [!DNL Facebook] LaunchPoint *deve* essere associato a un account di Business Manager oppure **la tua integrazione non funzionerà più dopo il 14 gennaio 2019**. Per configurare un account di Business Manager, consultare la [[!DNL Facebook] Guida](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>Microsoft sta spingendo tutti i clienti online all&#39;aggiornamento alla versione più recente di [!DNL Microsoft Dynamics]. Se stai integrando la tua istanza di Marketo con [!DNL Dynamics Online], dovrai [eseguire l&#39;aggiornamento alla versione più recente della soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md) prima del **31 gennaio 2019** per garantire che l&#39;integrazione continui a funzionare.

>[!NOTE]
>
>Marketo sta aggiornando la versione OAuth per GoToWebinar da 1.0 a 2.0. Il supporto per OAuth 1.0 verrà rimosso a gennaio 2019. Se sei un cliente GoToWebinar, dovrai autenticare nuovamente i tuoi accessi tramite LaunchPoint (nell&#39;area di amministrazione) entro il **31 gennaio 2019** per garantire che la tua integrazione continui a funzionare. Per ulteriori dettagli, consulta la nostra [pagina della community](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## Miglioramenti della piattaforma core {#core-platform-enhancements}

**[Invia e-mail a CC per e-mail Marketo](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Includi fino a cinque indirizzi CC per destinatario nelle e-mail inviate tramite Marketo.

**API**

* **Supporto di domini multi-branding per API risorse:** L&#39;approvazione e la clonazione delle risorse produce gli stessi risultati nell&#39;API e nell&#39;interfaccia utente.
* **Supporto di Email CC per Asset API**: gli utenti che clonano, approvano ed elaborano e-mail tramite l&#39;API manterranno la parità con le impostazioni dell&#39;interfaccia utente.

**[[!DNL Munchkin] v155 (Beta)](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **Modalità solo API**: gli utenti possono ora determinare quando e come tracciare i membri del proprio database consentendo alle app Web a pagina singola di chiamare esplicitamente quando desiderano registrare una visita a una pagina Web invece di affidarsi al tracciamento automatico di Marketo.
* **Gestione rinuncia**: gestisci facilmente le rinunce facendo corrispondere il dominio dei cookie di rinuncia con il dominio dei cookie di tracciamento [!DNL Munchkin].
* **Parametro Decider a livello di dominio**: i domini a due lettere ([website.io](https://website.io)&quot;) verranno tracciati automaticamente in Marketo senza requisiti di configurazione aggiuntivi.

## Marketo Sales Engage {#marketo-sales-engage}

* Profilo personalizzato **[!DNL Salesforce]**: Sales Engage ora supporta profili personalizzati illimitati.

* Personalizzazione **[!DNL Salesforce]**: rimuovendo i campi di attività personalizzati non critici, gli utenti possono configurare il coinvolgimento nelle vendite nella piattaforma CRM in modo più efficiente.
* **Servizio e-mail**: migliore recapito messaggi, migliore tracciamento delle risposte, funzionalità e-mail pianificate e funzionalità e-mail in blocco tramite la connessione a [!DNL Microsoft Outlook] (tramite Office365 o On-Prem tramite la scheda Connessione e-mail).
* **Nuove impostazioni amministratore**: sono state aggiunte due pagine amministratore per ottimizzare l&#39;istanza Sales Engage

   * _Gestione team_ supporta un processo di configurazione dell&#39;account semplice consentendo agli amministratori di modificare abbonamenti e team.
   * _Impostazioni amministratore Salesforce_ consente ai team di configurare la sincronizzazione SFDC in modo più rapido e semplice che mai.

* **Plug-in OWA per[!DNL Windows]**: con un solo componente aggiuntivo, tutti i client [!DNL Windows Office365] saranno supportati in Sales Engage, consentendo l&#39;utilizzo di feed dinamici in Outlook. Il nuovo plug-in sarà disponibile in Microsoft Store.
* **Spintore attività**: sincronizza il coinvolgimento delle vendite con la piattaforma principale di Marketo per sfruttare le informazioni di marketing in tempo reale.

## [!DNL Marketo Sky] {#marketo-sky}

>[!NOTE]
>
>[!DNL Marketo Sky] versioni si verificano con una frequenza maggiore. Le seguenti funzioni e miglioramenti dovrebbero essere rilasciati tra la fine del quarto trimestre e l’inizio del primo trimestre. Per ulteriori dettagli e aggiornamenti, consulta la [documentazione di Sky](https://help.marketo.com/).

* **Esperienza predefinita opzionale**: gli utenti di Marketo possono impostare [!DNL Marketo Sky] come esperienza predefinita se un amministratore gli ha fornito l&#39;accesso.

* **Il mio Marketo** è stato riprogettato: è possibile personalizzare l&#39;esperienza aggiungendo widget che forniscono informazioni critiche, notifiche e collegamenti alle aree visitate più di frequente.

* **Visualizzazioni elenco e pagine dettagli di Design Studio**: maggiore organizzazione e precisione con visualizzazioni elenco di e-mail, pagine di destinazione e moduli filtrabili e ricercabili. Le pagine dei dettagli delle risorse forniscono informazioni chiave su ciascuna risorsa, tra cui i programmi da cui è utilizzata, il numero di snippet utilizzati e altro ancora.

* **Ricerca globale**: Marketo offre ora una funzione di ricerca globale più veloce e affidabile in tutta la piattaforma. Le query di ricerca ora vengono eseguite in tutte le aree di lavoro accessibili e possono eseguire ricerche in risorse (sia attive che archiviate), etichette, campagne e programmi. I risultati della ricerca vengono forniti tramite una sovrapposizione e ogni risultato include il percorso del file per specificare dove si trova la risorsa.

* **Interfaccia utente migliorata**: nuove icone, modali e pulsanti insieme a una nuova palette di colori per riflettere l&#39;aggiornamento del marchio e rendere [!DNL Marketo Sky] ancora più sorprendente e funzionale.

* **Miglioramenti dell&#39;usabilità del programma e-mail**: continuiamo a muoverci verso la parità nelle funzionalità del programma e-mail tra la nostra piattaforma classica di gestione dei lead di Marketo e la nuova esperienza [!DNL Marketo Sky].
* **Programmi Event-With-Webinar**: i programmi Event-With-Webinar sono ora disponibili in [!DNL Marketo Sky] (nota: in questa versione sarà supportato solo GoToWebinar, con ulteriori integrazioni stabilite nel tempo).

## Account-Based Marketing {#account-based-marketing}

**[Segmentazione e filtro basati su Persona ABM](/help/marketo/product-docs/target-account-management/using-personas.md)**

Personalizza le campagne ABM per utenti tipo specifici all’interno di account denominati. La funzione Persona ABM crea una qualifica professionale predefinita basata sulla segmentazione dei lead e consente di configurare segmentazioni utente aggiuntive.

## Analytics {#analytics}

**[!DNL Bizible]**

* **Campi calcolati personalizzati**: utilizzare qualsiasi attributo [!DNL Bizible] per creare campi personalizzati che possono essere utilizzati per la generazione di rapporti e segmentazioni del dashboard.

* **Certificazione SOC II di tipo II**: la nuova certificazione di sicurezza e privacy si basa sull&#39;accreditamento di tipo I dell&#39;inizio di quest&#39;anno.

## [!DNL Web Personalization] {#web-personalization}

**[Aggiungi sottodomini nelle impostazioni account](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

Per gestire in modo più efficiente domini e sottodomini, gli utenti possono ora aggiungere sottodomini alle impostazioni del proprio account RTP.

## Marketo Mobile Engagement (MME) {#marketo-mobile-engagement-mme}

**Software Development Kit (SDK) MME aggiornato per Android**

Abbiamo aggiornato SDK per Android a un framework più moderno, stabile e scalabile che contiene maggiore flessibilità e nuove funzioni di progettazione. Gli sviluppatori di app Android ora possono utilizzare direttamente [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) (FCM) di Google con questo nuovo SDK.

* [Istruzioni per gli sviluppatori](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [Domande frequenti per sviluppatori](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>Gli sviluppatori di app **devono** eseguire l&#39;aggiornamento alla nuova versione prima del 31 marzo 2019. Se non aggiorni il tuo SDK entro il 31 marzo 2019, qualsiasi nuovo utente che scarica la tua app dopo tale data non potrà ricevere notifiche push fino all’aggiornamento alla versione più recente di SDK. Per eseguire l&#39;aggiornamento di SDK non è necessario che gli utenti dell&#39;app mobile esistente scarichino nuovamente una nuova versione dell&#39;app.

## Aggiornamenti aggiuntivi {#additional-updates}

**Piattaforma di webinar estensibile**

Oltre al rilascio del prodotto, il team dei partner sta lavorando a un nuovo framework che consente ai fornitori di webinar di creare e mantenere le proprie integrazioni con Marketo, fornendo maggiore flessibilità nell’aggiornamento e nel miglioramento delle soluzioni e consentendo agli addetti al marketing di ottenere il massimo dalle integrazioni scelte.

Prevediamo di implementare la nuova piattaforma con i provider caso per caso. Per ulteriori informazioni, consulta i [dettagli del programma](https://www.marketo.com/why-marketo/partners/technology/) o rivolgiti al tuo contatto Marketo.
