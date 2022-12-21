---
unique-page-id: 11380218
description: Note sulla versione - Estate 16 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Estate 16
exl-id: 3843668e-c729-42aa-b05c-55c33ee0d783
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 0%

---

# Note sulla versione: Estate &#39;16 {#release-notes-summer}

Le seguenti funzionalità sono incluse nella versione del 16 estate. Per informazioni sulla disponibilità delle funzioni, consulta la tua edizione Marketo . Fai clic sui collegamenti del titolo per visualizzare gli articoli dettagliati per ciascuna funzione.

## [Marketing basato su account](https://docs.marketo.com/display/docs/account+based+marketing) {#account-based-marketing}

Il marketing basato su account Marketo offre tutti gli elementi essenziali in un&#39;unica piattaforma unificata:

* **Target** - Individuazione account, abbinamento lead-to-account ed elenchi di account denominati
* **Coinvolgi** - Personalizzazione basata su account, coinvolgimento cross-channel e flussi di lavoro specifici per l’account
* **Misura** - Approfondimenti a livello di account ed elenco, punteggio di coinvolgimento dell&#39;account e impatto sulla pipeline e sui ricavi

![](assets/abm-5-acme.png)

>[!NOTE]
>
>ABM è disponibile come componente aggiuntivo del tuo abbonamento Marketo, quindi contatta il tuo rappresentante commerciale per implementarlo.

## [Audit Trail](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md) {#audit-trail}

Audit trail fornisce una cronologia completa delle modifiche apportate all’interno dell’abbonamento Marketo. Creerà responsabilità tra utenti e amministratori, aiuterà a identificare la causa di un comportamento imprevisto e fornirà la sicurezza di sapere chi sta facendo cosa e quando. Queste informazioni saranno disponibili in qualsiasi momento e possono essere utilizzate per rispondere a domande quali:

* Cos’è successo a questa risorsa o impostazione e chi l’ha aggiornata per ultimo?
* Fino a che punto è l&#39;utente X?
* Chi effettua l&#39;accesso al nostro account?

![](assets/audit-trail.png)

## [Integrazione di Marketo-Vibes SMS LaunchPoint](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md) {#marketo-vibes-sms-launchpoint-integration}

Crea facilmente messaggi SMS direttamente in Marketo. Personalizza ed esegui il targeting del messaggio utilizzando i tuoi dati Marketo avanzati e monitorane facilmente le prestazioni utilizzando il dashboard dei messaggi SMS.

>[!NOTE]
>
>Questa funzione richiede l’esistenza di un account SMS Vibes.

![](assets/vibes-sms2.png)

## [Miglioramenti a E-mail 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-enhancements}

**Variabili a livello di modulo**

Precedentemente, tutte le variabili specificate nei modelli Email 2.0 erano &quot;globali&quot; nell’ambito. Quando si utilizzano variabili all’interno dei moduli, questo non è sempre opportuno se si prevede di utilizzare più istanze del modulo. Con questa versione, le variabili possono ora essere specificate come &quot;livello di modulo&quot;, il che ti consente di indicare che l’utente deve essere in grado di impostare valori univoci per ciascun modulo in cui viene utilizzato.

![](assets/module-level-variables.png)

**Aggiornamenti della sintassi**

* È ora possibile utilizzare &quot;mktoAddByDefault&quot; sui moduli specificati nei modelli di e-mail 2.0 per indicare quali moduli devono essere visualizzati nelle nuove e-mail per impostazione predefinita. Questo è molto più conveniente se si sta creando un modello e-mail con un gran numero di moduli.
* Negli elementi immagine è ora possibile specificare se il sottostante `<img>` Le proprietà &quot;height&quot; e &quot;width&quot; dell’elemento HTML devono essere bloccate o modificabili per l’utente finale. mktoLockImgSize=&quot;true&quot; blocca l&#39;altezza/larghezza (anche se l&#39;immagine viene modificata). Analogamente, mktoLockImgStyle=&quot;true&quot; blocca la proprietà &quot;style&quot;.

**Ricerca del codice**

Utilizza la nuova funzionalità di ricerca per trovare e sostituire in modo efficiente il contenuto all’interno del codice dell’e-mail. Questa funzionalità è disponibile anche nell’editor modelli e-mail .

![](assets/2nd-screenshot.png)

**Supporto token negli elementi immagine**

I token possono ora essere utilizzati nell’area &quot;External URL&quot; dell’esperienza di inserimento immagine. Se hai specificato immagini con `{{my.tokens}}`, è ora possibile fare riferimento a questi token all’interno di E-mail Editor 2.0. L’immagine continuerà a essere danneggiata nell’area di lavoro di E-mail Editor 2.0. Tuttavia, potrai visualizzarli in Anteprima e invia campione prima di inviare il tuo messaggio e-mail.

## Più domini di branding {#multiple-branding-domains}

Sono finiti i giorni in cui i collegamenti di tracciamento e-mail potevano essere contrassegnati con un solo dominio di branding. Ora puoi aggiungere più domini di branding per ispirare la fiducia dei consumatori, creare un look più semplice da mettere a fuoco sul marchio, migliorare il recapito dei messaggi e-mail e scegliere, in base alle e-mail, quale dominio di branding utilizzare per i collegamenti di tracciamento di ogni e-mail.

![](assets/multiple-branding-domains.png)

## [Token del programma](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) {#program-tokens}

È stato creato un nuovo tipo di token per i programmi. Ora puoi eseguire il rendering di Nome programma, Descrizione e ID nelle risorse e nei passaggi del flusso di campagne avanzate.

![](assets/program-tokens.png)

## [Chiave aziendale](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/authorize-the-marketo-outlook-plugin.md) {#enterprise-key}

Richiedere a ogni persona del tuo team di vendita di installare il nostro plugin Insight di vendita per Outlook può essere noioso. Abbiamo introdotto un nuovo modo per installare il plugin per Outlook in remoto utilizzando una chiave aziendale. Invia al tuo team IT la tua chiave unica trovata nella sezione Marketo Sales Insight di Admin e lascia che faccia il resto.

![](assets/enterprise-key.png)

## [Campagne di personalizzazione web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) {#web-personalization-campaigns}

Specifica un ritardo per le campagne web da cui reagire sul sito web.

![](assets/dialog-campaign-delay.png)

## [Analisi dei contenuti ed esportazione Recommendations](/help/marketo/product-docs/web-personalization/understanding-web-personalization/understanding-content-analytics.md) {#content-analytics-and-recommendations-export}

Visualizzare i dati di analisi dei contenuti e consigli offline.

## [Supporto API per Email Editor 2.0](https://developers.marketo.com/documentation/asset-api/) {#api-support-for-email-editor}

Le API di risorse preesistenti, precedentemente compatibili solo con e-mail e modelli v1.0, sono ora abilitate per le risorse e-mail v2.0.

## [Sito per sviluppatori Marketo](https://developers.marketo.com/) {#marketo-developers-site}

Novità e miglioramenti!

## [Impostazioni privacy](/help/marketo/product-docs/administration/settings/understanding-privacy-settings.md) {#privacy-settings}

Gli addetti al marketing possono utilizzare le impostazioni sulla privacy per decidere se tenere traccia dei visitatori utilizzando Munchkin e le funzioni di personalizzazione web. Il livello di tracciamento è controllato utilizzando l’impostazione Do Not Track del browser, un cookie di rinuncia o un IP non specifico. Questi metodi possono influenzare il valore e la funzionalità di Marketo in aree specifiche, ma se l’addetto al marketing non apporta modifiche, la funzionalità di Marketo rimane la stessa.

Questa funzione verrà rilasciata gradualmente ai clienti in un periodo di sei settimane. Se necessario, contatta il supporto Marketo.
