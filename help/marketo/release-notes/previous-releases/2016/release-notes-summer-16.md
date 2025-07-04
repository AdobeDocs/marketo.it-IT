---
unique-page-id: 11380218
description: Note sulla versione - Estate del 16 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Estate 2016
exl-id: 3843668e-c729-42aa-b05c-55c33ee0d783
source-git-commit: 2b72932606a93d061eb2f57c0ff3256b94a0c20c
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# Note sulla versione: estate del &#39;16 {#release-notes-summer}

Le seguenti funzioni sono incluse nella versione dell’estate del 16. Verifica la disponibilità delle funzioni nella tua edizione di Marketo. Fai clic sui collegamenti del titolo per visualizzare articoli dettagliati per ciascuna funzione.

## [Marketing basato su account](https://docs.marketo.com/display/docs/account+based+marketing) {#account-based-marketing}

Il marketing basato su account Marketo offre tutte le funzionalità di base in un’unica piattaforma unificata:

* **Target** - Individuazione account, corrispondenza lead-account ed elenchi di account denominati
* **Coinvolgi** - Personalization basato su account, coinvolgimento su più canali e flussi di lavoro specifici per l&#39;account
* **Misura** - Informazioni a livello di account ed elenco, punteggio di coinvolgimento dell&#39;account e impatto sulla pipeline e sui ricavi

![](assets/abm-5-acme.png)

>[!NOTE]
>
>ABM è disponibile come componente aggiuntivo per l’abbonamento a Marketo; per favore contatta il tuo rappresentante di vendita per l’implementazione.

## [Audit trail](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md) {#audit-trail}

Audit trail fornisce una cronologia completa delle modifiche apportate all’interno dell’abbonamento Marketo. Creerà responsabilità tra utenti e amministratori, aiuterà a identificare la causa di comportamenti imprevisti e fornirà la sicurezza di sapere chi sta facendo cosa e quando. Queste informazioni saranno disponibili in qualsiasi momento e possono essere utilizzate per rispondere a domande quali:

* Cos’è successo a questa risorsa o impostazione e chi l’ha aggiornata per ultimo?
* Cosa ha fatto X l&#39;utente?
* Chi accede al nostro account?

![](assets/audit-trail.png)

## Integrazione Marketo-Vibes SMS LaunchPoint

Creazione semplice di messaggi SMS direttamente in Marketo. Personalizza e indirizza il messaggio utilizzando dati Marketo avanzati e monitorane facilmente le prestazioni tramite la dashboard dei messaggi SMS.

>[!NOTE]
>
>Questa funzionalità richiede un account [!DNL Vibes SMS] esistente.

![](assets/vibes-sms2.png)

## [Miglioramenti e-mail 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-enhancements}

**Variabili a livello di modulo**

In precedenza, tutte le variabili specificate in Modelli e-mail 2.0 erano &quot;globali&quot; nell’ambito. Quando si utilizzano le variabili all’interno dei moduli, questo non è sempre opportuno se si intende utilizzare più istanze del modulo. Con questa versione, le variabili possono ora essere specificate come &quot;livello modulo&quot;, che consente di indicare che l’utente deve essere in grado di impostare valori univoci per ogni modulo in cui vengono utilizzate.

![](assets/module-level-variables.png)

**Aggiornamenti sintassi**

* Ora è possibile utilizzare &quot;mktoAddByDefault&quot; sui moduli specificati in Modelli e-mail 2.0 per indicare quali moduli devono essere visualizzati nelle nuove e-mail per impostazione predefinita. Questa funzione è molto più utile se stai creando un modello e-mail con un numero elevato di moduli.
* Sugli elementi immagine è ora possibile specificare se le proprietà &quot;height&quot; e &quot;width&quot; dell&#39;elemento HTML sottostante devono essere bloccate o modificabili per l&#39;utente finale. `<img>` mktoLockImgSize=&quot;true&quot; causerà il blocco di altezza/larghezza (anche se l&#39;immagine viene modificata). Analogamente, mktoLockImgStyle=&quot;true&quot; causerà il blocco della proprietà &quot;style&quot;.

**Ricerca codice**

Utilizza la nuova funzionalità di ricerca per trovare e sostituire in modo efficiente il contenuto all’interno del codice e-mail. Questa funzionalità è disponibile anche nell’editor dei modelli e-mail.

![](assets/2nd-screenshot.png)

**Supporto token negli elementi immagine**

Ora è possibile utilizzare i token nell’area &quot;External URL&quot; dell’esperienza di inserimento immagine. Se hai specificato immagini con `{{my.tokens}}`, ora puoi fare riferimento a questi token in Email Editor 2.0. Tieni presente che l’immagine risulterà ancora danneggiata nell’area di lavoro di Email Editor 2.0. Tuttavia, li vedrai renderizzati in Anteprima e Invia campione prima di inviare l’e-mail.

## Più domini di branding {#multiple-branding-domains}

Sono finiti i giorni in cui i collegamenti di tracciamento e-mail potevano essere contrassegnati con un solo dominio di branding. Ora puoi aggiungere più domini di branding per ispirare la fiducia dei consumatori, conferire un aspetto più semplice al brand, migliorare il recapito messaggi e-mail e scegliere, in base alle e-mail, quale dominio di branding utilizzare per i collegamenti di tracciamento di ogni e-mail.

![](assets/multiple-branding-domains.png)

## [Token programma](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) {#program-tokens}

È stato creato un nuovo tipo di token per i programmi. Ora puoi eseguire il rendering di Nome programma, Descrizione e ID nei passaggi di risorse e flusso di campagne intelligenti.

![](assets/program-tokens.png)

## [Chiave organizzazione](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/authorize-the-marketo-outlook-plugin.md) {#enterprise-key}

Richiedere a ogni persona nel team vendite di installare il plug-in [!DNL Sales Insight] per [!DNL Outlook] può essere noioso. È stato introdotto un nuovo modo per installare il plug-in per [!DNL Outlook] in remoto utilizzando una chiave Enterprise. Invia al tuo team IT la tua chiave univoca trovata nella sezione Marketo [!DNL Sales Insight] di [!UICONTROL Admin] e lascia fare il resto.

![](assets/enterprise-key.png)

## [Campagne Web Personalization](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) {#web-personalization-campaigns}

Specifica un ritardo nella reazione delle campagne web sul tuo sito web.

![](assets/dialog-campaign-delay.png)

## [Esportazione Content Analytics e consigli](/help/marketo/product-docs/web-personalization/understanding-web-personalization/understanding-content-analytics.md) {#content-analytics-and-recommendations-export}

Visualizzare i dati di analisi dei contenuti e consigli offline.

## [Supporto API per l&#39;editor e-mail 2.0](https://developers.marketo.com/documentation/asset-api/) {#api-support-for-email-editor}

Le API di Asset preesistenti, in precedenza compatibili solo con e-mail e modelli v1.0, ora sono abilitate per le risorse e-mail v2.0.

## [Sito sviluppatori Marketo](https://developers.marketo.com/) {#marketo-developers-site}

Nuovo e migliorato!

## [Impostazioni privacy](/help/marketo/product-docs/administration/settings/understanding-privacy-settings.md) {#privacy-settings}

Gli addetti al marketing possono utilizzare le impostazioni relative alla privacy per decidere se tenere traccia dei visitatori utilizzando le funzionalità di [!DNL Munchkin] e Web Personalization. Il livello di tracciamento è controllato utilizzando l’impostazione Do Not Track del browser, un cookie di rinuncia o un IP non specifico. Questi metodi possono influenzare il valore e le funzionalità di Marketo in aree specifiche, ma se l’addetto marketing non cambia nulla, le funzionalità di Marketo rimangono le stesse.

Questa funzione verrà rilasciata gradualmente ai clienti in un periodo di sei settimane. Se ne hai bisogno immediatamente, contatta il supporto Marketo.
