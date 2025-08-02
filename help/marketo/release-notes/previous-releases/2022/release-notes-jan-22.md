---
description: Note sulla versione - Gennaio 2022 - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione - Gennaio 2022
exl-id: babc4e7f-3f11-4883-80c6-58e69c3e1ab4
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 0%

---

# Note sulla versione: gennaio 2022 {#release-notes-jan-22}

Le seguenti funzioni sono incluse nella versione di gennaio 2022. Verifica la disponibilità delle funzioni nella tua edizione di Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![stella](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

**_Versioni trimestrali_**

Le seguenti funzionalità inizieranno a essere rilasciate il **21 gennaio 2022**, con un rollout graduale di ogni funzionalità nelle settimane successive (salvo diversa indicazione).

## Esperienza di nuova generazione {#modern-ux}

* **Screens aggiornato nell&#39;esperienza di nuova generazione**: verranno forniti schermi aggiuntivi e aggiornati nell&#39;esperienza di nuova generazione che offrono una progettazione aggiornata e miglioramenti a livello di usabilità accessibili tramite l&#39;interruttore:

   * Dettagli risorsa pagina di destinazione in [!UICONTROL Design Studio]
   * Dettagli risorsa pagina di destinazione in [!UICONTROL Marketing Activities]

## Integrazione di [!DNL Microsoft Dynamics] {#microsoft-dynamics-integration}

* **Sincronizzazione del tipo di campo Multiselect Optionset generalmente disponibile**: sincronizza il tipo di campo Multiselect Optionset da [!DNL Microsoft Dynamics] per sfruttare in elenchi avanzati e campagne avanzate per un targeting più granulare del pubblico. Alcuni esempi includono: argomenti/prodotti di interesse, modalità di comunicazione preferite e altro ancora. Questa nuova sincronizzazione è disponibile per [!DNL Microsoft Dynamics] versione 9.X (incluso Dynamics 365 Online).

* **Autenticazione da server a server per[!DNL Microsoft Dynamics 365 Online]**: per una maggiore sicurezza, è ora possibile supportare Server to Server (S2S) come modalità di autenticazione aggiuntiva per l&#39;utente di sincronizzazione Marketo Engage in Azure Active Directory per l&#39;accesso non interattivo a [!DNL Microsoft Dynamics 365 Online]. Questo ti consente di utilizzare l’autenticazione a più fattori, in quanto tutte le autenticazioni e gli accessi saranno basati su OAuth (solo ID client e segreto client).

>[!NOTE]
>
>La modalità S2S si basa sull&#39;utente dell&#39;applicazione anziché sull&#39;utente con licenza, che consente di risparmiare l&#39;uso di una licenza aggiuntiva.

## Amministrazione {#administration}

* **[Regole di convalida modulo](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**: consente di mantenere l&#39;integrità del database con la possibilità di impedire l&#39;invio di Marketo Engage Form a domini e-mail problematici o indesiderati. Il pannello Regola di convalida modulo globale consente agli amministratori di definire un inserisco nell&#39;elenco Bloccati di o di abilitare un elenco predefinito di domini consumer liberi da bloccare dai moduli.

* **[Sicurezza intestazione pagina di destinazione](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**: gli amministratori possono gestire intestazioni Strict Transport Security e X-Frame Options nei domini delle pagine di destinazione per applicare requisiti di sicurezza elevati.

**_Rilascio nel corso del trimestre_**

Le seguenti funzioni sono in un ciclo non trimestrale e verranno rilasciate nei prossimi mesi.

## Connettore di destinazione Marketo Engage per AEP: creazione di nuovi lead {#aep-marketo-engage-destination-connector}

I clienti di Marketo Engage che utilizzano anche Adobe Experience Platform (AEP) possono massimizzare il database con la possibilità di inviare in rete i nuovi record di persone da AEP a Marketo Engage tramite il connettore di destinazione di AEP. Quando si inviano segmenti di pubblico da AEP a Marketo Engage, è possibile aggiungere automaticamente al segmento persone che non esistono già nel database di Marketo Engage [1.](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md)

## [!DNL Sales Insight] {#sales-insight}

![(stella)](assets/yellow-star.png)

**[!DNL Sales Insight]per [!DNL Salesforce] CRM**

* **Nuova colonna dei tipi per[!UICONTROL Best Bets]**: i venditori riceveranno informazioni più rapide con una nuova colonna denominata &quot;Tipo&quot; per distinguere i lead dai contatti nella pagina [!UICONTROL Best Bets].

* Aggiornamento API **[!DNL Salesforce]della piattaforma**: in risposta al ritiro di [!DNL Salesforce] delle versioni da 21.0 a 30.0 dell&#39;API della piattaforma [!DNL Salesforce], il pacchetto [!DNL Sales Insight] è stato aggiornato con le API più recenti.

* **Branding aggiornato**: tutte le [!DNL Sales Insight] pagine sono in fase di aggiornamento per l&#39;allineamento con il branding Adobe.

**[!DNL Sales Insight]per[!DNL Microsoft Dynamics]**

* **Layout account aggiornato**: i venditori possono ottenere una visualizzazione collettiva delle attività principali, ad esempio: attività e-mail, attività Web, momenti di interesse e variazioni di punteggio per tutti i contatti all&#39;interno di un account.

## [!DNL Sales Connect] {#sales-connect}

![(stella)](assets/yellow-star.png)

* **Risultati e motivi della chiamata**: scopri e tieni traccia in modo più dettagliato degli sforzi dei tuoi team di vendita in uscita con nuove opzioni personalizzabili per esito e motivo della chiamata. Oltre a questi nuovi campi, stiamo introducendo una nuova governance per applicare la selezione del motivo e del risultato della chiamata mentre i venditori effettuano chiamate, una nuova governance per abilitare o disabilitare i motivi e i risultati della chiamata e un nuovo campo personalizzato Motivo chiamata e Risultato chiamata [!DNL Salesforce] attività per la registrazione dei dati in [!DNL Salesforce]. [Fai clic qui](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) per ulteriori informazioni.

* Personalizzazione dettagli attività **[!DNL Salesforce]**: acquisisci ulteriori dati attività di vendita e attività in [!DNL Salesforce] personalizzando le informazioni aggiunte al campo dell&#39;oggetto attività [!DNL Salesforce] quando un&#39;attività di vendita viene registrata in [!DNL Salesforce] da [!DNL Sales Connect]. [Fai clic qui](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) per ulteriori informazioni.

## Annunci {#announcements}

* **Deprecazione di Marketo Sky**: a marzo, Marketo Sky non sarà più disponibile, in quanto le nostre risorse saranno concentrate sulla distribuzione dell&#39;esperienza utente di nuova generazione. Nel tentativo di mantenere l’accesso a funzionalità esclusive di Marketo Sky, a marzo le funzioni Scadenza risorse e Sostituzione priorità campagna avanzata saranno integrate nell’esperienza mainstream. [Fai clic qui](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) per ulteriori informazioni.

* **Deprecazione endpoint modulo**: i moduli programmatici POST non supportati per l&#39;endpoint leadCapture/save2 verranno rifiutati da Marketo Engage Form. [Fai clic qui](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) per ulteriori informazioni.

* **Accesso nella finestra di dialogo Invita utente**: a marzo, la funzionalità opzionale esistente &quot;Accesso nella finestra di dialogo Invita utente&quot; diventerà obsoleta. La funzionalità &quot;[!UICONTROL Login in Invite User Dialog]&quot; è sovrascritta dalla funzionalità Universal ID, necessaria per la prossima integrazione di sistema di Adobe Identity Management, ed è stata abilitata ad agosto 2021 per tutte le sottoscrizioni. In seguito alla rimozione di, Marketo Engage forzerà l’associazione di un solo utente per indirizzo e-mail all’interno di un abbonamento.

**Domini Marketo Engage - [!DNL Sales Insight] Configurazione**: per i domini Marketo Engage per i quali non è stato eseguito il provisioning del certificato SSL e https://, le chiamate non riusciranno e verrà restituito un errore di handshake SSL. Pertanto, questi domini saranno ritirati. Di conseguenza, [!DNL Sales Insight] utenti con una configurazione precedente che punta a uno di questi domini potrebbero riscontrare errori di callout di sistema nella pagina Lead, Contatto, Account, Pannelli opportunità o Globale Marketo. Se riscontri questo errore, ti consigliamo di aggiornare la [configurazione di Marketo Engage](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) in [!DNL Salesforce]. È sufficiente aggiornare le credenziali di Marketo Engage evidenziate nella sezione &quot;[!DNL Marketo Sales Insight] Config&quot; del documento.

**_Webinar sulla versione del prodotto_**

[Webinar sulla versione di Marketo Engage di gennaio 2022](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)
