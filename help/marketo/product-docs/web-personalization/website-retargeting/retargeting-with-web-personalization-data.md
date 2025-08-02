---
unique-page-id: 4720796
description: Retargeting con dati di Web Personalization - Documentazione di Marketo - Documentazione del prodotto
title: Retargeting con dati di Web Personalization
exl-id: b5af1f84-2061-4d0d-9d1f-2fff9191f028
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 1%

---

# Retargeting con dati [!DNL Web Personalization] {#retargeting-with-web-personalization-data}

>[!AVAILABILITY]
>
>Il retargeting dei siti web ora rientra nel riquadro Web Personalization. Se hai acquistato solo il retargeting, visualizzerai questa sezione e accederai al prodotto [!DNL Web Personalization] con **solo** funzionalità di retargeting abilitate. In questo modo puoi accedere alle impostazioni dell’account, alla pagina Retargeting, ai segmenti e alle pagine di tracciamento aggiuntive.

Il remarketing è destinato ai potenziali clienti che hanno visitato il tuo sito in passato con display advertising in base a chi sono e a cosa hanno fatto. Il retargeting personalizzato è destinato a tipi di pubblico specifici con annunci pertinenti basati su dati di settore, account denominati e persone note.

Web Personalization attualmente aggiunge dati alle seguenti piattaforme di remarketing:

* [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
* [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

[!DNL Web Personalization] invia i seguenti dati alle piattaforme di remarketing per creare tipi di pubblico ed eseguire campagne pubblicitarie di remarketing:

<table>
 <tbody>
  <tr>
   <th colspan="1">[!DNL Web Personalization] Dati</th>
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

1. Vai a **[!UICONTROL Retargeting]**.

   ![](assets/one.png)

   >[!NOTE]
   >
   >La configurazione del retargeting è per dominio o sottodominio. Attiva gli altri domini se desideri inviare dati da tali domini alla piattaforma di retargeting.

1. Attiva le impostazioni per Google Analytics o [!DNL Google Universal Analytics] per dominio.

   >[!NOTE]
   >
   >Devi avere il Tag di retargeting Google implementato sul tuo sito web.
   >
   >Se l&#39;integrazione è già stata impostata con Web Personalization e Google Analytics, non è necessario modificare questa parte in quanto si tratta della stessa configurazione in Impostazioni account.

   ![](assets/two.png)

1. Attiva la configurazione per Facebook. Fai clic sul pannello a soffietto [!DNL Facebook] ed espandilo, quindi fai clic su **[!UICONTROL On]** per inviare i rispettivi dati ed eventi a Facebook Audience Manager. Fai clic su **[!UICONTROL Save]**.

   >[!NOTE]
   >
   >Affinché questa funzione funzioni, devi avere [[!DNL Facebook] Pixel pubblico personalizzato](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) installato nel tuo sito Web.

   ![](assets/three.png)

## Creazione di un pubblico segmentato {#creating-segmented-audience}

Un pubblico segmentato consente di selezionare un segmento esistente come pubblico da utilizzare per le campagne di retargeting. Ad esempio, selezionando i segmenti Persona nota.

>[!TIP]
>
>Non è necessario creare un pubblico segmentato per il settore o altri dati già inviati tramite nella configurazione del dominio. È meglio utilizzare i tipi di pubblico segmentati per segmenti basati su dati di persone note.

1. Fai clic su **[!UICONTROL Create Segmented Audience]**.

   ![](assets/image2015-1-15-16-3a36-3a38.png)

1. Inserisci il Nome del pubblico, seleziona Canali, quindi seleziona Segmento dall’elenco dei Segmenti esistenti.

   ![](assets/image2015-1-15-16-3a40-3a17.png)

1. Fai clic su **[!UICONTROL Save]**.

   Hai completato la configurazione del retargeting in [!DNL Web Personalization], accedi alle tue piattaforme di retargeting, crea i tuoi tipi di pubblico in base a questi dati e configura le tue campagne pubblicitarie di retargeting.
