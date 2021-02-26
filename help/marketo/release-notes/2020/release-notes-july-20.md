---
unique-page-id: 45416698
description: Note sulla versione - Luglio 20 - Documenti Marketo - Documentazione prodotto
title: Note sulla versione - Luglio '20
translation-type: tm+mt
source-git-commit: b33f5ed707a1377daad51191cc6dd9f093138258
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 0%

---


# Note sulla versione: Luglio &#39;20 {#release-notes-july}

Le seguenti funzionalità sono incluse nella release di luglio 20. Per informazioni sulla disponibilità delle funzionalità, consulta la versione di Marketo.

>[!AVAILABILITY]
>
>A seconda del pacchetto corrente, gli elementi con una stella ( ![(star)](assets/star-yellow.svg)) potrebbero richiedere l&#39;acquisto di un componente aggiuntivo di valore. Per ulteriori informazioni, contattate il rappresentante del Marketo Engage.

**_Rilasci_** trimestraliLe seguenti funzionalità verranno rilasciate il 31  **luglio 2020**.

## Amministrazione {#administration}

* **[Esportazione &quot;Utilizzata da&quot; in Gestione](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)** campi: Adesso, gli amministratori possono esportare in un file CSV tutti i collegamenti delle risorse &quot;Usato da&quot; per un campo selezionato. Questo miglioramento può essere utile sia per gli amministratori che per gli utenti che non dispongono di autorizzazioni di livello amministratore per la pulizia dei campi inutilizzati. È inoltre possibile aprire le risorse in una nuova scheda o in una nuova finestra del browser.

## Marketing basato su account {#account-based-marketing}

![(stella)](assets/star-yellow.svg)

* **Interfaccia utente aggiornata per il profilo** account: Semplificate la creazione dell&#39;elenco account di destinazione in Profilo account con passaggi semplificati in un&#39;unica schermata.

<br> 

**_Rilascio per tutto il trimestre_**

Le seguenti funzionalità sono su un ciclo non trimestrale e verranno rilasciate nei prossimi mesi.

* **Servizio** Forms: Stiamo introducendo una convalida della sintassi del campo modulo più efficace e la capacità di bloccare pattern bot comuni con le nuove funzionalità Domini protetti per le pagine di destinazione. Bloccando i pattern dei bot è possibile ridurre l&#39;invio di moduli spam e migliorare la qualità del database.
* **Limite** maggiore di dimensioni URI API risorsa: Il limite di dimensione uniforme per gli URI (Resource Identifier) viene aumentato da 8 KB a 65 KB prima della rimozione del parametro &quot;_method&quot;. Durante l&#39;esecuzione di stringhe di query lunghe, questo aumento del limite di dimensione consentirà il passaggio più semplice dei dati. La rimozione del parametro &quot;_method&quot; fa parte di un prossimo aggiornamento di sicurezza.

## Informazioni sulle vendite {#sales-insight}

![(stella)](assets/star-yellow.svg)

* **[Insight delle vendite abilitato per i clienti con integrazione](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)  CRM Salesforce non nativa (versione beta)**: I clienti Marketi Engage con integrazioni CRM Salesforce non native ora possono utilizzare Sales Insight per aiutare i team di vendita a comprendere, priorizzare e interagire con i lead e le opportunità più coinvolgenti per consentire la vendita intelligente e l&#39;accelerazione delle offerte.

## Connect vendite {#sales-connect}

![(stella)](assets/star-yellow.svg)

* **[Consenso di due parti migliorato per le chiamate di vendita:](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** gli amministratori ora hanno maggiore controllo sulle configurazioni di registrazione delle chiamate. [Abilita ](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) le registrazioni delle chiamate in tutta sicurezza per essere conforme alla legge sul consenso delle due parti. Automatizzate la notifica della chiamata registrata e attivate le clip audio da riprodurre prima della chiamata.

<br> 

## Annunci e ritiri {#announcements-deprecations}

* **Rimozione** parametro API risorsa &quot;_method&quot;: Dopo settembre 2020, gli endpoint API delle risorse non accetteranno più &quot;_method&quot; per passare i parametri di query in un corpo POST per bypassare i limiti di lunghezza URI. Per soddisfare le richieste che richiedevano questo parametro, i limiti URI per le API delle risorse saranno aumentati da 8 KB a 65 KB.
* **[Munchkin Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: Con questa release del client JavaScript Munchkin, versione 159, inizieremo la rimozione del metodo Munchkin Associate Lead. Se richiamato, riceverete un messaggio di avviso che indica che il metodo verrà rimosso in una versione futura. Una volta rimosso, il metodo non sarà più funzionante e i tentativi di utilizzarlo non riusciranno. I clienti Marketi Engage che hanno utilizzato di recente questo metodo riceveranno una notifica individuale del loro utilizzo.
* **Supporto per Internet Explorer**: Come annunciato in precedenza, il supporto Marketo Engage per Internet Explorer 11 termina il 31  **luglio 2020**. Continueremo a supportare Google Chrome, Mozilla Firefox, Apple Safari e Microsoft Edge.
* **Esperienza** predefinita cielo: L&#39;opzione per gli amministratori o gli utenti di impostare Marketo Sky come esperienza predefinita verrà rimossa in questa versione in preparazione di un aggiornamento all&#39;esperienza utente principale. Maggiori dettagli sull&#39;aggiornamento all&#39;esperienza principale, in programma per la fine di quest&#39;anno, saranno disponibili a luglio. Gli utenti che hanno impostato i Marketo Sky come esperienza predefinita, o ai quali è stato concesso l&#39;accesso ai Marketo Sky, possono continuare ad accedere ai Marketo Sky da una sezione della home page di My Marketo.
* **Supporto** di Microsoft EdgeHTML (non cromo): Il Marketo Engage non supporterà più le versioni EdgeHTML di Microsoft Edge alla fine del 2020. A partire dal 1 gennaio 2021, sarà supportata solo l&#39;ultima versione di Chromio di Microsoft Edge.
