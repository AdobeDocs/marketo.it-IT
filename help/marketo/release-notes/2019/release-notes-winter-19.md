---
unique-page-id: 17727823
description: Note sulla versione -Winter '19 - Marketo Docs - Documentazione prodotto
title: Note sulla versione - Inverno '19
translation-type: tm+mt
source-git-commit: b33f5ed707a1377daad51191cc6dd9f093138258
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 0%

---


# Note sulla versione: Inverno &#39;19 {#release-notes-winter}

Le seguenti funzionalità sono incluse nella release invernale &#39;19. Per informazioni sulla disponibilità delle funzionalità, consulta la versione di Marketo.

Fate clic sui collegamenti del titolo per visualizzare gli articoli dettagliati di ciascuna funzione, se disponibili.

>[!NOTE]
>
>Facebook ora richiede un account Business Manager per sfruttare l&#39;integrazione dell&#39;audience personalizzata. Il servizio LaunchPoint di Facebook *deve essere associato a un account Business Manager oppure **l&#39;integrazione non funzionerà più dopo il 14 gennaio 2019**.* Per impostare un account Business Manager, fare riferimento alla [Guida di Facebook](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>Microsoft sta spingendo tutti i clienti online a effettuare l&#39;aggiornamento alla versione più recente di Microsoft Dynamics. Se state integrando l&#39;istanza di Marketo con Dynamics Online, è necessario [eseguire l&#39;aggiornamento alla versione più recente della soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/upgrade-the-marketo-solution-for-microsoft-dynamics.md) prima del **31 gennaio 2019** per garantire che l&#39;integrazione continui a funzionare.

>[!NOTE]
>
>È in corso l&#39;aggiornamento della versione OAuth per GoToWebinar da 1.0 a 2.0. Il supporto per OAuth 1.0 diventerà obsoleto a gennaio 2019. Se sei un cliente GoToWebinar, dovrai autenticare nuovamente gli accessi tramite LaunchPoint (nell&#39;area Amministratore) entro il **31 gennaio 2019** per assicurarti che l&#39;integrazione continui a funzionare. Per ulteriori informazioni, fare riferimento alla nostra [pagina della community](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## Miglioramenti della piattaforma di base {#core-platform-enhancements}

**[E-mail CC per e-mail Marketo](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Puoi includere fino a cinque indirizzi CC per destinatario nelle e-mail inviate tramite Marketo.

**API**

* **Supporto del dominio con più marchi per l’API delle risorse:** approvare e clonare risorse produce gli stessi risultati all’interno dell’API e dell’interfaccia utente.
* **Supporto per e-mail CC per l’API** delle risorse: Gli utenti che duplicano, approvano ed elaborano i messaggi e-mail tramite l&#39;API rimarranno in parità con le impostazioni dell&#39;interfaccia utente.

**[Munchkin v155 (versione beta)](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **Modalità** Solo API: Gli utenti ora possono determinare quando e come monitorare i membri del proprio database consentendo alle app Web a pagina singola di chiamare in modo esplicito quando desiderano registrare una visita a una pagina Web invece di affidarsi al tracciamento automatico di Marketo.
* **Gestione** del rifiuto: Gestite facilmente le opzioni di rifiuto facendo corrispondere il dominio dei cookie di rinuncia con il dominio dei cookie di tracciamento Munchkin.
* **Parametro** Decideder a livello di dominio: Domini a due lettere (ad es. &quot;  [website.io](https://website.io)&quot;) verrà tracciato automaticamente in Marketo senza ulteriori requisiti di configurazione.

## Coinvolgimento vendite marketing {#marketo-sales-engage}

* **Profilo** personalizzato Salesforce: Engage di vendita ora supporta un numero illimitato di profili personalizzati.

* **Personalizzazione** Salesforce: Rimuovendo i campi di attività personalizzati non critici, gli utenti possono configurare il coinvolgimento delle vendite nella piattaforma CRM in modo più efficiente.
* **Servizio** e-mail: Ottenete una migliore recapito e un migliore tracciamento delle risposte, funzionalità e-mail pianificate e funzionalità e-mail in blocco tramite la connessione a Microsoft Outlook (tramite Office365 o On-Prem tramite la scheda Connessione e-mail).
* **Nuove impostazioni** amministratore: Sono state aggiunte due pagine di amministrazione per ottimizzare l’istanza di coinvolgimento nelle vendite

   * _Team_ Management supporta un processo di configurazione dell&#39;account senza soluzione di continuità consentendo agli amministratori di modificare iscrizioni e team.
   * _I team_ di amministrazione delle soluzioni Salesforce configurano la sincronizzazione SFDC in modo più rapido e semplice che mai.

* **Plug-in OWA per Windows**: Con un singolo componente aggiuntivo, tutti i client Windows Office365 saranno supportati in Coinvolgimento vendite, fornendo la possibilità di utilizzare Feed dal vivo in Outlook. Il nuovo plug-in sarà disponibile in Microsoft Store.
* **Spintore attività**: Sincronizza il coinvolgimento nelle vendite con la piattaforma di base Marketo per sfruttare informazioni di marketing in tempo reale.

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>I rilasci Marketo Sky si verificano con cadenza più frequente. Le seguenti funzionalità e miglioramenti dovrebbero essere rilasciati nel corso della fine del Q4 o della prima metà del Q1. Per maggiori dettagli e aggiornamenti, consulta la nostra [documentazione Sky](https://help.marketo.com/).

* **Esperienza** predefinita opzionale: Gli utenti Marketo possono impostare Marketo Sky come esperienza predefinita se gli è stato fornito l&#39;accesso da un amministratore.

* **Riimmagina Il Mio Marketo**: Personalizzate l&#39;esperienza aggiungendo widget che forniscono informazioni critiche, notifiche e collegamenti alle aree visitate più di frequente.

* **Visualizzazione elenco e pagine** di dettagli di Design Studio: È possibile migliorare l&#39;organizzazione e la precisione grazie a viste elenco filtrabili e ricercabili di e-mail, pagine di destinazione e moduli. Le pagine dei dettagli delle risorse forniscono informazioni chiave su ciascuna risorsa, compresi i programmi utilizzati dalla risorsa, il numero di snippet utilizzati e altro ancora.

* **Ricerca** globale: Marketo offre ora una funzione di ricerca globale più veloce e affidabile su tutta la piattaforma. Le query di ricerca ora vengono eseguite in tutte le aree di lavoro accessibili e possono eseguire ricerche in risorse (attive e archiviate), etichette, campagne e programmi. I risultati della ricerca vengono forniti tramite una sovrapposizione e ogni risultato include la traccia della posizione del file per specificare dove vive la risorsa.

* **Interfaccia** utente migliorata: Nuove icone, modelli e pulsanti, insieme a una nuova tavolozza di colori che riflette l&#39;aggiornamento del marchio e rende i Marketo Sky ancora più straordinari e funzionali.

* **Miglioramenti** dell&#39;usabilità del programma e-mail: Continuiamo a progredire verso la parità nelle funzionalità del programma e-mail tra la nostra classica piattaforma di gestione dei lead di Marketo e la nuova esperienza Marketo Sky.
* **Programmi** Eventi Con Webinar: I programmi Event-With Webinar sono ora disponibili in Marketo Sky (nota: in questa versione sarà supportato solo GoToWebinar, con ulteriori integrazioni stabilite nel tempo).

## Marketing basato su account {#account-based-marketing}

**[Segmentazione e filtro basati su ABM Persona](/help/marketo/product-docs/account-based-marketing/using-personas.md)**

Personalizza le tue campagne ABM per persone specifiche all&#39;interno di account denominati. La funzione ABM Persona crea un titolo di processo predefinito basato sulla segmentazione del lead e consente la configurazione di ulteriori segmentazioni personali.

## Analytics {#analytics}

**Bizible**

* **Campi** calcolati personalizzati: Utilizzate qualsiasi attributo Bizible per creare campi personalizzati da utilizzare per il reporting e la segmentazione del dashboard.

* **Certificazione** SOC II di tipo II: La nuova certificazione in materia di sicurezza e privacy si basa sull&#39;accreditamento di tipo I all&#39;inizio di quest&#39;anno.

## Personalizzazione Web {#web-personalization}

**[Aggiungi sottodomini in Impostazioni account](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

Per gestire domini e sottodomini in modo più efficiente, gli utenti ora possono aggiungere sottodomini alle impostazioni dell&#39;account RTP.

## Coinvolgimento Marketo Mobile (MME) {#marketo-mobile-engagement-mme}

**Aggiornato MME Software Development Kit (SDK) per Android**

Abbiamo aggiornato il nostro SDK per Android a una struttura più moderna, stabile e scalabile che contiene più flessibilità e nuove funzionalità di progettazione. Gli sviluppatori di app Android ora possono utilizzare direttamente l&#39;SDK di Google [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) (FCM) con questo nuovo SDK.

* [Istruzioni per gli sviluppatori](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [Domande frequenti per sviluppatori](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>Gli sviluppatori di app **devono** eseguire l&#39;aggiornamento alla nuova versione prima del 31 marzo 2019. Se l’SDK non viene aggiornato entro il 31 marzo 2019, tutti i nuovi utenti che scaricano l’app dopo tale data non potranno ricevere notifiche push fino all’aggiornamento all’ultima versione dell’SDK. L&#39;aggiornamento dell&#39;SDK non richiederà che gli utenti attuali dell&#39;app mobile scaricino nuovamente una nuova versione dell&#39;app.

## Aggiornamenti aggiuntivi {#additional-updates}

**Extensible Webinar Platform**

Oltre al rilascio del nostro prodotto, il nostro team di partner sta lavorando a un nuovo framework che consente ai fornitori di webinar di creare e mantenere le proprie integrazioni con Marketo, fornendo maggiore flessibilità nell&#39;aggiornamento e nel miglioramento delle proprie soluzioni, consentendo al contempo ai professionisti del marketing di trarre il massimo dalle integrazioni scelte.

Prevediamo di implementare la nostra nuova piattaforma con i fornitori, caso per caso. Per ulteriori informazioni, vedere i nostri [dettagli del programma](https://www.marketo.com/why-marketo/partners/technology/) o contattare Marketo.
