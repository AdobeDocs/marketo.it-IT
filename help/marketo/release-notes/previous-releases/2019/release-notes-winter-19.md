---
unique-page-id: 17727823
description: Note sulla versione - Inverno del 19 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Inverno '19
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 0%

---

# Note sulla versione: Inverno &#39;19 {#release-notes-winter}

Le seguenti funzioni sono incluse nella versione Inverno del 19. Per informazioni sulla disponibilità delle funzioni, consulta la tua edizione Marketo .

Fai clic sui collegamenti del titolo per visualizzare gli articoli dettagliati di ciascuna funzione, se disponibili.

>[!NOTE]
>
>Facebook ora richiede un account Business Manager per sfruttare l’integrazione con Custom Audience. Servizio Facebook LaunchPoint *deve* essere associato a un account Business Manager o **l’integrazione non funzionerà più dopo il 14 gennaio 2019**. Per configurare un account Business Manager, fare riferimento a [Guida di facebook](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>Microsoft sta inviando a tutti i clienti online l’aggiornamento alla versione più recente di Microsoft Dynamics. Se stai integrando la tua istanza di Marketo con Dynamics Online, dovrai [aggiornamento alla versione più recente della soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md) prima **31 gennaio 2019** per garantire il funzionamento dell’integrazione.

>[!NOTE]
>
>È in corso l’aggiornamento della versione OAuth per GoToWebinar da 1.0 a 2.0. Il supporto per OAuth 1.0 diventerà obsoleto a gennaio 2019. Se sei un cliente GoToWebinar, dovrai autenticare nuovamente gli accessi tramite LaunchPoint (nell’area Amministratore) tramite **31 gennaio 2019** per garantire il funzionamento dell’integrazione. Per maggiori dettagli, consulta la nostra [Pagina della community](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## Miglioramenti alla piattaforma core {#core-platform-enhancements}

**[E-mail CC per e-mail Marketo](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Puoi includere fino a cinque indirizzi CC per destinatario nelle e-mail inviate tramite Marketo.

**API**

* **Supporto del dominio con più marchi per l’API delle risorse:** L’approvazione e la clonazione delle risorse producono gli stessi risultati all’interno dell’API e dell’interfaccia utente.
* **Supporto di e-mail per l’API delle risorse**: Gli utenti che clonano, approvano ed elaborano e-mail tramite l’API manterranno la stessa parità con le impostazioni dell’interfaccia utente.

**[Munchkin v155 (versione beta)](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **Modalità solo API**: Gli utenti possono ora determinare quando e come monitorare i membri del proprio database consentendo alle app web a pagina singola di chiamare esplicitamente quando desiderano registrare una visita a una pagina web invece di fare affidamento sul monitoraggio automatico di Marketo.
* **Gestione delle rinunce**: Gestisci facilmente le rinunce facendo corrispondere il dominio del cookie di rinuncia con il dominio del cookie di tracciamento Munchkin.
* **Parametro Decider a livello di dominio**: Domini a due lettere (ad es. &quot; [sito web.io](https://website.io)&quot;) eseguirà automaticamente il tracciamento in Marketo senza ulteriori requisiti di configurazione.

## Marketo Sales Engage {#marketo-sales-engage}

* **Profilo personalizzato Salesforce**: Il coinvolgimento nelle vendite ora supporta profili personalizzati illimitati.

* **Personalizzazione Salesforce**: Rimuovendo i campi di attività personalizzati non critici, gli utenti possono impostare il coinvolgimento nelle vendite nella piattaforma CRM in modo più efficiente.
* **Servizio e-mail**: Migliore recapito messaggi, migliore tracciamento delle risposte, funzionalità e-mail pianificate e funzionalità di posta elettronica in blocco tramite la connessione a Microsoft Outlook (tramite Office365 o On-Prem tramite la scheda Connessione e-mail).
* **Nuove impostazioni amministratore**: Sono state aggiunte due pagine di amministrazione per ottimizzare l’istanza di Sales Engage

   * _Gestione team_ supporta un processo di configurazione dell’account senza soluzione di continuità, consentendo agli amministratori di modificare abbonamenti e team.
   * _Impostazioni amministratore Salesforce_ consente ai team di configurare la sincronizzazione SFDC in modo più rapido e semplice.

* **Plug-in OWA per Windows**: Con un solo componente aggiuntivo, tutti i client Windows Office365 saranno supportati in Sales Engage, fornendo la possibilità di utilizzare Live Feed in Outlook. Il nuovo plug-in sarà disponibile in Microsoft Store.
* **Utilità di spinta attività**: Sincronizza il coinvolgimento nelle vendite con la piattaforma Marketo di base per sfruttare le informazioni di marketing in tempo reale.

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>I rilasci di Marketo Sky avvengono con cadenza più frequente. Le seguenti funzionalità e miglioramenti dovrebbero essere rilasciati durante la fine del Q4/primo trimestre. Per maggiori dettagli e aggiornamenti, consulta la nostra [Documentazione di Sky](https://help.marketo.com/).

* **Esperienza predefinita opzionale**: Gli utenti Marketo possono impostare Marketo Sky come esperienza predefinita se gli è stato fornito l’accesso da un amministratore.

* **Reimmaginato il mio Marketo**: Personalizza la tua esperienza aggiungendo widget che forniscono informazioni critiche, notifiche e collegamenti alle aree più visitate.

* **Viste elenco di Design Studio e pagine di dettagli**: Usufruisci di un livello maggiore di organizzazione e precisione grazie alle viste elenco filtrabili e ricercabili di e-mail, pagine di destinazione e moduli. Le pagine dei dettagli delle risorse forniscono informazioni chiave su ciascuna risorsa, tra cui i programmi utilizzati dalla risorsa, il numero di snippet utilizzati e altro ancora.

* **Ricerca globale**: Marketo offre ora una funzione di ricerca globale più rapida e solida su tutta la piattaforma. Le query di ricerca ora vengono eseguite in tutte le aree di lavoro accessibili e possono eseguire ricerche nelle risorse (attive e archiviate), nelle etichette, nelle campagne e nei programmi. I risultati della ricerca vengono forniti tramite una sovrapposizione e ogni risultato include il relativo percorso di percorso del file per specificare dove si trova la risorsa.

* **Interfaccia utente migliorata**: Nuove icone, modelli e pulsanti, insieme a una nuova palette di colori per riflettere l’aggiornamento del brand e rendere Marketo Sky ancora più sbalorditivo e funzionale.

* **Miglioramenti a livello di usabilità del programma e-mail**: Continuiamo a migliorare la funzionalità del programma e-mail tra la nostra piattaforma classica Marketo Lead Management e la nuova esperienza Marketo Sky.
* **Programmi evento-con-webinar**: In Marketo Sky sono ora disponibili i programmi evento con webinar (nota: in questa versione sarà supportato solo GoToWebinar, con ulteriori integrazioni stabilite nel tempo).

## Account-Based Marketing {#account-based-marketing}

**[Segmentazione e filtro basati su ABM Personona](/help/marketo/product-docs/target-account-management/using-personas.md)**

Personalizza le tue campagne ABM per specifici utenti all’interno di account denominati. La funzione ABM Persona crea un titolo di lavoro predefinito basato sulla segmentazione del lead e consente la configurazione di ulteriori segmentazioni personali.

## Analytics {#analytics}

**Bizible**

* **Campi calcolati personalizzati**: Utilizza qualsiasi attributo Bizible per creare campi personalizzati che possono essere utilizzati per il reporting e la segmentazione del dashboard.

* **Certificazione SOC II di tipo II**: La nuova certificazione di sicurezza e privacy si basa sull&#39;accreditamento di tipo I dall&#39;inizio di quest&#39;anno.

## Personalizzazione web {#web-personalization}

**[Aggiungi sottodomini nelle impostazioni account](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

Per gestire domini e sottodomini in modo più efficiente, gli utenti possono ora aggiungere sottodomini alle impostazioni dell’account RTP.

## Marketo Mobile Engagement (MME) {#marketo-mobile-engagement-mme}

**Aggiornamento del kit di sviluppo software MME (SDK) per Android**

Abbiamo aggiornato il nostro SDK per Android a un framework più moderno, stabile e scalabile che contiene più flessibilità e nuove funzionalità ingegneristiche. Gli sviluppatori di app Android ora possono utilizzare direttamente Google [Messaggistica Firebase Cloud](https://firebase.google.com/docs/cloud-messaging/) (FCM) con questo nuovo SDK.

* [Istruzioni per gli sviluppatori](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [Domande frequenti sugli sviluppatori](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>Sviluppatori di app **deve** aggiornamento alla nuova versione prima del 31 marzo 2019. Se non aggiorni l’SDK entro il 31 marzo 2019, qualsiasi nuovo utente che scarica l’app dopo tale data non potrà ricevere notifiche push finché non aggiorni l’ultima versione dell’SDK. L&#39;aggiornamento dell&#39;SDK non richiederà agli utenti attuali dell&#39;app mobile di scaricare nuovamente una nuova versione dell&#39;app.

## Aggiornamenti aggiuntivi {#additional-updates}

**Piattaforma di webinar estensibile**

Oltre alla versione del nostro prodotto, il nostro team partner sta lavorando a un nuovo framework che consente ai fornitori di webinar di creare e mantenere le proprie integrazioni con Marketo, fornendo maggiore flessibilità nell’aggiornamento e nel miglioramento delle proprie soluzioni, consentendo al contempo agli esperti di marketing di trarre il massimo dalle integrazioni scelte.

Prevediamo di implementare la nostra nuova piattaforma con i provider caso per caso. Per ulteriori informazioni, consulta la nostra [dettagli del programma](https://www.marketo.com/why-marketo/partners/technology/) o contatta il tuo contatto Marketo.
