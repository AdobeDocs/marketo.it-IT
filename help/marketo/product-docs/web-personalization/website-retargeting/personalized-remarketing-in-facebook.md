---
unique-page-id: 4720917
description: Notizie personalizzate su Facebook - Marketo Docs - Documentazione prodotto
title: Osservazioni personalizzate su Facebook
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---


# Osservazioni personalizzate su Facebook {#personalized-remarketing-in-facebook}

La funzione di marcatura personalizzata consente di coinvolgere nuovamente gli utenti utilizzando i dati RTP e la potenza della funzione di marcatura di Facebook.

>[!NOTE]
>
>**Prerequisiti**
>
>* Completa il [retargeting con la configurazione dei dati](retargeting-with-web-personalization-data.md) di personalizzazione Web
>* Consulta la documentazione di [](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) Facebook su [](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)Pubblico personalizzato e Osservazioni

>



## Creazione di un pubblico in Facebook {#creating-an-audience-in-facebook}

1. In Facebook, andate alla scheda [](https://www.facebook.com/ads/audience_manager) Audience in Ads Manager.
1. Fate clic su **Strumenti** e selezionate **Audience**.

   ![](assets/one-1.png)

1. Fate clic su **Crea un pubblico** personalizzato.

   ![](assets/two-1.png)

1. Selezionate Traffico **sito Web**.

   ![](assets/image2015-1-19-16-3a32-3a2.png)

1. Nell&#39;elenco del traffico del sito Web, selezionare** Combinazione personalizzata**.

   ![](assets/image2015-1-19-16-3a33-3a21.png)

1. Nell&#39;elenco Includi, selezionare **Evento**.

   ![](assets/image2015-1-19-16-3a34-3a9.png)

1. Nell&#39;elenco Evento, selezionare **RTP Note **e selezionare un parametro.

   ![](assets/image2015-1-19-16-3a52-3a29.png)

1. In questo esempio, selezionare Settore per contenere **Istruzione**. Accedete **a Education** e modificate **In the Last** in modo da ottenere 180 giorni. Inserisci nome pubblico: **Istruzione**. Fate clic su **Crea pubblico**.

   ![](assets/image2015-1-19-16-3a56-3a15.png)

1. Ora hai creato una nuova audience personalizzata utilizzando i dati RTP in Facebook.

   ![](assets/image2015-1-19-16-3a59-3a2.png)

## Punti dati RTP in Facebook {#rtp-data-points-in-facebook}

<table> 
 <tbody> 
  <tr> 
   <th>Nome evento</th> 
   <th> </th> 
  </tr> 
  <tr> 
   <td>Risposte RTP</td> 
   <td> 
    <div> 
     <table> 
      <tbody> 
       <tr> 
        <th>Parametro</th> 
        <th>Valore</th> 
       </tr> 
       <tr> 
        <td>Elenco ABM</td> 
        <td>(Nome dell'elenco basato su account)</td> 
       </tr> 
       <tr> 
        <td colspan="1">Categoria</td> 
        <td colspan="1"><p>Fortune 500</p><p>Fortune 1000</p><p>Global 2000</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">Gruppo</td> 
        <td colspan="1"><p>Enterprise</p><p>SMB</p></td> 
       </tr> 
       <tr> 
        <td>Industria</td> 
        <td><p>Difesa</p><p>Istruzione</p><p>Servizi finanziari</p><p>Governo</p><p>Medicale, Pharma, Biotech</p><p>Software e Internet</p><p>ecc... (in base alle opzioni del settore RTP)</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">Pubblico segmentato</td> 
        <td colspan="1">(Nome dell’audience segmentata creata in RTP)</td> 
       </tr> 
      </tbody> 
     </table> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## Esegue il targeting del pubblico con un annuncio {#target-your-audience-with-an-ad}

Per ulteriori dettagli, consultate la documentazione [di](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#target-your-audience)Facebook.

1. Vai a Gestione annunci, fai clic su **Crea annuncio**.

   ![](assets/image2015-1-19-17-3a10-3a19.png)

1. Selezionate **Invia utenti al sito Web** come obiettivo della campagna.

   ![](assets/image2015-1-19-17-3a11-3a20.png)

1. Inserite l’URL del sito Web.

   ![](assets/image2015-1-19-17-3a12-3a39.png)

1. Create il set di annunci. Selezionate un&#39;audience personalizzata dall&#39;elenco di Audience che avete creato, ad esempio, Education Industry (Settore dell&#39;istruzione).

   ![](assets/image2015-1-19-17-3a18-3a13.png)

1. Seleziona tutte le altre opzioni di set di annunci, imposta il budget e definisce le tue creatività.

   ![](assets/image2015-1-19-17-3a19-3a25.png)

1. Ora tutti siete pronti con una campagna di remarketing personalizzata su Facebook.

>[!NOTE]
>
>**Articoli correlati**
>
>* [Ritargeting con dati di personalizzazione Web](retargeting-with-web-personalization-data.md)
>* [Osservazioni personalizzate in Google](personalized-remarketing-in-google.md)

>



