---
unique-page-id: 4720758
description: Note sulla versione - Gennaio 2015 - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione - Gennaio 2015
exl-id: f312ff87-6ac1-4167-be98-76600bb4b3cd
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 0%

---

# Note sulla versione: Gennaio 2015 {#release-notes-january}

Le seguenti funzionalità sono incluse nella versione di gennaio 2015. Per informazioni sulla disponibilità delle funzioni, controlla la tua Marketo Edition. Dopo il rilascio, assicurati di tornare a trovare i collegamenti agli articoli dettagliati per ogni funzione!

## Aggiornamenti dell&#39;automazione di marketing {#marketing-automation-updates}

**Pagine di destinazione compatibili con i dispositivi mobili**

Ora è possibile [creare visualizzazioni mobili per le pagine di destinazione](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md) dall’interno dell’editor delle pagine di destinazione. Distribuisci il messaggio in modo efficace indipendentemente dal dispositivo e aumenta il coinvolgimento adattando i contenuti per un facile utilizzo on-the-go. Questa funzione verrà implementata gradualmente durante tutta la settimana successiva al rilascio.

[- Video introduttivo sulla pagina di destinazione](https://youtu.be/aPQHlG2X6c0)

**Nuove chiamate API Rest**

Tre nuove chiamate per l’API Lead &amp; Activity ReST:

* Elimina lead
* Ottieni lead per ID programma
* Recupera lead eliminati

Inoltre, esiste una nuova opzione per Sync Lead, per scrivere la modifica del lead in modo asincrono per una chiamata API più veloce. I dettagli completi saranno disponibili dopo la versione all&#39;indirizzo [developers.marketo.com](https://developers.marketo.com)

**Supporto per oggetti personalizzati con script e-mail**

Accedi ora agli oggetti personalizzati associati all’oggetto Account dall’interno degli script e-mail.

## Personalizzazione in tempo reale {#real-time-personalization}

**Remarketing personalizzato per Google e Facebook**

Il remarketing mostra gli annunci alle persone che hanno visitato il tuo sito web. Ora puoi personalizzare le campagne di remarketing su [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md) e [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md) utilizzando i dati della personalizzazione in tempo reale. Osservazioni a tipi di pubblico di settori diversi, elenchi di account denominati, dimensioni aziendali o qualsiasi dato proveniente da lead noti.

[Modulo elenco account denominato](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

I miglioramenti al modulo Account denominati miglioreranno i tassi di corrispondenza e le convalide per gli utenti. Le aggiunte includono:

* Organizzazioni corrispondenti dall’elenco Account con nome utilizzando l’indirizzo e-mail del lead (anche per i clienti con solo RTP)
* Supporto fino a 100.000 record per account
* Modello di file CSV da visualizzare e scaricare

![](assets/image2015-1-14-11-3a12-3a16.png)

**Opzioni di tag RTP aggiornate**

Le opzioni di tag RTP in Impostazioni account sono state aggiornate per includere:

1. CDN e asincrono (tag consigliato)
1. CDN e sincrono (alta velocità)
1. Tag asincrono senza CDN
1. Tag sincrono senza CDN

Per ottenere le migliori prestazioni, è consigliabile posizionare il tag nella parte superiore dell’intestazione nella pagina web dopo `<head>`. Tutti i tag consentono l’utilizzo dell’ [API RTP](https://developers.marketo.com/documentation/websites/rtp-js-api/). Per informazioni su come distribuire il tag RTP, vedi [qui](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

![](assets/image2015-1-15-13-3a30-3a45.png)
