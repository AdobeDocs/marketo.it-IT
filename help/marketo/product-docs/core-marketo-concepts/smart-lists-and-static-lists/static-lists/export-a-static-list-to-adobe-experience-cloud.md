---
unique-page-id: 37356194
description: Esportazione di un elenco statico in Adobe Experience Cloud - Marketo Docs - Documentazione prodotto
title: Esportazione di un elenco statico in Adobe Experience Cloud
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---


# Esportazione di un elenco statico in Adobe Experience Cloud {#export-a-static-list-to-adobe-experience-cloud}

>[!NOTE]
>
>Una distribuzione HIPAA di un&#39;istanza di Marketo non può utilizzare questa funzione.

>[!PREREQUISITES]
>
>[Configurare la condivisione dell&#39;audience di Adobe Experience Cloud](http://docs.marketo.com/x/D4GMAg)

## Applicazioni di destinazione supportate {#supported-destination-applications}

* Adobe Advertising Cloud
*  Adobe Analytics (**solo** se si possiede una licenza Adobe Audience Manager)
* Adobe Audience Manager
* Adobe Experience Manager
* Piattaforma dati cliente in tempo reale  Adobe
*  Adobe Target

## Come esportare un elenco {#how-to-export-a-list}

1. In Marketo, trovate e selezionate l’elenco da esportare.

   ![](assets/one.png)

1. Fare clic sul menu a discesa **Azioni elenco** e selezionare **Invia a  Experience Cloud**.

   ![](assets/two-1.png)

1. Fare clic sul menu a discesa **cartella Audience Manager** e selezionare la cartella di destinazione desiderata nel Experience Cloud .

   ![](assets/three-1.png)

1. Scegliete se creare una nuova audience o sovrascriverne una esistente (in questo esempio ne stiamo creando una nuova). Immettete il nuovo nome del pubblico e fate clic su **Invia**.

   ![](assets/four.png)

1. Fare clic su **OK**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Possono essere necessarie fino a 6-8 ore prima che l&#39;iscrizione al pubblico venga compilata completamente nel  Adobe.

## Note {#things-to-note}

**Condivisione su  Adobe Analytics**

Per i clienti che possiedono sia Adobe Audience Manager che  Adobe Analytics, questa integrazione consentirà la condivisione dei tipi di pubblico da Marketo alle suite di rapporti Adobe Analytics , tuttavia, per attivare questa funzionalità è necessario effettuare alcune configurazioni aggiuntive in Adobe Audience Manager. Per ulteriori informazioni sulla configurazione, consulta la documentazione di Adobe Audience Manager: [https://docs.adobe.com/content/help/en/analytics/integration/audience-analytics/mc-audiences-aam.html](http://docs.adobe.com/content/help/en/analytics/integration/audience-analytics/mc-audiences-aam.html).

**Utilizzo delle caratteristiche per i clienti Adobe Audience Manager**

Quando avviate un&#39;esportazione di elenco in Marketo, noterete le seguenti modifiche che si riflettono nell&#39;istanza di Adobe Audience Manager:

* Per tutti i lead nell’elenco esportato, Marketo scriverà una caratteristica utilizzando i messaggi e-mail con hash dei lead come identificatore multi-dispositivo. Il nome della caratteristica corrisponderà al Nome pubblico di destinazione specificato durante l&#39;esportazione.
* Per tutti gli ECID che Marketo è riuscito a far corrispondere ai lead nell’elenco esportato, Marketo scriverà una caratteristica utilizzando l’identificatore dispositivo ECID. Il nome della caratteristica corrisponderà al Nome pubblico di destinazione specificato durante l&#39;esportazione.
* Marketo creerà anche un segmento nell’istanza di Audience Manager  utilizzando la caratteristica ECID come unico criterio di segmentazione. Il nome del segmento corrisponderà al Nome pubblico di destinazione specificato durante l’esportazione.

## Domande frequenti {#faq}

**Perché la dimensione dell&#39;elenco in Marketo è diversa da quella nel Adobe ?**

Sotto la cappa, l&#39;integrazione del pubblico funziona sincronizzando i cookie Marketo Munchkin con il cookie ECID del Adobe corrispondente. Marketo può condividere dati di appartenenza solo per i lead per i quali Marketo ha sincronizzato un ECID. Per ottenere i migliori risultati possibili, si consiglia di caricare lo script di tracciamento munchkin.js di Marketo in parallelo con  codice di tracciamento visitor.js del Adobe su tutte le pagine che si desidera tracciare a scopo di marketing.

**Come funziona la sincronizzazione dei cookie?**

Quando la sincronizzazione dei cookie è abilitata per l’iscrizione a Marketo, il file munchkin.js di Marketo tenterà di acquisire e memorizzare  ECID Adobe per l’organizzazione IMS del Adobe  specificata durante l’impostazione dell’integrazione e far corrispondere questi ECID al corrispondente identificatore di cookie Marketo. Questo consente ai profili utente anonimi di Marketo di arricchirsi con  ECID Adobe.

È necessario un ulteriore passaggio per associare il profilo utente anonimo a un profilo lead, identificato mediante un messaggio e-mail di testo normale. Esattamente come funziona questo è descritto qui: [https://docs.marketo.com/display/public/DOCS/Tracking+Anonymous+Activity+and+People](http://docs.marketo.com/display/public/DOCS/Tracking+Anonymous+Activity+and+People).
