---
unique-page-id: 6094890
description: Note sulla versione - Febbraio 2015 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Febbraio 2015
exl-id: a7ce88dc-a4d2-4ccb-9fe5-61130334d24d
feature: Release Information
TQID: https://experienceleague.adobe.com/IC-YEO8DuW1Y8bNWyUGo9EBp98dsmhZBOVOXmRBPFds
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: c954475c-8548-4e33-a0b8-6b550d956115id: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 338
ht-degree: 1%

---

# Note sulla versione - Febbraio 2015 {#release-notes-february}

Le seguenti funzioni sono incluse nella versione di febbraio 2015. Per informazioni sulla disponibilità delle funzioni, controllare la Marketo Edition. Dopo il rilascio, torna indietro per trovare i collegamenti agli articoli dettagliati per ogni funzione. Rullo di tamburo...

## Miglioramenti dell’automazione del marketing {#marketing-automation-enhancements}

**[Sposta campagna avanzata](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

Rallegratevi! Ora è possibile spostare le campagne intelligenti all’interno e all’esterno dei programmi tramite il trascinamento della selezione o la funzione Sposta nella struttura.

**[[!DNL Dynamics] 2015 (online)](https://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises)** - supportato.

**Modifiche al certificato HTTPS**

Per proteggere la riservatezza e l&#39;integrità dei dati dei clienti e dei servizi SaaS, Marketo segue le best practice del settore SaaS

e sostituirà i protocolli di sicurezza attualmente utilizzati (SHA-1 e SSL) con versioni più sicure (SHA-2 (alias SHA-256) e TLS) per i seguenti domini:

* marketo.net (traffico [!DNL Munchkin] crittografato)

* [marketo.com](https://marketo.com) (principali applicazioni SaaS)

Ciò avverrà poco dopo questa versione. Il protocollo SHA-1 verrà temporaneamente supportato sul dominio [mktoapi.com](https://mktoapi.com) fino a dicembre 2015 per consentire ai proprietari di sistemi e applicazioni legacy di aggiornare i propri sistemi con compatibilità SHA-2.

**Proteggi[!DNL Munchkin]**

È in corso la rimozione del supporto per SSL3. Abbiamo mantenuto SSL3 fino ad ora per mantenere il supporto per i vecchi browser web, ma nel 2015 non vediamo più traffico web significativo da questi browser. Questo influisce solo su [!DNL Munchkin] se utilizzato su pagine sicure e verrà distribuito lentamente dopo la versione di febbraio.

## Miglioramenti di Real-Time Personalization {#real-time-personalization-enhancements}

**[URL di destinazione per campagne](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

Seleziona le pagine da visualizzare per la campagna in tempo reale utilizzando &quot;Aggiungi un URL di destinazione&quot;. Questa funzione funziona con tutti i tipi di campagna (Finestra di dialogo, Nella zona, Widget), ma è particolarmente utile per le campagne Nella zona in cui una campagna eseguirà il rendering nell’ID zona per solo l’URL di destinazione selezionato. Supporta l’aggiunta di più URL per il targeting di pagine web diverse.

![](assets/image2015-2-19-11-3a0-3a30.png)

**Paese e stato aggiunti al targeting basato sull&#39;account**

È ora possibile aggiungere il paese e lo stato agli elenchi degli account denominati. Eseguire il targeting di potenziali account chiave da posizioni specifiche.
