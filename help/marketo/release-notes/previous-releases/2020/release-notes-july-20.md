---
unique-page-id: 45416698
description: Note sulla versione -20 luglio - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Luglio 20
exl-id: 3c9b1f1d-961c-4bf8-8b99-37b483230506
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---

# Note sulla versione: Luglio &#39;20 {#release-notes-july}

Le seguenti funzioni sono incluse nella versione di luglio 2020. Verifica la disponibilità delle funzioni nella tua edizione di Marketo.

>[!AVAILABILITY]
>
>Si prega di notare che, a seconda del pacchetto attuale, gli elementi con una stella ( ![(stella)](assets/yellow-star.png)) può richiedere l&#39;acquisto di una maggiorazione di valore. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

**_Versioni trimestrali_** Le seguenti funzioni verranno rilasciate il **31 luglio 2020**.

## Amministrazione {#administration}

* **[Esportazione &quot;Utilizzato da&quot; nella gestione dei campi](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)**: gli amministratori possono ora esportare in un file CSV tutti i collegamenti alle risorse &quot;Utilizzate da&quot; per un campo selezionato. Questo miglioramento può aiutare sia gli amministratori che i non amministratori a pulire i campi non utilizzati. Inoltre, ora è possibile aprire le risorse in una nuova scheda o finestra del browser.

## Account-Based Marketing {#account-based-marketing}

![(stella)](assets/yellow-star.png)

* **Interfaccia utente aggiornata per la profilazione dell’account**: semplifica la creazione dell’elenco degli account di destinazione in Profilatura account con passaggi semplificati in un’unica schermata.

<br> 

**_Rilascio nel corso del trimestre_**

Le seguenti funzioni sono in un ciclo non trimestrale e verranno rilasciate nei prossimi mesi.

* **Servizio Forms**: stiamo introducendo una convalida più efficace della sintassi del campo modulo e la possibilità di bloccare pattern di bot comuni con nuove funzionalità Domini protetti per le pagine di destinazione. Il blocco dei pattern di bot può ridurre l’invio di moduli spam e migliorare la qualità del database.

>[!NOTE]
>
>Il rollout completo della convalida della sintassi del campo modulo migliorato è stato posticipato a dopo la versione di gennaio 2021.

* **Limite aumentato per le dimensioni dell’URI API delle risorse**: il limite di dimensione dell’URI (Uniform Resource Identifier) viene aumentato da 8 KB a 65 KB prima della rimozione del parametro &quot;_method&quot;. Quando si eseguono stringhe di query lunghe, questo aumento del limite di dimensione consentirà ai dati di passare più facilmente. La rimozione del parametro &quot;_method&quot; fa parte di un aggiornamento della sicurezza imminente.

## Insight sulle vendite {#sales-insight}

![(stella)](assets/yellow-star.png)

* **[Informazioni sulle vendite abilitate per i clienti con integrazione CRM Salesforce non nativa](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md) (Beta)**: i clienti di Marketo Engage con integrazioni CRM Salesforce non native possono ora utilizzare Sales Insight per aiutare i loro team di vendita a comprendere, assegnare priorità e interagire con i lead e le opportunità più coinvolti per consentire vendite intelligenti e operazioni più veloci.

## Sales Connect {#sales-connect}

![(stella)](assets/yellow-star.png)

* **[Consenso di due parti migliorato per le chiamate di vendita:](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** Gli amministratori ora hanno un maggiore controllo sulle configurazioni di registrazione delle chiamate. [Abilita registrazioni chiamate](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) confidando nel rispetto della legge sul consenso di due parti. Automatizza la notifica della registrazione della chiamata e attiva le clip audio da riprodurre prima della chiamata.

<br> 

## Annunci ed elementi obsoleti {#announcements-deprecations}

* **Rimozione parametro &quot;_method&quot; di Asset API**: dopo settembre 2020, gli endpoint API di Asset non accetteranno più &quot;_method&quot; per passare i parametri di query nel corpo di un POST al fine di aggirare le limitazioni relative alla lunghezza degli URI. Per soddisfare le richieste che richiedevano questo parametro, i limiti URI per le API Asset verranno aumentati da 8 KB a 65 KB.
* **[Lead associato Munchkin](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: con questa versione del client JavaScript Munchkin, versione 159, verrà dichiarato obsoleto il metodo Munchkin Associate Lead. Se richiamato, riceverai un avviso che indica che il metodo verrà rimosso in una versione futura. Una volta rimosso, il metodo non sarà più funzionale e i tentativi di utilizzarlo non riusciranno. I clienti del Marketo Engage che hanno utilizzato questo metodo di recente riceveranno una notifica individuale del loro utilizzo.
* **Supporto per Internet Explorer**: come annunciato in precedenza, il supporto di Marketo Engage per Internet Explorer 11 termina il **31 luglio 2020**. Continueremo a supportare Google Chrome, Mozilla Firefox, Apple Safari e Microsoft Edge.
* **Esperienza predefinita Sky**: l’opzione per gli amministratori o gli utenti di impostare Marketo Sky come esperienza predefinita verrà rimossa in questa versione in preparazione di un aggiornamento dell’esperienza utente principale. Ulteriori dettagli sull’aggiornamento dell’esperienza principale, pianificato per la fine dell’anno, saranno disponibili a luglio. Gli utenti che hanno impostato Marketo Sky come esperienza predefinita o a cui è stato concesso l’accesso a Marketo Sky possono continuare ad accedere a Marketo Sky da una sezione della home page di My Marketo.
* **Supporto EdgeHTML (non Chromium) Microsoft Edge**: il Marketo Engage non supporterà più le versioni EdgeHTML di Microsoft Edge alla fine del 2020. A partire dal 1° gennaio 2021, supporteremo solo la versione più recente di Microsoft Edge in formato Chromium.
