---
unique-page-id: 4720758
description: Note sulla versione -Gennaio 2015 - Documenti Marketo - Documentazione prodotto
title: Note sulla versione - gennaio 2015
translation-type: tm+mt
source-git-commit: 029d8b419ba5078980b4fde9890bdb35194bf264
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 0%

---


# Note sulla versione: Gennaio 2015 {#release-notes-january}

Le seguenti funzionalità sono incluse nella release di gennaio 2015. Per informazioni sulla disponibilità delle funzionalità, consulta la versione di Marketo Edition. Dopo il rilascio, accertatevi di tornare indietro per trovare i collegamenti agli articoli dettagliati per ogni funzione!

## Aggiornamenti di Marketing Automation {#marketing-automation-updates}

**Pagine di destinazione intuitive per dispositivi mobili**

Ora è possibile [creare visualizzazioni mobili per le pagine di destinazione](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md) dall&#39;editor della pagina di destinazione. Distribuite i vostri messaggi in modo efficace indipendentemente dal dispositivo e aumentate il coinvolgimento personalizzando i vostri contenuti per un facile consumo in movimento. Questa funzione verrà implementata gradualmente per tutta la settimana successiva al rilascio.

[- Video introduttivo sulla pagina di destinazione](https://youtu.be/aPQHlG2X6c0)

**Nuove chiamate API Rest**

Tre nuove chiamate per l&#39;API Lead &amp; Activity ReST:

* Elimina lead
* Ottieni lead per ID programma
* Ottieni lead eliminati

Inoltre, esiste una nuova opzione per Sinc. lead, per scrivere la modifica del lead in modo asincrono per una chiamata API più veloce. I dettagli completi saranno disponibili dopo il rilascio all&#39;indirizzo [developers.marketo.com](https://developers.marketo.com)

**Supporto per oggetti personalizzati con script e-mail**

Ora è possibile accedere agli oggetti personalizzati associati all&#39;oggetto Account direttamente dagli script e-mail.

## Personalizzazione in tempo reale {#real-time-personalization}

**Osservazioni personalizzate per Google e Facebook**

Notizie mostra annunci a persone che hanno visitato il tuo sito Web. Ora puoi personalizzare le campagne di remarketing su [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md) e [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md) utilizzando i dati di Real-Time Personalization (Personalizzazione in tempo reale). Notizie a tipi di pubblico provenienti da settori diversi, elenchi di account denominati, dimensioni aziendali o qualsiasi dato proveniente da lead noti.

[Modulo elenco account denominato](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

I miglioramenti al modulo Account denominati miglioreranno i tassi di corrispondenza e le convalide per gli utenti. Le aggiunte includono:

* Corrispondenza delle organizzazioni dall’elenco Account denominato utilizzando l’indirizzo e-mail del lead (anche per i clienti con solo RTP)
* Supporto fino a 100.000 record per account
* Modello di file CSV da visualizzare e scaricare

![](assets/image2015-1-14-11-3a12-3a16.png)

**Opzioni tag RTP aggiornate**

Le opzioni dei tag RTP in Impostazioni account sono state aggiornate per includere:

1. CDN e asincrono (tag consigliato)
1. CDN e sincrono (alta velocità)
1. Tag asincrono senza CDN
1. Tag sincrono senza CDN

Per ottenere migliori prestazioni, si consiglia di posizionare il tag nella parte superiore dell&#39;intestazione nella pagina Web dopo `<head>`. Tutti i tag consentono l&#39;utilizzo dell&#39;API [RTP](https://developers.marketo.com/documentation/websites/rtp-js-api/). Per informazioni su come distribuire il tag RTP, vedere [qui](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

![](assets/image2015-1-15-13-3a30-3a45.png)
