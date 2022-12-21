---
unique-page-id: 45416698
description: Note sulla versione - Luglio 20 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Luglio 20
exl-id: 3c9b1f1d-961c-4bf8-8b99-37b483230506
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---

# Note sulla versione: Luglio 20 {#release-notes-july}

Le seguenti funzionalità sono incluse nella versione del 20 luglio. Per informazioni sulla disponibilità delle funzioni, consulta la tua edizione Marketo .

>[!AVAILABILITY]
>
>Tieni presente che, a seconda del pacchetto corrente, gli articoli con una stella ( ![(stella)](assets/yellow-star.png)) può richiedere l’acquisto di un componente aggiuntivo per valori. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

**_Versioni trimestrali_** Le seguenti funzionalità verranno rilasciate il **31 luglio 2020**.

## Amministrazione {#administration}

* **[Esportazione &quot;Utilizzata da&quot; nella gestione dei campi](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)**: Gli amministratori possono ora esportare in un file CSV tutti i collegamenti alle risorse &quot;Usato da&quot; per un campo selezionato. Questo miglioramento può essere utile sia per gli amministratori che per i non amministratori nella pulizia dei campi inutilizzati. Inoltre, le risorse possono ora essere aperte in una nuova scheda o finestra del browser.

## Account-Based Marketing {#account-based-marketing}

![(stella)](assets/yellow-star.png)

* **Interfaccia aggiornata per il profiling dell’account**: Semplifica la creazione dell’elenco degli account di destinazione in Profilo account con passaggi semplificati in un’unica schermata.

<br> 

**_Rilascio in tutto il trimestre_**

Le seguenti caratteristiche sono su un ciclo non trimestrale e saranno rilasciate durante i prossimi mesi.

* **Servizio Forms**: Stiamo introducendo una convalida più forte della sintassi dei campi modulo e la possibilità di bloccare i pattern bot comuni con le nuove funzionalità Domini protetti per le pagine di destinazione. Bloccare i pattern di bot può ridurre gli invii di moduli spam e migliorare la qualità del database.

>[!NOTE]
>
>Il rollout completo della convalida della sintassi dei campi modulo avanzata è stato posticipato fino a dopo la versione di gennaio 2021.

* **Limite dimensione URI API risorsa aumentato**: Il limite di dimensione dell’identificatore di risorsa uniforme (URI) viene aumentato da 8 KB a 65 KB prima della rimozione del parametro &quot;_method&quot;. Quando si eseguono stringhe di query lunghe, questo aumento del limite di dimensione consentirà ai dati di passare più facilmente. La rimozione del parametro &quot;_method&quot; fa parte di un prossimo aggiornamento della sicurezza.

## Approfondimenti vendite {#sales-insight}

![(stella)](assets/yellow-star.png)

* **[Approfondimenti vendite abilitati per i clienti con integrazione CRM non nativa di Salesforce](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md) (Beta)**: I clienti di Marketo Engage con integrazioni CRM non native di Salesforce possono ora utilizzare la funzione Approfondimenti vendite per aiutare i loro team di vendita a comprendere, assegnare le priorità e interagire con i lead e le opportunità più coinvolti per consentire la vendita intelligente e offerte più veloci.

## Sales Connect {#sales-connect}

![(stella)](assets/yellow-star.png)

* **[Consenso avanzato tra due parti per le chiamate di vendita:](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** Gli amministratori ora hanno un maggiore controllo sulle configurazioni di registrazione delle chiamate. [Abilita registrazioni chiamate](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) con la certezza di rispettare la legge sul consenso di due parti. Automatizza la notifica della chiamata in corso e attiva le clip audio da riprodurre prima della chiamata.

<br> 

## Annunci ed elementi obsoleti {#announcements-deprecations}

* **Rimozione parametro API &quot;_method&quot; della risorsa**: A partire da settembre 2020, gli endpoint API di Assets non accetteranno più &quot;_method&quot; per passare i parametri di query nel corpo di un POST per aggirare le limitazioni relative alla lunghezza degli URI. Per soddisfare le richieste che richiedevano questo parametro, i limiti URI per le API delle risorse saranno aumentati da 8 KB a 65 KB.
* **[Capo associato Munchkin](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: Con questa versione del client JavaScript Munchkin, versione 159, inizieremo a rendere obsoleto il metodo Munchkin Associate Lead. Se richiamato, riceverai un avviso che indica che il metodo verrà rimosso in una versione futura. Una volta rimosso, il metodo non sarà più funzionale e i tentativi di utilizzarlo non riusciranno. I clienti del Marketo Engage che hanno recentemente utilizzato questo metodo riceveranno una notifica individuale del loro utilizzo.
* **Supporto per Internet Explorer**: Come annunciato in precedenza, il supporto Marketo Engage per Internet Explorer 11 termina il **31 luglio 2020**. Continueremo a supportare Google Chrome, Mozilla Firefox, Apple Safari e Microsoft Edge.
* **Esperienza predefinita Sky**: L’opzione per gli amministratori o gli utenti di impostare Marketo Sky come esperienza predefinita verrà rimossa in questa versione in preparazione di un aggiornamento dell’esperienza utente principale. Maggiori dettagli sull&#39;aggiornamento dell&#39;esperienza primaria, in programma per la fine di quest&#39;anno, saranno disponibili a luglio. Gli utenti che hanno impostato Marketo Sky come esperienza predefinita o a cui è stato concesso l’accesso ad Marketo Sky possono continuare ad accedere ad Marketo Sky da un riquadro nella home page di My Marketo.
* **Supporto di EdgeHTML (non cromo) Microsoft Edge**: Alla fine del 2020 Marketi Engage non supporterà più le versioni EdgeHTML di Microsoft Edge. A partire dal 1° gennaio 2021, supporteremo solo l’ultima versione di Chromium di Microsoft Edge.
