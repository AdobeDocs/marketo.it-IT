---
unique-page-id: 4720125
description: Integrare RTP con Google Universal Analytics - Marketo Docs - Documentazione prodotto
title: Integrare RTP con Google Universal Analytics
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---


# Integrare RTP con Google Universal Analytics {#integrate-rtp-with-google-universal-analytics}

## Introduzione {#intro}

Sfruttate Google Universal Analytics (GUA) con i dati di personalizzazione e personalizzazione in tempo reale (RTP) di Marketo per misurare e analizzare al meglio le attività di marketing online.

Questo post spiega come impostare e integrare la piattaforma Marketo Real-Time Personalization (RTP) con gli account Google Universal Analytics (GUA). I dati RTP possono essere aggiunti al tuo account GUA per consentirti di visualizzare e visualizzare le prestazioni di organizzazioni, industrie, elementi grafici e segmenti RTP presenti sul tuo sito Web.

**Google Universal Analytics**

Google Universal Analytics con i dati RTP offre una migliore comprensione di come gli utenti B2B interagiscono con i contenuti online e aiutano a misurare e ottenere risultati migliori dalle campagne di personalizzazione. [Ulteriori informazioni su Google Universal Analytics](https://support.google.com/analytics/answer/2790010/?hl=en&amp;authuser=1).

>[!NOTE]
>
>**Solo per utenti di Google Tag Manager**
>
>Non è necessario eseguire alcuna codifica o configurazione speciale. Completate il seguente elenco di controllo:
>
>* Le dimensioni RTP vengono create in Google Universal Analytics
>* [Il tag RTP è installato correttamente in Google Tag Manager](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* L&#39;integrazione di Google Universal Analytics è abilitata nelle impostazioni account della RTP
>* [Il tag Google Universal Analytics è configurato correttamente in Google Tag Manager](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* [Tag Google Tag Manager installato correttamente nel sito Web](https://developers.google.com/tag-manager/quickstart)


## Impostazione di Dimension personalizzati in GUA {#set-up-custom-dimensions-in-gua}

1. In Google Analytics,

   1. Vai a **Admin**
   1. Selezionare l&#39; **Account.**
   1. Selezionare la proprietà **.**
   1. Selezionare **Definizioni personalizzate** e **Dimension personalizzati**.
      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. Aggiungi una nuova dimensione personalizzata. Fare clic su **+Nuovo Dimension personalizzato**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. Aggiungere i seguenti Dimension **personalizzati:**

<table> 
 <tbody> 
  <tr> 
   <td><p><strong>Nome Dimension personalizzato</strong></p></td> 
   <td><p><strong>Ambito</strong></p></td> 
   <td><p><strong>Attivo</strong></p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Organization</strong></p></td> 
   <td><p>Sessione</p></td> 
   <td><p align="center">AND</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Industry</strong></p></td> 
   <td><p>Sessione</p></td> 
   <td><p align="center">AND</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Category</strong></p></td> 
   <td><p>Sessione</p></td> 
   <td><p align="center">AND</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Group</strong></p></td> 
   <td><p>Sessione</p></td> 
   <td><p align="center">AND</p></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**I** nomi degli Dimension personalizzati devono essere esattamente come definiti nella tabella precedente (altrimenti i dashboard e i rapporti RTP personalizzati in GUA non verranno visualizzati correttamente)

1. Aggiungete il **Nome**. Selezionare l&#39;ambito come **sessione**. Fare clic su **Crea**.

   ![](assets/image2014-11-29-11-3a12-3a51.png)

L&#39;elenco Dimension personalizzato dovrebbe essere simile al seguente.

![](assets/image2014-11-29-11-36-50-version-2.png)

Una volta attivati i Dimension personalizzati in GUA, andate alla piattaforma RTP per abilitare queste dimensioni all&#39;interno di RTP.

## Attivare l&#39;integrazione GUA nel proprio account RTP {#activate-the-gua-integration-in-your-rtp-account}

1. Nella piattaforma RTP, passare a **Impostazioni account.**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. In **Impostazioni account**, fare clic su **Dominio**.
1. In **Analytics** fare clic su **Google Universal Analytics**.
1. Ruotare **On** i Dimension e gli eventi personalizzati pertinenti per aggiungere questi dati da RTP a Google Universal Analytics.
1. Immettere il **numero di indice** della dimensione allineata con il numero di indice in GUA.
1. Fare clic su **Salva**.

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>Il numero di indice per il Dimension personalizzato si trova in GUA in Dimension personalizzati.
>
>Esempio: Numero indice RTP-Industry uguale a 1, Numero indice RTP-Organization uguale a 2.

## Rimuovere vecchie dashboard nelle Google Analytics {#remove-old-dashboards-in-google-analytics}

1. In Google Analytics. Vai a **Reporting.**
1. Fare clic su **Dashboard.**
1. Selezionare un **dashboard** (RTP B2B o RTP Performance)
1. Fare clic su **Elimina dashboard**.

![](assets/image2014-11-29-11-3a42-3a55.png)
