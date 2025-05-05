---
unique-page-id: 4720758
description: Note sulla versione -Gennaio 2015 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Gennaio 2015
exl-id: f312ff87-6ac1-4167-be98-76600bb4b3cd
feature: Release Information
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Note sulla versione: gennaio 2015 {#release-notes-january}

Le seguenti funzioni sono incluse nella versione di gennaio 2015. Per informazioni sulla disponibilità delle funzioni, controllare la Marketo Edition. Dopo il rilascio, torna indietro per trovare i collegamenti agli articoli dettagliati per ogni funzione.

## Aggiornamenti di Marketing Automation {#marketing-automation-updates}

**Pagine Di Destinazione Per Dispositivi Mobili**

Ora puoi [creare visualizzazioni per dispositivi mobili per le pagine di destinazione](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md) dall&#39;editor delle pagine di destinazione. Distribuisci il messaggio in modo efficace indipendentemente dal dispositivo e aumenta il coinvolgimento personalizzando i contenuti per facilitarne l’utilizzo in movimento. Questa funzione verrà implementata gradualmente nel corso della settimana successiva al rilascio.

Video introduttivo sulla pagina di destinazione [-](https://youtu.be/aPQHlG2X6c0)

**Nuove chiamate API REST**

Tre nuove chiamate per l’API ReST per lead e attività:

* Elimina lead
* Ottieni lead per ID programma
* Ottieni lead eliminati

Inoltre, è disponibile una nuova opzione per Lead di sincronizzazione, che consente di scrivere la modifica del lead in modo asincrono per una chiamata API più veloce. I dettagli completi saranno disponibili dopo il rilascio all&#39;indirizzo [https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/home](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/home)

**Supporto Oggetto Personalizzato Script E-Mail**

Ora puoi accedere agli oggetti personalizzati associati all’oggetto Account dall’interno degli script e-mail.

## Real-Time Personalization {#real-time-personalization}

**Remarketing personalizzato per Google e Facebook**

Il remarketing mostra annunci a persone che hanno visitato il tuo sito web. Ora puoi personalizzare le campagne di remarketing in [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md) e [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md) utilizzando i dati di Real-Time Personalization. Rivolgiti a tipi di pubblico di diversi settori, elenchi di account denominati, dimensioni dell’azienda o qualsiasi dato proveniente da lead noti.

[Modulo elenco account denominati](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

I miglioramenti al modulo Account denominati miglioreranno le percentuali di corrispondenza e le convalide per gli utenti. Le aggiunte includono:

* Associare le organizzazioni dall’elenco Account denominato utilizzando l’indirizzo e-mail del lead (anche per i clienti solo RTP)
* Supporto per un massimo di 100.000 record per account
* Modello di file CSV da visualizzare e scaricare

![](assets/image2015-1-14-11-3a12-3a16.png)

**Opzioni tag RTP aggiornate**

Le opzioni dei tag RTP in Impostazioni account sono state aggiornate per includere:

1. CDN e asincrono (tag consigliato)
1. CDN e sincrono (alta velocità)
1. Tag asincrono senza CDN
1. Tag sincrono senza CDN

Per ottenere prestazioni ottimali, si consiglia di posizionare il tag nella parte superiore dell&#39;intestazione della pagina Web dopo `<head>`. Tutti i tag consentono l&#39;utilizzo dell&#39;[API RTP](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/javascriptapi/rich-media-recommendation). Per informazioni su come distribuire il tag RTP, vedi [qui](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

![](assets/image2015-1-15-13-3a30-3a45.png)
