---
unique-page-id: 4720125
description: Integrare RTP con Google Universal Analytics - Documenti Marketo - Documentazione del prodotto
title: Integrare RTP con Google Universal Analytics
exl-id: e8fc8730-c91d-44ad-8843-aa5b38f1ebd1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---

# Integrare RTP con Google Universal Analytics {#integrate-rtp-with-google-universal-analytics}

## Introduzione {#intro}

Sfrutta i dati di personalizzazione e firmware di Google Universal Analytics (GUA) con Marketo Real-Time Personalization (RTP) per misurare e analizzare al meglio le tue attività di marketing online.

Questo post spiega come configurare e integrare la piattaforma Marketo Real-Time Personalization (RTP) con gli account Google Universal Analytics (GUA). I dati RTP possono essere aggiunti al tuo account GUA per consentirti di visualizzare e visualizzare le prestazioni di organizzazioni, industrie, aziende e segmenti RTP che visitano il tuo sito web.

**Google Universal Analytics**

Google Universal Analytics con i dati di RTP offre una migliore comprensione di come gli utenti B2B interagiscono con i contenuti online e aiuta a misurare e ottenere risultati migliori dalle campagne di personalizzazione. [Ulteriori informazioni su Google Universal Analytics](https://support.google.com/analytics/answer/2790010/?hl=en&amp;authuser=1).

>[!NOTE]
>
>**Solo per utenti di Google Tag Manager**
>
>Non è necessario eseguire alcuna codifica o configurazione speciale. Assicurati di completare la seguente lista di controllo:
>
>* Le dimensioni RTP vengono create in Google Universal Analytics.
>* [Il tag RTP è installato correttamente in Google Tag Manager](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* L’integrazione Google Universal Analytics è abilitata nelle impostazioni account della RTP
>* [Il tag Google Universal Analytics è configurato correttamente in Google Tag Manager](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* [Il tag Google Tag Manager è installato correttamente nel sito Web](https://developers.google.com/tag-manager/quickstart)


## Configurazione di Dimension personalizzati in GUA {#set-up-custom-dimensions-in-gua}

1. In Google Analytics,

   1. Vai a **Amministratore**
   1. Seleziona la **Conto.**
   1. Seleziona la **Proprietà.**
   1. Seleziona **Definizioni personalizzate** e **Dimension personalizzati**.
      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. Aggiungi una nuova dimensione personalizzata. Fai clic su **+Nuovo Dimension personalizzato**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. Aggiungi quanto segue **Dimension personalizzati:**

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
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Industry</strong></p></td> 
   <td><p>Sessione</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>Categoria RTP</strong></p></td> 
   <td><p>Sessione</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>Gruppo RTP</strong></p></td> 
   <td><p>Sessione</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**Nomi di Dimension personalizzati** deve essere esattamente come definito nella tabella precedente (in caso contrario le dashboard e i rapporti personalizzati RTP in GUA non verranno visualizzati correttamente)

1. Aggiungi il **Nome**. Seleziona l&#39;ambito come **Sessione**. Fai clic su **Crea**.

   ![](assets/image2014-11-29-11-3a12-3a51.png)

L&#39;elenco dei Dimension personalizzati dovrebbe essere simile al seguente.

![](assets/image2014-11-29-11-36-50-version-2.png)

Una volta attivati i Dimension personalizzati in GUA, vai alla piattaforma RTP per abilitare queste dimensioni all’interno di RTP.

## Attivare l’integrazione GUA nel tuo account RTP {#activate-the-gua-integration-in-your-rtp-account}

1. Nella piattaforma RTP, vai a **Impostazioni account.**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. Sotto **Impostazioni account**, fai clic su **Dominio**.
1. Sotto **Analytics**, fai clic su **Google Universal Analytics**.
1. Girare **On** i Dimension personalizzati e gli eventi pertinenti per aggiungere questi dati da RTP a Google Universal Analytics.
1. Inserisci il **Numero indice** della dimensione allineata con il numero di indice in GUA.
1. Fai clic su **Salva**.

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>Il numero di indice per il Dimension personalizzato si trova in GUA in Dimension personalizzati.
>
>Esempio: Numero indice RTP-Industry è uguale a 1, Numero indice RTP-Organization è uguale a 2.

## Rimuovere le vecchie dashboard nelle Google Analytics {#remove-old-dashboards-in-google-analytics}

1. In Google Analytics. Vai a **Generazione rapporti.**
1. Fai clic su **Dashboard.**
1. Seleziona una **Dashboard** (Prestazioni RTP B2B o RTP)
1. Fai clic su **Elimina dashboard**.

![](assets/image2014-11-29-11-3a42-3a55.png)
