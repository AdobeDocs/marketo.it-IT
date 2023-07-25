---
unique-page-id: 4720796
description: Retargeting con dati di personalizzazione web - Documenti Marketo - Documentazione del prodotto
title: Retargeting con dati di personalizzazione web
exl-id: b5af1f84-2061-4d0d-9d1f-2fff9191f028
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Retargeting con dati di personalizzazione web {#retargeting-with-web-personalization-data}

>[!AVAILABILITY]
>
>Il retargeting dei siti web ora rientra nel riquadro Personalizzazione web. Se hai acquistato solo il retargeting, visualizzerai questa sezione e accederai al prodotto di personalizzazione web con **solo** Funzioni di retargeting abilitate. In questo modo puoi accedere alle impostazioni dell’account, alla pagina Retargeting, ai segmenti e alle pagine di tracciamento aggiuntive.

Il remarketing è destinato ai potenziali clienti che hanno visitato il tuo sito in passato con display advertising in base a chi sono e a cosa hanno fatto. Il retargeting personalizzato è destinato a tipi di pubblico specifici con annunci pertinenti basati su dati di settore, account denominati e persone note.

La personalizzazione web aggiunge attualmente i dati alle seguenti piattaforme di remarketing:

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
   <th><p>Elenco ABM (elenchi account denominati)</p></th> 
  </tr> 
  <tr> 
   <th><p>Pubblico segmentato (in base ai segmenti)</p></th> 
  </tr> 
  <tr> 
   <th><p>Campagne Web selezionate</p></th> 
  </tr> 
 </tbody> 
</table>

## Configurazione remarketing {#remarketing-configuration}

1. Vai a **Retargeting**.

   ![](assets/one.png)

   >[!NOTE]
   >
   >La configurazione del retargeting è per dominio o sottodominio. Attiva gli altri domini se desideri inviare dati da tali domini alla piattaforma di retargeting.

1. Attiva le impostazioni per Google Analytics o Google Universal Analytics per dominio.

   >[!NOTE]
   >
   >Devi avere il Tag di retargeting Google implementato sul tuo sito web.
   >
   >Se l&#39;integrazione è già stata impostata con Personalizzazione Web e Google Analytics, non è necessario modificare questa parte in quanto si tratta della stessa configurazione in Impostazioni account.

   ![](assets/two.png)

1. Attiva la configurazione per Facebook. Fai clic su ed espandi il pannello a soffietto Facebook, quindi fai clic su **On** per inviare i rispettivi Eventi e dati tramite a Facebook Audience Manager. Clic **Salva**.

   >[!NOTE]
   >
   >Devi avere [Pixel pubblico personalizzato facebook](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)ha installato il tuo sito web per far funzionare questa funzione.

   ![](assets/three.png)

## Creazione di un pubblico segmentato {#creating-segmented-audience}

Un pubblico segmentato consente di selezionare un segmento esistente come pubblico da utilizzare per le campagne di retargeting. Ad esempio, selezionando i segmenti Persona nota.

>[!TIP]
>
>Non è necessario creare un pubblico segmentato per il settore o altri dati già inviati tramite nella configurazione del dominio. È meglio utilizzare i tipi di pubblico segmentati per segmenti basati su dati di persone note.

1. Clic **Creare un pubblico segmentato**.

   ![](assets/image2015-1-15-16-3a36-3a38.png)

1. Inserisci il Nome del pubblico, seleziona Canali, quindi seleziona Segmento dall’elenco dei Segmenti esistenti.

   ![](assets/image2015-1-15-16-3a40-3a17.png)

1. Clic **Salva**.

   Hai completato la configurazione del retargeting in Personalizzazione web, accedi alle piattaforme di retargeting, crea i tipi di pubblico in base a questi dati e configura le campagne pubblicitarie di retargeting.
