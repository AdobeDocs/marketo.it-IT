---
description: Note sulla versione corrente - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione corrente
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: 49b1bd707b8394ceeea0984c4c11d3ac88ab81b6
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 0%

---

# Note sulla versione: Gennaio 2022 {#release-notes-jan-22}

Le seguenti funzionalità sono incluse nella versione del 22 gennaio. Per informazioni sulla disponibilità delle funzioni, consulta l’edizione del Marketo Engage di Adobe.

>[!AVAILABILITY]
>
>Caratteristiche indicate da una stella (![stella](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

**_Versioni trimestrali_**

Le seguenti funzionalità verranno rilasciate il **21 gennaio 2022**.

## Esperienza di nuova generazione {#next-generation-experience}

* **Schermi aggiornati nell’esperienza di nuova generazione**: Nell’esperienza di nuova generazione, offriamo schermi aggiuntivi e aggiornati che offrono miglioramenti di progettazione e usabilità aggiornati tramite l’interruttore di attivazione/disattivazione:

   * Dettagli delle risorse della pagina di destinazione in Design Studio
   * Dettagli delle risorse della pagina di destinazione nelle attività di marketing
   * Visualizzazione elenco e-mail in Design Studio (comprese nuove azioni in blocco)

* **Admin Control per l’interruttore di attivazione/disattivazione esperienza di nuova generazione**: Gli amministratori possono selezionare i tipi di utenti che possono accedere all’interruttore di attivazione/disattivazione per visualizzare le schermate nell’esperienza di nuova generazione.

## Integrazione con Microsoft Dynamics {#microsoft-dynamics-integration}

* **Sincronizzazione del tipo di campo Optionset multiselect Generalmente disponibile**: Sincronizza il tipo di campo set di opzioni multiseletto da Microsoft Dynamics per sfruttare in Elenchi avanzati e Campagne avanzate per un targeting del pubblico più granulare. Gli esempi includono: argomenti/prodotti di interesse, modalità di comunicazione preferita e altro ancora. Questa nuova sincronizzazione è disponibile per Microsoft Dynamics versione 9.X (incluso Dynamics 365 Online).

* **Autenticazione server-to-server per Microsoft Dynamics 365 Online**: Per una maggiore sicurezza, ora supporteremo Server to Server (S2S) come modalità di autenticazione aggiuntiva per l’utente di sincronizzazione del Marketo Engage su Azure Active Directory per l’accesso non interattivo a Microsoft Dynamics 365 Online. Questo consente di utilizzare l’autenticazione a più fattori, in quanto tutte le autenticazione e gli accessi saranno basati su OAuth (solo ID client e segreto client).

>[!NOTE]
>
>La modalità S2S si basa sull’utente dell’applicazione anziché su quello concesso in licenza, il che consente di risparmiare l’utilizzo di una licenza aggiuntiva.

## Amministrazione {#administration}

* **Regole di convalida del modulo**: Mantenere lo stato del database con la possibilità di bloccare i domini e-mail problematici o indesiderati dall’invio dei moduli di Marketo Engage. Il pannello Regola di convalida globale del modulo consente agli amministratori di definire un inserire nell&#39;elenco Bloccati o di abilitare un elenco predefinito di domini consumer liberi per il blocco dai moduli.

* **Sicurezza intestazione pagina di destinazione**: Gli amministratori possono gestire le intestazioni Strict Transport Security e X-Frame Options sui propri domini della pagina di destinazione per applicare requisiti di sicurezza elevati.

**_Rilascio in tutto il trimestre_**

Le seguenti caratteristiche sono su un ciclo non trimestrale e saranno rilasciate durante i prossimi mesi.

## Connettore di destinazione del Marketo Engage AEP - Crea nuovi lead mancanti di rete {#aep-marketo-engage-destination-connector}

I clienti di Marketo Engage che utilizzano anche Adobe Experience Platform (AEP) possono massimizzare il proprio database con la possibilità di inviare record nuovi di persone al Marketo Engage da AEP tramite il connettore di destinazione AEP. Quando invii segmenti di pubblico da AEP al Marketo Engage, le persone all’interno del segmento che non esistono già nel database del Marketo Engage verranno aggiunte automaticamente.

## Approfondimenti vendite {#sales-insight}

![(stella)](assets/yellow-star.png)

* **Informazioni sulle vendite per CRM Salesforce**

* **Nuova colonna di tipi per migliori**: I venditori riceveranno informazioni più rapide con una nuova colonna denominata &quot;Tipo&quot; per distinguere tra lead e contatti nella pagina Best Bets.

* **Aggiornamento API della piattaforma Salesforce**: In risposta al ritiro delle versioni API di Salesforce Platform da 21.0 a 30.0, il pacchetto Insight vendite è stato aggiornato con le API più recenti.

* **Branding aggiornato**: Tutte le pagine Approfondimenti vendite vengono aggiornate per allinearle con il marchio Adobe.

**Approfondimenti vendite per Microsoft Dynamics**

* **Layout account aggiornato**: I venditori possono ottenere una visione collettiva delle attività principali come: attività e-mail, attività web, momenti interessanti e modifiche al punteggio per tutti i contatti all’interno di un account.

## Sales Connect {#sales-connect}

![(stella)](assets/yellow-star.png)

* **Risultati e motivi della chiamata**: Comprendi e monitora gli sforzi in uscita dei tuoi team di vendita in modo più dettagliato con nuove opzioni di risultato della chiamata e del motivo della chiamata completamente personalizzabili. Oltre a questi nuovi campi, stiamo introducendo una nuova governance per applicare il motivo della chiamata e la selezione dei risultati mentre i venditori eseguono chiamate, una nuova governance per abilitare o disabilitare i motivi e i risultati della chiamata e un nuovo campo personalizzato Ragione della chiamata e risultato della chiamata Salesforce Activity per registrare i dati in Salesforce. [Fai clic qui](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) per saperne di più.

* **Personalizzazione dei dettagli dell&#39;attività Salesforce**: Acquisisci ulteriori dati relativi alle attività di vendita e alle attività in Salesforce personalizzando quali informazioni vengono aggiunte al campo oggetto attività Salesforce quando un&#39;attività di vendita viene registrata a Salesforce da Sales Connect. [Fai clic qui](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) per saperne di più.

## Annunci {#announcements}

* **Sunsetting Marketo Sky**: L’11 marzo Marketo Sky non sarà più disponibile in quanto ci occuperemo delle risorse per offrire un’esperienza utente di nuova generazione. Per mantenere l’accesso a funzionalità esclusive di Marketo Sky, a marzo porteremo Asset Expiration e Smart Campaign Priority Override nell’esperienza tradizionale.

* **Elementi obsoleti del modulo**: I POST programmatici non supportati nell’endpoint leadCapture/save2 verranno rifiutati dai moduli di Marketo Engage. [Fai clic qui](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) per saperne di più.

* **Verifica e-mail**: A partire da questa versione, gli abbonamenti al Marketo Engage inizieranno ad avere gli utenti &quot;non-API only&quot; che verificano gli indirizzi e-mail. Gli utenti autenticati del servizio di directory verificheranno automaticamente le loro e-mail quando la loro sottoscrizione viene abilitata con Verifica e-mail. La verifica e-mail per coloro che utilizzano la funzione &quot;Login in Invite User Dialog&quot; o per quelli con abbonamenti che hanno un singolo messaggio e-mail associato a più utenti all’interno dell’abbonamento verrà ritardata e coinciderà con la funzione obsoleta a marzo.

* **Accedi alla finestra di dialogo Invita utente**: A marzo, la funzione opzionale esistente &quot;Accesso nella finestra di dialogo per l’invito di utenti&quot; diventerà obsoleta. La funzionalità &quot;Accesso nella finestra di dialogo per l’invito dell’utente&quot; viene ignorata dalla funzione ID universale, necessaria per la prossima integrazione di sistema di Adobe Identity Management ed è stata abilitata nell’agosto 2021 per tutte le sottoscrizioni. A seguito dell’eliminazione, il Marketo Engage applicherà tutti gli ID utente (accessi) affinché corrispondano all’indirizzo e-mail dell’utente e consentirà l’associazione di un solo utente per indirizzo e-mail all’interno di un abbonamento.
