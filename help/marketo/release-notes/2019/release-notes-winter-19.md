---
unique-page-id: 17727823
description: Note sulla versione - Inverno del 19 - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione - Inverno '19
translation-type: tm+mt
source-git-commit: 9d8a6d9880de5d2af211906c2410f2057c1f454d
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 0%

---


# Note sulla versione: Inverno &#39;19 {#release-notes-winter}

Le seguenti funzionalità sono incluse nella versione Inverno del 19. Per informazioni sulla disponibilità delle funzioni, consulta la tua edizione di Marketo .

Fai clic sui collegamenti del titolo per visualizzare gli articoli dettagliati di ciascuna funzione, se disponibili.

>[!NOTE]
>
>Facebook ora richiede un account Business Manager per sfruttare l’integrazione con i tipi di pubblico personalizzati. Il servizio Facebook LaunchPoint *deve* essere associato a un account Business Manager oppure **l’integrazione non funzionerà più dopo il 14 gennaio 2019**. Per impostare un account Business Manager, fare riferimento alla [Guida di Facebook](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>Microsoft sta inviando a tutti i clienti online l’aggiornamento alla versione più recente di Microsoft Dynamics. Se stai integrando l’istanza Marketo con Dynamics Online, dovrai [eseguire l’aggiornamento alla versione più recente della soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md) prima del **31 gennaio 2019** per garantire che l’integrazione continui a funzionare.

>[!NOTE]
>
>È in corso l’aggiornamento della versione OAuth per GoToWebinar da 1.0 a 2.0. Il supporto per OAuth 1.0 diventerà obsoleto a gennaio 2019. Se sei un cliente GoToWebinar, dovrai autenticare nuovamente gli accessi tramite LaunchPoint (nell’area Amministratore) entro il **31 gennaio 2019** per garantire che l’integrazione continui a funzionare. Per ulteriori informazioni, consulta la nostra [pagina della community](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## Miglioramenti della piattaforma core {#core-platform-enhancements}

**[E-mail CC per e-mail Marketo](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Puoi includere fino a cinque indirizzi CC per destinatario nelle e-mail inviate tramite Marketo.

**API**

* **Supporto per domini con più marchi per API di risorse:** l’approvazione e la clonazione di risorse genera gli stessi risultati all’interno dell’API e dell’interfaccia utente.
* **Supporto per e-mail CC per l’API** delle risorse: Gli utenti che clonano, approvano ed elaborano e-mail tramite l’API manterranno la stessa parità con le impostazioni dell’interfaccia utente.

**[Munchkin v155 (versione beta)](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **Modalità** solo API: Gli utenti ora possono determinare quando e come monitorare i membri del proprio database consentendo alle app web a pagina singola di chiamare esplicitamente quando desiderano registrare una visita a una pagina web invece di affidarsi al tracciamento automatico di Marketo.
* **Gestione** rinunce: Gestisci facilmente le rinunce facendo corrispondere il dominio del cookie di rinuncia con il dominio del cookie di tracciamento Munchkin.
* **Parametro** Decider a livello di dominio: Domini a due lettere (ad es. &quot;  [website.io](https://website.io)&quot;) verrà automaticamente monitorato in Marketo senza requisiti di configurazione aggiuntivi.

## Coinvolgimento vendite Marketo {#marketo-sales-engage}

* **Profilo** personalizzato Salesforce: Il coinvolgimento nelle vendite ora supporta profili personalizzati illimitati.

* **Personalizzazione** Salesforce: Rimuovendo i campi di attività personalizzati non critici, gli utenti possono impostare il coinvolgimento nelle vendite nella piattaforma CRM in modo più efficiente.
* **Servizio** e-mail: È possibile migliorare il recapito messaggi e migliorare il tracciamento delle risposte, le funzionalità e-mail pianificate e le funzionalità di posta elettronica in blocco tramite Microsoft Outlook (tramite Office365 o On-Prem tramite la scheda Connessione e-mail).
* **Nuove impostazioni** amministratore: Sono state aggiunte due pagine di amministrazione per ottimizzare l’istanza di Sales Engage

   * _Team_ Management supporta un processo di configurazione dell’account senza soluzione di continuità, consentendo agli amministratori di modificare abbonamenti e team.
   * _I team_ di Salesforce Admin Settings (Impostazioni amministratore) configurano la sincronizzazione SFDC più rapidamente e più semplice che mai.

* **Plug-in OWA per Windows**: Con un solo componente aggiuntivo, tutti i client Windows Office365 saranno supportati in Sales Engage, fornendo la possibilità di utilizzare Live Feed in Outlook. Il nuovo plug-in sarà disponibile in Microsoft Store.
* **Utilità di spinta** attività: Sincronizza il coinvolgimento nelle vendite con la piattaforma principale Marketo per sfruttare le informazioni di marketing in tempo reale.

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>I rilasci di Marketo Sky avvengono con cadenza più frequente. Le seguenti funzionalità e miglioramenti dovrebbero essere rilasciati durante la fine del Q4/primo trimestre. Per ulteriori dettagli e aggiornamenti, consulta la nostra [documentazione Sky](https://help.marketo.com/).

* **Esperienza** predefinita opzionale: Gli utenti di Marketo possono impostare Marketo Sky come esperienza predefinita se gli è stato fornito l’accesso da un amministratore.

* **Riimmaginato Il Mio Marketo**: Personalizza la tua esperienza aggiungendo widget che forniscono informazioni critiche, notifiche e collegamenti alle aree più visitate.

* **Visualizzazioni elenco e pagine** di dettagli di Design Studio: Usufruisci di un livello maggiore di organizzazione e precisione grazie alle viste elenco filtrabili e ricercabili di e-mail, pagine di destinazione e moduli. Le pagine dei dettagli delle risorse forniscono informazioni chiave su ciascuna risorsa, tra cui i programmi utilizzati dalla risorsa, il numero di snippet utilizzati e altro ancora.

* **Ricerca** globale: Marketo offre ora una funzione di ricerca globale più veloce e affidabile su tutta la piattaforma. Le query di ricerca ora vengono eseguite in tutte le aree di lavoro accessibili e possono eseguire ricerche nelle risorse (attive e archiviate), nelle etichette, nelle campagne e nei programmi. I risultati della ricerca vengono forniti tramite una sovrapposizione e ogni risultato include il relativo percorso di percorso del file per specificare dove si trova la risorsa.

* **Interfaccia** utente migliorata: Nuove icone, modelli e pulsanti, insieme a una nuova palette di colori per riflettere l’aggiornamento del brand e rendere Marketo Sky ancora più sbalorditivo e funzionale.

* **Miglioramenti** a livello di usabilità del programma e-mail: Continuiamo a passare alla parità nella funzionalità del programma e-mail tra la nostra classica piattaforma Marketo Lead Management e la nuova esperienza Marketo Sky.
* **Programmi** evento-con-webinar: In Marketo Sky sono ora disponibili i programmi evento con webinar (nota: in questa versione sarà supportato solo GoToWebinar, con ulteriori integrazioni stabilite nel tempo).

## Marketing basato su account {#account-based-marketing}

**[Segmentazione e filtro basati su ABM Personona](/help/marketo/product-docs/target-account-management/using-personas.md)**

Personalizza le tue campagne ABM per specifici utenti all’interno di account denominati. La funzione ABM Persona crea un titolo di lavoro predefinito basato sulla segmentazione del lead e consente la configurazione di ulteriori segmentazioni personali.

## Analytics {#analytics}

**Bizible**

* **Campi** calcolati personalizzati: Utilizza qualsiasi attributo Bizible per creare campi personalizzati che possono essere utilizzati per il reporting e la segmentazione del dashboard.

* **Certificazione** SOC II di tipo II: La nuova certificazione di sicurezza e privacy si basa sull&#39;accreditamento di tipo I dall&#39;inizio di quest&#39;anno.

## Personalizzazione web {#web-personalization}

**[Aggiungi sottodomini nelle impostazioni account](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

Per gestire domini e sottodomini in modo più efficiente, gli utenti possono ora aggiungere sottodomini alle impostazioni dell’account RTP.

## Coinvolgimento Marketo Mobile (MME) {#marketo-mobile-engagement-mme}

**Kit di sviluppo software MME (SDK) aggiornato per Android**

Abbiamo aggiornato il nostro SDK per Android a un framework più moderno, stabile e scalabile che contiene più flessibilità e nuove funzionalità ingegneristiche. Gli sviluppatori di app Android ora possono utilizzare direttamente Google [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) (FCM) con questo nuovo SDK.

* [Istruzioni per gli sviluppatori](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [Domande frequenti sugli sviluppatori](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>Gli sviluppatori di app **devono** aggiornare la nuova versione prima del 31 marzo 2019. Se non aggiorni l’SDK entro il 31 marzo 2019, qualsiasi nuovo utente che scarica l’app dopo tale data non potrà ricevere notifiche push finché non aggiorni l’ultima versione dell’SDK. L&#39;aggiornamento dell&#39;SDK non richiederà agli utenti attuali dell&#39;app mobile di scaricare nuovamente una nuova versione dell&#39;app.

## Aggiornamenti aggiuntivi {#additional-updates}

**Piattaforma di webinar estensibile**

Oltre alla versione del nostro prodotto, il nostro team partner sta lavorando a un nuovo framework che consente ai fornitori di webinar di creare e mantenere le proprie integrazioni con Marketo, fornendo maggiore flessibilità nell’aggiornamento e nel miglioramento delle proprie soluzioni, consentendo al contempo ai professionisti del marketing di trarre il massimo dalle integrazioni scelte.

Prevediamo di implementare la nostra nuova piattaforma con i provider caso per caso. Per ulteriori informazioni, consulta i nostri [dettagli del programma](https://www.marketo.com/why-marketo/partners/technology/) o contatta il tuo contatto Marketo.
