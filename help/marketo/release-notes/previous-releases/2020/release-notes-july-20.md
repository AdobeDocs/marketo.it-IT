---
unique-page-id: 45416698
description: Note sulla versione -20 luglio - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Luglio 20
exl-id: 3c9b1f1d-961c-4bf8-8b99-37b483230506
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 0%

---

# Note sulla versione: Luglio &#39;20 {#release-notes-july}

Le seguenti funzioni sono incluse nella versione di luglio 2020. Verifica la disponibilità delle funzioni nella tua edizione di Marketo.

>[!AVAILABILITY]
>
>A seconda del pacchetto corrente, gli elementi con un asterisco ( ![(stella)](assets/yellow-star.png)) potrebbero richiedere l&#39;acquisto di un componente aggiuntivo di valore. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

**_Versioni trimestrali_** Le seguenti funzionalità verranno rilasciate il **31 luglio 2020**.

## Amministrazione {#administration}

* **[Esportazione &quot;Utilizzato da&quot; in Gestione campi](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)**: gli amministratori ora possono esportare tutti i collegamenti alle risorse &quot;Usato da&quot; per un campo selezionato in un file CSV. Questo miglioramento può aiutare sia gli amministratori che i non amministratori a pulire i campi non utilizzati. Inoltre, ora è possibile aprire le risorse in una nuova scheda o finestra del browser.

## Account-Based Marketing {#account-based-marketing}

![(stella)](assets/yellow-star.png)

* **Interfaccia utente aggiornata per la profilazione account**: semplifica la creazione dell&#39;elenco degli account di destinazione in profilazione account con passaggi semplificati in un&#39;unica schermata.

<br> 

**_Rilascio nel corso del trimestre_**

Le seguenti funzioni sono in un ciclo non trimestrale e verranno rilasciate nei prossimi mesi.

* **Servizio Forms**: stiamo introducendo una convalida più avanzata della sintassi del campo modulo e la possibilità di bloccare i pattern bot comuni con le nuove funzionalità Domini protetti per le pagine di destinazione. Il blocco dei pattern di bot può ridurre l’invio di moduli spam e migliorare la qualità del database.

>[!NOTE]
>
>Il rollout completo della convalida della sintassi del campo modulo migliorato è stato posticipato a dopo la versione di gennaio 2021.

* **Limite dimensione URI API risorsa aumentato**: il limite dimensione URI (Uniform Resource Identifier) viene aumentato da 8 KB a 65 KB prima della rimozione del parametro &quot;_method&quot;. Quando si eseguono stringhe di query lunghe, questo aumento del limite di dimensione consentirà ai dati di passare più facilmente. La rimozione del parametro &quot;_method&quot; fa parte di un aggiornamento della sicurezza imminente.

## [!DNL Sales Insight] {#sales-insight}

![(stella)](assets/yellow-star.png)

* **[[!DNL Sales Insight] Abilitato per i clienti con integrazione CRM non nativa [!DNL Salesforce] CRM](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md) (Beta)**: i clienti Marketo Engage con integrazioni CRM [!DNL Salesforce] non native ora possono utilizzare [!DNL Sales Insight] per aiutare i loro team di vendita a comprendere, assegnare priorità e interagire con i lead e le opportunità più coinvolti per consentire vendite intelligenti e offerte più veloci.

## [!DNL Sales Connect] {#sales-connect}

![(stella)](assets/yellow-star.png)

* **[Consenso avanzato di due parti per le chiamate di vendita:](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** gli amministratori ora hanno un maggiore controllo sulle configurazioni di registrazione delle chiamate. [Abilita le registrazioni delle chiamate](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) assicurandoti di rispettare la legge sul consenso di due parti. Automatizza la notifica della registrazione della chiamata e attiva le clip audio da riprodurre prima della chiamata.

<br> 

## Annunci ed elementi obsoleti {#announcements-deprecations}

* **Rimozione parametro &quot;_method&quot; di Asset API**: dopo settembre 2020, gli endpoint di Asset API non accetteranno più &quot;_method&quot; per passare i parametri di query nel corpo di un POST per aggirare le limitazioni relative alla lunghezza degli URI. Per soddisfare le richieste che richiedevano questo parametro, i limiti URI per le API Asset verranno aumentati da 8 KB a 65 KB.
* **[[!DNL Munchkin] Associa lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: con questa versione del client Munchkin JavaScript, versione 159, verrà dichiarata obsoleta la versione del metodo [!DNL Munchkin] Associa lead. Se richiamato, riceverai un avviso che indica che il metodo verrà rimosso in una versione futura. Una volta rimosso, il metodo non sarà più funzionale e i tentativi di utilizzarlo non riusciranno. I clienti Marketo Engage che hanno utilizzato di recente questo metodo riceveranno una notifica individuale del loro utilizzo.
* **Supporto per Internet Explorer**: come annunciato in precedenza, il supporto di Marketo Engage per Internet Explorer 11 termina il **31 luglio 2020**. Continueremo a supportare [!DNL Google Chrome], [!DNL Mozilla Firefox],[!DNL &#x200B; Apple Safari] e [!DNL Microsoft Edge].
* **Esperienza predefinita Sky**: l&#39;opzione che consente agli amministratori o agli utenti di impostare [!DNL Marketo Sky] come esperienza predefinita verrà rimossa in questa versione in preparazione di un aggiornamento dell&#39;esperienza utente principale. Ulteriori dettagli sull’aggiornamento dell’esperienza principale, pianificato per la fine dell’anno, saranno disponibili a luglio. Gli utenti che hanno impostato [!DNL Marketo Sky] come esperienza predefinita o a cui è stato concesso l&#39;accesso a [!DNL Marketo Sky] possono continuare ad accedere a [!DNL Marketo Sky] da un riquadro nella home page di My Marketo.
* Supporto di **EdgeHTML (non Chromium) [!DNL Microsoft Edge]**: Marketo Engage non supporterà più le versioni EdgeHTML di Microsoft Edge alla fine del 2020. A partire dal 1° gennaio 2021, supporteremo solo l’ultima versione di Microsoft Edge in formato Chromium.
