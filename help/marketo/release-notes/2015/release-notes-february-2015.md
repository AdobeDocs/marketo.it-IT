---
unique-page-id: 6094890
description: Note sulla versione - Febbraio 2015 - Marketo Docs - Documentazione prodotto
title: Note sulla versione - febbraio 2015
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 0%

---


# Note sulla versione: Febbraio 2015 {#release-notes-february}

Le seguenti funzionalità sono incluse nella release di febbraio 2015. Per informazioni sulla disponibilità delle funzionalità, consulta la versione di Marketo Edition. Dopo il rilascio, accertatevi di tornare indietro per trovare i collegamenti agli articoli dettagliati per ciascuna funzione. Rullo del tamburo...

## Miglioramenti dell&#39;automazione marketing {#marketing-automation-enhancements}

** [Sposta campagna intelligente](../../product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)*

Felice! Ora puoi spostare le campagne intelligenti all&#39;interno e all&#39;esterno dei programmi tramite trascinamento o la funzione Sposta nella struttura.

** [Dynamics 2015 (online)](https://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises) **- supportato!

**Modifiche al certificato HTTPS**

Per proteggere la riservatezza e l&#39;integrità dei dati dei clienti e dei servizi SaaS, Marketo segue le best practice del settore SaaS

e sostituirà i protocolli di sicurezza attualmente utilizzati (SHA-1 e SSL) con versioni più sicure (SHA-2 (alias SHA-256) e TLS) per i seguenti domini:

`·` [marketo.net](https://marketo.net) (traffico Munchkin crittografato)

`·` [marketo.com](https://marketo.com) (principali applicazioni SaaS)

Ciò si verificherà poco dopo questa versione. Il protocollo SHA-1 sarà temporaneamente supportato su [mktoapi.com](https://mktoapi.com) dominio fino a dicembre 2015 per consentire ai proprietari di sistemi e applicazioni legacy di aggiornare i propri sistemi con la compatibilità SHA-2.

**Munchkin sicuro**

Stiamo rimuovendo il supporto per SSL3. Abbiamo mantenuto SSL3 fino ad ora per mantenere il supporto per i vecchi browser Web, ma nel 2015 non vediamo più traffico web significativo da questi browser. Questo interesserebbe Munchkin solo se utilizzato su pagine sicure, e verrà implementato lentamente dopo il rilascio di febbraio.

## Miglioramenti della personalizzazione in tempo reale {#real-time-personalization-enhancements}

** [URL di destinazione per campagne](../../product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

Selezionate le pagine sulle quali desiderate visualizzare la campagna in tempo reale utilizzando l&#39;opzione &quot;Aggiungi un URL di destinazione&quot;. Questa funzione funziona con tutti i tipi di campagne (finestra di dialogo, area, widget), ma è particolarmente utile per le campagne In Zone, dove una campagna verrà rappresentata nell’ID di zona solo per l’URL di destinazione selezionato. Supporta l’aggiunta di più URL per diverse pagine Web.

![](assets/image2015-2-19-11-3a0-3a30.png)

** [Paese e stato aggiunti al targeting basato su account](https://docs.marketo.com/display/DOCS/View+a+Named+Account+List)**

È ora possibile aggiungere Paese e Stato agli elenchi degli account denominati. Esegue il targeting dei potenziali account chiave da posizioni specifiche.
