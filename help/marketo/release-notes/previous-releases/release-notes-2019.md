---
title: 2019
description: 2019 - Documentazione di Marketo - Documentazione del prodotto
feature: Release Information
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: d65b4a73-87a3-4d56-b638-74e74d9939ceid: e2290edd-b061-4880-9d79-dee306cf5aa9id: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: ea90ebee-5c84-42d9-8b21-006bdabc95a3id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bccid: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2: id: a1d50dda-6d94-4e16-8c30-5eb7181c4650id: d5c7388a-594e-4d15-9b39-98d6ce479e8bid: de9e3aa9-f002-4fe1-897b-09ee3c55114bid: df8eb12b-4f82-491f-acbb-d74012ca5654id: ffdd6159-0e10-4a57-8021-94e93bab8183
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: bbbea26f-9621-49eb-9ab8-e06fb3bbce8cid: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: d095671a-1355-40aa-8b5f-06c33c68080bid: e0eb8757-182f-49f3-94a4-1587d16f5094id: e1e0219c-f879-479f-8427-888ed2a6e9c2id: eddd9b14-83bd-4ff4-9072-54a4a484abb7id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 4d4669f3239b43afbcbd660644c8d1a35734a556
workflow-type: tm+mt
source-wordcount: 2528
ht-degree: 0%

---

# 2019

## Inverno 2019 {#winter}

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

   * *Gestione team* supporta un processo di configurazione dell&#39;account semplice consentendo agli amministratori di modificare abbonamenti e team.
   * *Impostazioni amministratore Salesforce* consente ai team di configurare la sincronizzazione SFDC in modo più rapido e semplice che mai.

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

## Analisi {#analytics}

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

## Primavera 2019 {#spring}

Le seguenti funzioni sono incluse nella versione di primavera del 19. Verifica la disponibilità delle funzioni nella tua edizione di Marketo.

Fai clic sui collegamenti del titolo per visualizzare articoli dettagliati per ciascuna funzione, se disponibile.

***Versioni trimestrali_**

Le seguenti funzionalità sono state rilasciate il 15 marzo 2019.

## Miglioramenti della piattaforma core {#core-platform-enhancements}

* **In lista d&#39;attesa:** nuovo stato di programma/evento per l&#39;inserimento in lista d&#39;attesa di un membro quando si desidera [bloccarlo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md) fino all&#39;apertura di un ruolo vacante. Questo vale per i canali associati ai programmi Event in Marketo Classic e sia Event che Event con i programmi Webinar in [!DNL Marketo Sky]. Per impostazione predefinita, In lista d’attesa ha lo stesso valore di passaggio di Registrato.
* **[Limite di comunicazione personalizzato](/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md)**: gli amministratori ora possono impostare limiti di comunicazione giornalieri o settimanali personalizzati.
* **[API per risorse Smart Campaign](https://developers.marketo.com/rest-api/assets/smart-campaigns/)**: arricchisci le analisi al di fuori di Marketo con il recupero intelligente dei record della campagna in base alla data e all&#39;ID aggiornati.
* **Collegamenti di tracciamento HTTPS per e-mail:** Per i clienti che hanno acquistato &quot;Domini protetti per collegamenti di tracciamento&quot;, i collegamenti di tracciamento con marchio possono ora essere visualizzati nelle e-mail come HTTPS.
* **Aggiornamenti Powerpack per il recapito messaggi e-mail**: possibilità di contrassegnare e commentare specifici risultati dei test, condividere i risultati con le parti interessate tramite un URL e tenere traccia delle modifiche per visualizzare l&#39;evoluzione di un messaggio e-mail mentre le parti interessate modificano il contenuto.

Account-Based Marketing

**[AccountAI](/help/marketo/product-docs/target-account-management/account-profiling/account-profiling-ranking-and-tuning.md)** Ora disponibile a livello generale. AccountAI utilizza l’intelligenza artificiale per visualizzare gli account di destinazione per la strategia ABM.

<br> 

**_Versioni Non Trimestrali_**

Le seguenti funzionalità dovrebbero essere rilasciate nel corso del primo trimestre del calendario e all&#39;inizio del secondo trimestre del 2019.

## [!DNL Marketo Sky] {#marketo-sky}

* **Funzionalità completa del programma e-mail**: invia e-mail, crea test A/B e tieni traccia dei risultati in un&#39;esperienza semplice.
* **Funzionalità Smart Campaign**: maggiore stabilità in una nuova interfaccia utente con il continuo rollout della funzionalità Smart Campaign in Sky.
* **Gestisci Assets di Design Studio**: è stata aggiunta la possibilità di gestire in blocco modelli, immagini, Forms, snippet, file, e-mail e pagine di destinazione dalle viste elenco di Design Studio.
* **Dashboard del fuso orario del destinatario**: comprendi il comportamento del cliente con i rapporti per le e-mail inviate utilizzando la funzione Consegna nel fuso orario del destinatario in Sky.

## Marketo Sales Engage {#marketo-sales-engage}

* **Controllo avanzato**: nuova visibilità per tutte le persone, le e-mail e il [contenuto](/help/marketo/product-docs/marketo-sales-connect/templates/view-template-list-as-another-user.md) in un&#39;istanza con la possibilità di [terminare le campagne esistenti](/help/marketo/product-docs/marketo-sales-connect/campaigns/view-campaigns-list-as-another-user.md)create da altri utenti.
* **[Gestione annullamento abbonamento](/help/marketo/product-docs/marketo-sales-connect/email/unsubscribes/marketo-unsubscribe-check.md)**: ottimizzazione del recapito messaggi e della conformità con la possibilità di [bloccare i domini e-mail](/help/marketo/product-docs/marketo-sales-connect/admin/blocked-domains.md) da contattare. Marketo farà inoltre riferimento al database dei lead per gli annullamenti dell’abbonamento prima di inviare un’e-mail.

## [!DNL Bizible] di Marketo {#bizible-by-marketo}

* **[!DNL Bizible]Scopri i miglioramenti delle funzioni**: le nuove funzionalità di segmentazione del dashboard consentono agli addetti al marketing di comprendere meglio le prestazioni.
* **Supporto multi-valuta**: consente di passare dalla valuta aziendale a qualsiasi valuta locale con la nuova funzionalità di conversione automatica della valuta di [!DNL Bizible] basata sulle tabelle di valuta CRM.
* **Costi campagna CRM**: misura la spesa e il ROI delle attività di marketing offline con la possibilità di estrarre automaticamente i dati dei costi dall&#39;oggetto campagna CRM.

## Giugno 2019 {#june}

Le seguenti funzioni sono incluse nella versione del 19 giugno. Verifica la disponibilità delle funzioni nella tua edizione di Marketo.

**_Versioni trimestrali_**

Le seguenti funzionalità sono state rilasciate il 14 giugno 2019.

## Servizi di base di Marketo {#marketo-core-services}

* **Checksum dell&#39;estrazione in blocco dei file**: verificare che sia stato recuperato un file completo confrontando l&#39;hash del file con la stringa di checksum dei processi di estrazione completati.
* **Migrazione automatizzata da e-mail 1.0 a e-mail 2.0**: e-mail 2.0 è completamente compatibile con e-mail 1.0 e modelli. Scopri nuove funzionalità, come la possibilità di raggruppare gli elementi di contenuto (immagini, testo, ecc.) nei moduli, definisci variabili come Stringa, Colore, Immagine, ecc. all’interno dei modelli e sfrutta i modelli iniziali completamente reattivi. Include anche un selettore del modello e-mail visivo.

>[!CAUTION]
>
>A partire dal 18 giugno 2019, E-mail 1.0 non è più disponibile. Ulteriori informazioni su E-mail 2.0 e sulla rimozione di E-mail 1.0 [qui](https://nation.marketo.com/docs/DOC-7038).

## Account-Based Marketing {#account-based-marketing}

* Corrispondenza account **[!DNL LinkedIn](BETA)**: è ora disponibile una nuova funzionalità ABM in versione beta che consente di inviare elenchi di account noti e con spazi vuoti direttamente da Marketo a LinkedIn. Questa funzionalità è inclusa automaticamente per tutti i clienti ABM di Marketo.

<br> 

**_Rilascio nel corso del trimestre_**

Le seguenti funzionalità dovrebbero essere rilasciate nel corso del secondo trimestre del calendario e all&#39;inizio del terzo trimestre del 2019.

## [!DNL Marketo Sky] {#marketo-sky}

* **Capi evento** e **Obiettivi evento** sono generalmente disponibili in [!DNL Marketo Sky] nel componente aggiuntivo Eventi Premium.

   * Limiti per gli eventi: ottimizza l’esperienza del cliente per i tuoi eventi e webinar con limiti di registrazione, reindirizzamenti di pagina e funzionalità di lista d’attesa.
   * Obiettivi dell’evento: imposta gli obiettivi di registrazione e partecipazione all’evento e tieni traccia dell’avanzamento in tempo reale.

* **Collegamenti di navigazione completi**: è stata abilitata la navigazione in tutte le applicazioni per cui sono state concesse autorizzazioni, ad esempio Hootsuite, Calendar e altro ancora.
* **Visualizzazioni elenco e-mail, pagina di destinazione, frammento di codice, modulo, immagine e file**: visualizza, cerca ed esegue azioni di massa su qualsiasi risorsa in Design Studio.
* **Pagina dettagli immagine, file e snippet**: ottieni dettagli rapidi sulle risorse con metadati come _creato alle/entro_ e azioni come _elimina_ e _approva_.
* **Widget post blog community**: accesso ai post recenti dalla community in My Marketo.
* **Widget a breve scadenza**: aggiungi il widget &quot;In scadenza&quot; alla dashboard di My Marketo per vedere quali campagne e pagine di destinazione sono impostate per scadere in seguito.
* **Altre smart list**: segmentare e impostare la destinazione in modo appropriato con altre smart list, inclusi il passaggio di flusso &quot;Crea attività&quot;, le regole degli smart list CRM e altro ancora.
* **Email Champion/Challenger Details Page**: visualizza dati come criteri di vittoria, creati alle, ecc. dai tuoi test e-mail champion/Challenger.

## Marketo [!DNL Sales Connect] {#marketo-sales-connect}

* **Azioni in blocco nella personalizzazione [!DNL Salesforce]**: massimizza la produttività inviando e-mail e aggiungendo contatti alle campagne in blocco con la personalizzazione [!DNL Salesforce].
* **Impostazioni - [!DNL Salesforce] Pagina per amministratori e non amministratori**: gestisci l&#39;istanza [!DNL Sales Connect] con una visualizzazione chiara dell&#39;istanza [!DNL Salesforce] connessa a [!DNL Sales Connect], nonché dell&#39;indirizzo e-mail personale agli aggiornamenti [!DNL Salesforce]. Le impostazioni di sincronizzazione migliorate per amministratori, non amministratori e Sincronizzazione a livello di team verranno rilasciate nei prossimi mesi.
* **Impostazioni - Pagina di integrazione**: uno sportello unico per tutte le integrazioni, in modo da poter ottenere il massimo dal nostro ecosistema aperto.
* **Impostazioni - Pagina profilo**: visualizza e aggiorna i dettagli dell&#39;account, cambia la password e controlla lo stato dell&#39;implementazione dell&#39;istanza in questa nuova pagina profilo.

* **Modelli e-mail di sistema**: funzionalità di progettazione, reattività e internazionalizzazione aggiornate.

## [!DNL Bizible] di Marketo {#bizible-by-marketo}

* **Supporto multi-valuta per[!DNL Dynamics]**: [!DNL Bizible] si adatta ora alle tabelle di valuta [!DNL Microsoft Dynamics], per passare facilmente dalla valuta aziendale a quella locale. (Nota: il supporto per SFDC è stato rilasciato nel primo trimestre del 2019.)
* **Integrazione derivazione**: scopri in che modo le conversazioni derivate influiscono sul percorso del cliente. [!DNL Bizible] richiamerà inoltre gli indirizzi e-mail dalle conversazioni per creare un nuovo lead o collegare il punto di contatto a un lead esistente.
* **Localizzazione**: [!DNL Bizible] è ora disponibile in tutte le lingue supportate da Marketo (inglese, giapponese, tedesco, spagnolo, francese e portoghese).

_**Webinar sulla versione del prodotto**_ Guarda la registrazione del nostro webinar sulle innovazioni della versione di giugno &#39;19 [qui](https://engage.marketo.com/Marketo-June-Product-Release-2019-On-Demand.html).

## Agosto 2019 {#august}

Le seguenti funzioni sono incluse nella versione di agosto 19. Verifica la disponibilità delle funzioni nella tua edizione di Marketo.

**_Versioni trimestrali_**

Le seguenti funzionalità sono state rilasciate il 16 agosto 2019.

## Marketo Engage core {#core-marketo-engage}

* **Extensible Webinar Framework**: risparmia tempo con il nuovo framework di webinar preconfigurato di Marketo (introdotto nelle note sulla versione di Winter &#39;19) che trasmette senza problemi i dati dai provider di webinar a Marketo e viceversa. Cvent e Zoom sono ora disponibili in questo nuovo framework.
* **Aggiornamento API di Smart Campaign**: gestisci le funzionalità del ciclo di vita di Smart Campaign mentre viene completata l&#39;interfaccia CRUD (create, read, update, delete).
* **Modifica API intestazioni e-mail**: l&#39;API Aggiorna intestazione e-mail non richiede più che un&#39;e-mail abbia un modello allegato per aggiornare i campi dell&#39;intestazione, ad esempio la riga dell&#39;oggetto.

**Account-Based Marketing** ![(stella)](assets/yellow-star.png)

* La corrispondenza dell&#39;account **[!DNL LinkedIn]**, precedentemente in versione beta, è ora generalmente disponibile.
* È in corso il rebranding ufficiale di **AccountAI** come **profilazione account**.

<br> 

**_Rilascio nel corso del trimestre_**

Le seguenti funzionalità sono presentate in un ciclo non trimestrale e saranno rilasciate durante il terzo trimestre del calendario e all’inizio del quarto trimestre del 2019.

**[!DNL Marketo Sales Connect]** ![(stella)](assets/yellow-star.png)

* **Miglioramento del layout della pagina Persone:** Gestisci persone e gruppi tramite le importazioni di elenchi e le azioni collettive nel nuovo layout della pagina Persone.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella ( ![(stella)](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo.

>[!NOTE]
>
>**Deprecazione di TLS 1.0 e 1.1**: per allinearsi allo standard Adobe per la sicurezza, a partire dal 13 dicembre 2019 il supporto per TLS (Transport Layer Security) 1.0 e 1.1 verrà rimosso. I sistemi che si integrano con Marketo non conformi al protocollo 1.2 potrebbero perdere l’accesso ai servizi Marketo Engage.
>
>**Per mantenere l&#39;accesso a Marketo Engage, verificare che tutti i sistemi client siano conformi a TLS 1.2 prima del 13 dicembre 2019**. Ulteriori informazioni sono disponibili [qui](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq).

**_Webinar sulla versione del prodotto_** [Unisciti a noi](https://engage.marketo.com/August_19_Release_Webinar.html) il 28 agosto alle 1:00PM PT / 4:00PM ET per un webinar live ospitato dal nostro team di prodotto e scopri di più sulle funzioni incluse in questa versione.
