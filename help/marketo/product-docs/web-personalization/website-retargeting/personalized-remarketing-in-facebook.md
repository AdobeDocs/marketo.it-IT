---
unique-page-id: 4720917
description: Remarketing personalizzato in Facebook - Documentazione Marketo - Documentazione del prodotto
title: Remarketing personalizzato in Facebook
exl-id: 47636afa-49df-40ba-8948-4f2850467c2f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 1%

---

# Remarketing personalizzato in Facebook {#personalized-remarketing-in-facebook}

Il remarketing personalizzato consente di coinvolgere nuovamente gli utenti utilizzando i dati RTP e la potenza del remarketing Facebook.

>[!PREREQUISITES]
>
>* Completa il [Retargeting with Web Personalization Data](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md) setup
>* Consulta la sezione [](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) [Documentazione di facebook sui tipi di pubblico personalizzati](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) e il remarketing.


## Creazione di un pubblico in Facebook {#creating-an-audience-in-facebook}

1. In Facebook, vai al tuo [Scheda Pubblico](https://www.facebook.com/ads/audience_manager) in Ads Manager.

1. Fai clic su **Strumenti** e seleziona **Tipi di pubblico**.

   ![](assets/one-1.png)

1. Fai clic su **Creare un pubblico personalizzato**.

   ![](assets/two-1.png)

1. Seleziona **Traffico sito web**.

   ![](assets/image2015-1-19-16-3a32-3a2.png)

1. Nell’elenco Traffico sito web, seleziona **Combinazione personalizzata**.

   ![](assets/image2015-1-19-16-3a33-3a21.png)

1. Nell’elenco Includi, seleziona **Evento**.

   ![](assets/image2015-1-19-16-3a34-3a9.png)

1. Nell’elenco Evento, seleziona **Remarketing RTP** e seleziona un parametro.

   ![](assets/image2015-1-19-16-3a52-3a29.png)

1. Per questo esempio, selezionare Settore da contenere **Istruzione**. Invio **Istruzione** e modifica **Nell&#39;ultimo** 180 giorni. Immetti il nome del pubblico: **Industria dell&#39;istruzione**. Fai clic su **Crea pubblico**.

   ![](assets/image2015-1-19-16-3a56-3a15.png)

1. Ora hai creato un nuovo pubblico personalizzato utilizzando i dati RTP in Facebook.

   ![](assets/image2015-1-19-16-3a59-3a2.png)

## Punti dati RTP in Facebook {#rtp-data-points-in-facebook}

<table> 
 <tbody> 
  <tr> 
   <th>Nome evento</th> 
   <th> </th> 
  </tr> 
  <tr> 
   <td>Remarketing RTP</td> 
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
        <td>(Nome dell'elenco basato su conto)</td> 
       </tr> 
       <tr> 
        <td colspan="1">Categoria</td> 
        <td colspan="1"><p>Fortune 500</p><p>Fortuna 1000</p><p>Globale 2000</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">Gruppo</td> 
        <td colspan="1"><p>Enterprise</p><p>SMB</p></td> 
       </tr> 
       <tr> 
        <td>Settore</td> 
        <td><p>Difesa</p><p>Istruzione</p><p>Servizi finanziari</p><p>Governo</p><p>Medicale, Farma, Biotecnologia</p><p>Software e Internet</p><p>ecc.. (secondo le opzioni del settore RTP)</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">Pubblico segmentato</td> 
        <td colspan="1">(Nome del pubblico segmentato creato in RTP)</td> 
       </tr> 
      </tbody> 
     </table> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## Eseguire il targeting del pubblico con un annuncio {#target-your-audience-with-an-ad}

Per ulteriori dettagli, consulta [Documentazione di facebook](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#target-your-audience).

1. Vai a Gestione annunci, fai clic su **Crea annuncio**.

   ![](assets/image2015-1-19-17-3a10-3a19.png)

1. Seleziona **Invia persone al tuo sito web** come obiettivo della campagna.

   ![](assets/image2015-1-19-17-3a11-3a20.png)

1. Inserisci l’URL del sito web.

   ![](assets/image2015-1-19-17-3a12-3a39.png)

1. Crea il tuo set di annunci. Seleziona un pubblico personalizzato dall’elenco dei tipi di pubblico creati, ad esempio Education Industry.

   ![](assets/image2015-1-19-17-3a18-3a13.png)

1. Seleziona tutte le altre opzioni di set di annunci, imposta il budget e definisci i creativi degli annunci.

   ![](assets/image2015-1-19-17-3a19-3a25.png)

1. Ora siete tutti configurati con una campagna di remarketing personalizzata in Facebook.

>[!MORELIKETHIS]
>
>* [Retargeting with Web Personalization Data](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Remarketing personalizzato in Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)

