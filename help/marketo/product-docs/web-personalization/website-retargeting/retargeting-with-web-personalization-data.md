---
unique-page-id: 4720796
description: Retargeting con dati di personalizzazione Web - Documenti Marketo - Documentazione prodotto
title: Ritargeting con dati di personalizzazione Web
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---


# Ritargeting con dati di personalizzazione Web {#retargeting-with-web-personalization-data}

>[!AVAILABILITY]
>
>Il retargeting dei siti Web ora si trova nella sezione Personalizzazione Web. Se avete acquistato solo Retargeting, visualizzerete questa sezione e accederete al prodotto Web Personalization con le funzioni di **solo** Retargeting abilitate. Questo consente di accedere alle impostazioni dell’account, alla pagina Retargeting, ai segmenti e alle pagine di tracciamento aggiuntive.

Notizie si rivolge ai potenziali clienti che hanno visitato il tuo sito in passato con una pubblicità basata su chi sono e cosa hanno fatto. Il retargeting personalizzato si rivolge a audience specifiche con annunci pertinenti basati su settori, account denominati e dati di persone conosciute.

Web Personalization attualmente aggiunge i dati alle seguenti piattaforme di remarketing:

* [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
* [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

Web Personalization invia i seguenti dati alle piattaforme di remarketing per creare audience ed eseguire campagne di remarketing:

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">Dati di personalizzazione Web</th> 
  </tr> 
  <tr> 
   <th><p>Industria</p></th> 
  </tr> 
  <tr> 
   <th><p>Gruppo (Enterprise, SMB)</p></th> 
  </tr> 
  <tr> 
   <th><p>Categoria (Fortune 500/1000, Global 2000)</p></th> 
  </tr> 
  <tr> 
   <th><p>Elenco ABM (Elenchi Account Denominati)</p></th> 
  </tr> 
  <tr> 
   <th><p>Audience segmentata (in base ai segmenti)</p></th> 
  </tr> 
  <tr> 
   <th><p>Campagne Web selezionate</p></th> 
  </tr> 
 </tbody> 
</table>

## Configurazione della notazione {#remarketing-configuration}

1. Vai a **Retargeting**.

   ![](assets/one.png)

   >[!NOTE]
   >
   >La configurazione di retargeting è per dominio o sottodominio. Attivate gli altri domini se desiderate inviare i dati da tali domini alla piattaforma di retargeting.

1. Attiva le impostazioni per Google Analytics o Google Universal Analytics per dominio.

   >[!NOTE]
   >
   >È necessario che Google Retargeting Tag sia implementato sul sito Web.
   >
   >Se hai già configurato l&#39;integrazione con la personalizzazione Web e le Google Analytics, non devi modificare questa parte perché è la stessa configurazione in Impostazioni account.

   ![](assets/two.png)

1. Attivate la configurazione per Facebook. Fate clic su e espandete la struttura di navigazione Facebook, fate clic su **On** per inviare i rispettivi eventi e dati al Audience Manager  Facebook. Fare clic su **Salva**.

   >[!NOTE]
   >
   >Affinché questa funzione funzioni funzioni, è necessario che sul sito Web sia installato [Facebook Custom Audience Pixel](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)di Facebook.

   ![](assets/three.png)

## Creazione di audience segmentata {#creating-segmented-audience}

Un pubblico segmentato consente di selezionare un segmento esistente come audience da utilizzare per le campagne di retargeting. Ad esempio, seleziona i segmenti Persona nota.

>[!TIP]
>
>Non è necessario creare un pubblico segmentato per il settore o altri dati già inviati tramite in Configurazione dominio. È consigliabile utilizzare Audience segmentate per segmenti basati su dati di persone note.

1. Fate clic su **Crea pubblico segmentato**.

   ![](assets/image2015-1-15-16-3a36-3a38.png)

1. Immettete Nome audience, selezionate Canali, quindi Segmento dall&#39;elenco dei Segmenti esistenti.

   ![](assets/image2015-1-15-16-3a40-3a17.png)

1. Fare clic su **Salva**.

   È stata completata l&#39;impostazione di retargeting in Web Personalization (Personalizzazione Web), è possibile accedere alle piattaforme di retargeting e creare il pubblico in base a tali dati e impostare le campagne di retargeting.
