---
unique-page-id: 4720796
description: Retargeting with Web Personalization Data - Marketo Docs - Documentazione del prodotto
title: Retargeting with Web Personalization Data
exl-id: b5af1f84-2061-4d0d-9d1f-2fff9191f028
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Retargeting with Web Personalization Data {#retargeting-with-web-personalization-data}

>[!AVAILABILITY]
>
>Il retargeting dei siti web ora rientra nella sezione Personalizzazione web . Se hai acquistato solo Retargeting, visualizzerai questo riquadro e accederai al prodotto di personalizzazione web con **only** Funzioni di retargeting abilitate. Questo consente di accedere alle impostazioni dell’account, alla pagina Retargeting, ai segmenti e alle pagine di tracciamento aggiuntive.

Il remarketing si rivolge ai potenziali clienti che hanno visitato il tuo sito in passato con display advertising basati su chi sono e cosa hanno fatto. Il retargeting personalizzato esegue il targeting di tipi di pubblico specifici con annunci pertinenti basati sul settore, account denominati e dati di persone note.

La personalizzazione web aggiunge attualmente dati alle seguenti piattaforme di remarketing:

* [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
* [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

La personalizzazione web invia i seguenti dati alle piattaforme di remarketing per creare tipi di pubblico ed eseguire campagne pubblicitarie di remarketing:

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">Dati di personalizzazione web</th> 
  </tr> 
  <tr> 
   <th><p>Settore</p></th> 
  </tr> 
  <tr> 
   <th><p>Gruppo (Enterprise, SMB)</p></th> 
  </tr> 
  <tr> 
   <th><p>Categoria (Fortune 500/1000, Global 2000)</p></th> 
  </tr> 
  <tr> 
   <th><p>Elenco ABM (Elenchi account denominati)</p></th> 
  </tr> 
  <tr> 
   <th><p>Pubblico segmentato (in base ai segmenti)</p></th> 
  </tr> 
  <tr> 
   <th><p>Campagne web selezionate</p></th> 
  </tr> 
 </tbody> 
</table>

## Configurazione del remarketing {#remarketing-configuration}

1. Vai a **Retargeting**.

   ![](assets/one.png)

   >[!NOTE]
   >
   >La configurazione di retargeting è per dominio o sottodominio. Attiva gli altri domini se desideri inviare dati da tali domini alla piattaforma di retargeting.

1. Attiva le impostazioni per Google Analytics o Google Universal Analytics per dominio.

   >[!NOTE]
   >
   >È necessario che il tag di retargeting di Google sia implementato sul sito web.
   >
   >Se si imposta già l&#39;integrazione con la personalizzazione Web e le Google Analytics, non è necessario modificare questa parte in quanto si tratta della stessa configurazione in Impostazioni account.

   ![](assets/two.png)

1. Attiva la configurazione per Facebook. Fai clic su ed espandi il pannello a soffietto Facebook, fai clic su **On** per inviare il rispettivo evento e i relativi dati ad Facebook Audience Manager. Fai clic su **Salva**.

   >[!NOTE]
   >
   >Devi [Pixel di pubblico personalizzati facebook](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)è stato installato il sito Web per il funzionamento di questa funzionalità.

   ![](assets/three.png)

## Creazione di un pubblico segmentato {#creating-segmented-audience}

Un pubblico segmentato consente di selezionare un segmento esistente come pubblico da utilizzare per le campagne di retargeting. Ad esempio, selezionando i segmenti di Persona nota .

>[!TIP]
>
>Non è necessario creare un pubblico segmentato per il settore o altri dati già inviati tramite nella configurazione del dominio. È consigliabile utilizzare Tipi di pubblico segmentati per segmenti basati su dati di persone note.

1. Fai clic su **Creare un pubblico segmentato**.

   ![](assets/image2015-1-15-16-3a36-3a38.png)

1. Immetti il Nome del pubblico, seleziona Canali e seleziona Segmento dall’elenco dei Segmenti esistenti.

   ![](assets/image2015-1-15-16-3a40-3a17.png)

1. Fai clic su **Salva**.

   Hai completato il programma di impostazione del retargeting in Personalizzazione web, accedi alle piattaforme di retargeting e crea i tuoi tipi di pubblico in base a questi dati e configura le tue campagne pubblicitarie di retargeting.
