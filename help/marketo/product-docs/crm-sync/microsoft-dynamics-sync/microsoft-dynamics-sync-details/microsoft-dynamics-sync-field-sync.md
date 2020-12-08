---
unique-page-id: 3571838
description: Microsoft Dynamics Sync -Field Sync - Marketo Docs - Documentazione prodotto
title: Microsoft Dynamics Sync - Sincronizzazione campi
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Sincronizzazione campo {#microsoft-dynamics-sync-field-sync}

>[!NOTE]
>
>**FYI**
>
>Marketo sta ora standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che l&#39;iscrizione contenga lead/lead e la persona/persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

La sincronizzazione tra Marketo e Dynamics è super potente. Ecco i dettagli.

## Come vengono mantenuti sincronizzati i dettagli del campo tra i due sistemi? {#how-are-field-details-kept-in-sync-between-the-two-systems}

La sincronizzazione è bidirezionale per le entità lead e contatto. Se apporti modifiche a un lead o a un contatto in Dynamics o a una persona in Marketo, gli aggiornamenti si rifletteranno su entrambi i sistemi.

Per le entità account, utente, opportunità, team e personalizzate, la sincronizzazione è unidirezionale: Dinamica a Marketo. Se apporti modifiche a queste entità in Dynamics, gli aggiornamenti si rifletteranno su Marketo.

## Cosa succede se nello stesso campo vengono apportate modifiche contemporaneamente in entrambi i sistemi? (Collisione dati) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Anche se questo è raro, Marketo vincerà per le persone (lead) e Dynamics vincerà per i contatti. Questo perché riteniamo che il reparto marketing sia autorevole per le persone, mentre il sistema ufficiale di registrazione dei contatti è nel reparto vendite (CRM). Per le entità di sincronizzazione unidirezionale, Dynamics vincerà sempre.

## Posso creare un campo in Dynamics utilizzando Marketo? {#can-i-create-a-field-in-dynamics-using-marketo}

No, al momento non è supportato.

## Ho creato un campo in Dynamics. Posso sincronizzarlo con Marketo? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Sì, è possibile [sincronizzare il campo](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) finché l&#39;utente sincronizzato ha accesso ad esso in Dynamics.

Quali campi verranno sincronizzati con Marketo?

Potete [selezionare i campi da sincronizzare](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) durante l&#39;impostazione.

## Cosa succede se devo aggiungere un campo personalizzato dopo che Marketo e Dynamics sono stati sincronizzati? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

Puoi aggiungere campi in qualsiasi momento e prevedere che i dati saranno aggiornati da Dynamics a Marketo. Per ulteriori informazioni, consulta [Utilizzare la sincronizzazione rapida con Microsoft Dynamics per un nuovo campo](microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md) personalizzato.

>[!NOTE]
>
>**Articoli correlati**
>
>* [Usa sincronizzazione rapida con Microsoft Dynamics per un nuovo campo personalizzato](microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md)

>



