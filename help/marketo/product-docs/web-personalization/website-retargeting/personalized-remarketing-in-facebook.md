---
unique-page-id: 4720917
description: Remarketing personalizzato in Facebook - Documentazione Marketo - Documentazione del prodotto
title: Remarketing personalizzato in Facebook
exl-id: 47636afa-49df-40ba-8948-4f2850467c2f
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 1%

---

# Remarketing personalizzato in Facebook {#personalized-remarketing-in-facebook}

Il remarketing personalizzato consente di coinvolgere nuovamente gli utenti utilizzando i dati RTP e la potenza del remarketing Facebook.

>[!PREREQUISITES]
>
>* Completare l&#39;installazione di [Retargeting con dati Web Personalization](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* Rivedi la [&#128279;](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) [documentazione di Facebook su tipi di pubblico personalizzati](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) e remarketing.

## Creazione di un pubblico in Facebook {#creating-an-audience-in-facebook}

1. In Facebook, vai alla [scheda Pubblico](https://www.facebook.com/ads/audience_manager) in Ads Manager.

1. Fai clic su **Strumenti** e seleziona **Tipi di pubblico**.

   ![](assets/one-1.png)

1. Fai clic su **Crea un pubblico personalizzato**.

   ![](assets/two-1.png)

1. Seleziona **Traffico sito Web**.

   ![](assets/image2015-1-19-16-3a32-3a2.png)

1. Nell&#39;elenco Traffico sito Web selezionare **Combinazione personalizzata**.

   ![](assets/image2015-1-19-16-3a33-3a21.png)

1. Nell&#39;elenco Includi selezionare **Evento**.

   ![](assets/image2015-1-19-16-3a34-3a9.png)

1. Nell&#39;elenco Evento, selezionare **Remarketing RTP** e selezionare un parametro.

   ![](assets/image2015-1-19-16-3a52-3a29.png)

1. Per questo esempio, seleziona Settore per contenere **Istruzione**. Immetti **Istruzione** e modifica **Negli ultimi** in modo che siano 180 giorni. Immetti Nome Pubblico: **Settore Dell&#39;Istruzione**. Fai clic su **Crea pubblico**.

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
        <td>(Nome dell’elenco basato sull’account)</td> 
       </tr> 
       <tr> 
        <td colspan="1">Categoria</td> 
        <td colspan="1"><p>Fortune 500</p><p>Fortune 1000</p><p>Globale 2000</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">Gruppo</td> 
        <td colspan="1"><p>Enterprise</p><p>PMI</p></td> 
       </tr> 
       <tr> 
        <td>Settore</td> 
        <td><p>Difesa</p><p>Istruzione</p><p>Servizi finanziari</p><p>Pubblica amministrazione</p><p>Sanità, Pharma, Biotech</p><p>Software e Internet</p><p>ecc... (secondo le opzioni RTP del settore)</p></td> 
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

## Indirizza il pubblico con un annuncio {#target-your-audience-with-an-ad}

Per ulteriori dettagli, consulta la [documentazione di Facebook](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#target-your-audience).

1. Vai ad Ads Manager, fai clic su **Crea annuncio**.

   ![](assets/image2015-1-19-17-3a10-3a19.png)

1. Seleziona **Invia persone al tuo sito Web** come obiettivo della campagna.

   ![](assets/image2015-1-19-17-3a11-3a20.png)

1. Immetti l’URL del sito web.

   ![](assets/image2015-1-19-17-3a12-3a39.png)

1. Crea il set di annunci. Seleziona un pubblico personalizzato dall’elenco dei tipi di pubblico creati, ad esempio Settore dell’istruzione.

   ![](assets/image2015-1-19-17-3a18-3a13.png)

1. Seleziona tutte le altre opzioni per set di annunci, imposta il budget e definisci le creatività degli annunci.

   ![](assets/image2015-1-19-17-3a19-3a25.png)

1. Ora è tutto pronto per una campagna di remarketing personalizzata in Facebook.

>[!MORELIKETHIS]
>
>* [Retargeting con dati Web Personalization](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Remarketing personalizzato in Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
