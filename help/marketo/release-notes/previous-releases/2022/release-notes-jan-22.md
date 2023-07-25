---
description: Note sulla versione - Gennaio 2022 - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione - Gennaio 2022
exl-id: babc4e7f-3f11-4883-80c6-58e69c3e1ab4
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 0%

---

# Note sulla versione: gennaio 2022 {#release-notes-jan-22}

Le seguenti funzioni sono incluse nella versione di gennaio 2022. Verifica la disponibilità delle funzioni nella tua edizione di Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Caratteristiche contrassegnate da una stella (![stella](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

**_Versioni trimestrali_**

Le seguenti funzioni inizieranno ad essere rilasciate il **21 gennaio 2022**, con un rollout graduale di ogni funzione nelle settimane successive (salvo diversa indicazione).

## Esperienza di nuova generazione {#modern-ux}

* **Schermi aggiornati nell’esperienza di nuova generazione**: nell’esperienza di nuova generazione, presentiamo schermi aggiuntivi e aggiornati che offrono un design aggiornato e miglioramenti a livello di usabilità accessibili tramite interruttore:

   * Dettagli sulla risorsa della pagina di destinazione in Design Studio
   * Dettagli sulle risorse della pagina di destinazione nelle attività di marketing

## Integrazione con Microsoft Dynamics {#microsoft-dynamics-integration}

* **Sincronizzazione del tipo di campo Multiselect Optionset generalmente disponibile**: sincronizza il tipo di campo set di opzioni a selezione multipla da Microsoft Dynamics per sfruttare in Elenchi avanzati e Campagne avanzate per un targeting del pubblico più granulare. Alcuni esempi includono: argomenti/prodotti di interesse, modalità di comunicazione preferite e altro ancora. Questa nuova sincronizzazione è disponibile per Microsoft Dynamics versione 9.X (incluso Dynamics 365 Online).

* **Autenticazione da server a server per Microsoft Dynamics 365 Online**: per una maggiore sicurezza, ora supporteremo Server to Server (S2S) come modalità di autenticazione aggiuntiva per l’utente di sincronizzazione del Marketo Engage in Azure Active Directory per l’accesso non interattivo a Microsoft Dynamics 365 Online. Questo ti consente di utilizzare l’autenticazione a più fattori, in quanto tutte le autenticazioni e gli accessi saranno basati su OAuth (solo ID client e segreto client).

>[!NOTE]
>
>La modalità S2S si basa sull&#39;utente dell&#39;applicazione anziché sull&#39;utente con licenza, che consente di risparmiare l&#39;uso di una licenza aggiuntiva.

## Amministrazione {#administration}

* **[Regole di convalida modulo](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**: mantieni l’integrità del database con la possibilità di impedire l’invio di moduli di Marketo Engage a domini e-mail problematici o indesiderati. Il pannello Regola di convalida modulo globale consente agli amministratori di definire un inserisco nell&#39;elenco Bloccati di o di abilitare un elenco predefinito di domini consumer liberi da bloccare dai moduli.

* **[Sicurezza intestazione pagina di destinazione](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**: gli amministratori possono gestire le intestazioni Strict Transport Security e X-Frame Options sui propri domini di pagina di destinazione per applicare requisiti di sicurezza rigorosi.

**_Rilascio nel corso del trimestre_**

Le seguenti funzioni sono in un ciclo non trimestrale e verranno rilasciate nei prossimi mesi.

## Connettore di destinazione Marketo Engage AEP - Creazione di lead nuovi {#aep-marketo-engage-destination-connector}

I clienti di Marketo Engage che utilizzano anche Adobe Experience Platform (AEP) possono massimizzare il database con la possibilità di inviare record di persone nuovi al Marketo Engage da AEP tramite il connettore di destinazione AEP. Quando invii segmenti di pubblico da AEP al Marketo Engage, persone all’interno del segmento che non esistono già nel database di Marketo Engage [può essere aggiunto automaticamente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md).

## Insight sulle vendite {#sales-insight}

![(stella)](assets/yellow-star.png)

**Insight vendite per Salesforce CRM**

* **Nuova colonna Tipo per elementi di maggiore rilevanza**: i venditori riceveranno informazioni più rapide con una nuova colonna denominata &quot;Tipo&quot; per distinguere lead e contatti nella pagina Elementi di maggiore rilevanza.

* **Aggiornamento API Salesforce Platform**: in risposta al ritiro delle versioni 21.0-30.0 dell’API di Salesforce Platform, il pacchetto Sales Insight è stato aggiornato con le API più recenti.

* **Branding aggiornato**: tutte le pagine Sales Insight vengono aggiornate per allinearsi al branding Adobe.

**Informazioni sulla vendita per Microsoft Dynamics**

* **Layout dell’account aggiornato**: i venditori possono ottenere una visione collettiva delle attività principali, ad esempio e-mail, attività web, momenti di interesse e modifiche di punteggio per tutti i contatti all’interno di un account.

## Sales Connect {#sales-connect}

![(stella)](assets/yellow-star.png)

* **Risultati e motivi della chiamata**: scopri e tieni traccia delle attività in uscita dei tuoi team di vendita in modo più dettagliato, con nuove opzioni completamente personalizzabili per esito e motivo della chiamata. Oltre a questi nuovi campi, stiamo introducendo una nuova governance per applicare il motivo della chiamata e la selezione dei risultati durante le chiamate dei venditori, una nuova governance per abilitare o disabilitare i motivi e i risultati delle chiamate e un nuovo campo personalizzato Motivo della chiamata e Risultato della chiamata Attività Salesforce per la registrazione dei dati in Salesforce. [Fai clic qui](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) per ulteriori informazioni.

* **Personalizzazione dettagli attività Salesforce**: acquisisci ulteriori attività di vendita e dati sulle attività in Salesforce personalizzando le informazioni aggiunte al campo dell’oggetto attività Salesforce quando un’attività di vendita viene registrata in Salesforce da Sales Connect. [Fai clic qui](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) per ulteriori informazioni.

## Annunci {#announcements}

* **Obsolescenza Marketo Sky**: a marzo, Marketo Sky non sarà più disponibile, poiché le nostre risorse verranno dedicate alla creazione di un’esperienza di utilizzo di nuova generazione. Nel tentativo di mantenere l’accesso a funzionalità esclusive di Marketo Sky, a marzo presenteremo Asset Expiration e Smart Campaign Priority Override nell’esperienza mainstream. [Fai clic qui](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) per ulteriori informazioni.

* **Endpoint modulo obsoleti**: i moduli programmatici POST non supportati per l’endpoint leadCapture/save2 verranno rifiutati dai moduli di Marketo Engage. [Fai clic qui](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) per ulteriori informazioni.

**Domini Marketo Engage - Configurazione approfondimento vendite**: per i domini di Marketo Engage per i quali non è stato eseguito il provisioning del certificato SSL e https://, le chiamate non riusciranno e verrà restituito un errore di handshake SSL. Pertanto, questi domini saranno ritirati. Di conseguenza, gli utenti di Sales Insight con una configurazione precedente che punta a uno di questi domini potrebbero riscontrare errori di callout di sistema nella pagina Lead, Contact, Account, Opportunity Panels o Marketo Global. Si consiglia di aggiornare [Configurazione Marketo Engage](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) in Salesforce se riscontri questo errore. È sufficiente aggiornare le credenziali del Marketo Engage evidenziate nella sezione &quot;Marketo Sales Insight Config&quot; del documento.

**_Webinar sulla versione del prodotto_**

[Webinar sulla versione del Marketo Engage di gennaio 2022](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)
