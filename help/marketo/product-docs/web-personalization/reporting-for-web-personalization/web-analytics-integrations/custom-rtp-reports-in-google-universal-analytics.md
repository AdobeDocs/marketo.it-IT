---
unique-page-id: 7504218
description: Report RTP personalizzati in Google Universal Analytics - Documenti Marketo - Documentazione prodotto
title: Report RTP personalizzati in Google Universal Analytics
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---


# Report RTP personalizzati in Google Universal Analytics {#custom-rtp-reports-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Integrare RTP con Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

Questo articolo spiega come impostare i rapporti personalizzati RTP per Google Universal Analytics (GUA).  I dati inviati da RTP a GUA possono essere impostati come due rapporti personalizzati separati, denominati:

* RTP B2B
* Coinvolgimento RTP

## Impostazione di un report personalizzato {#setting-up-a-custom-report}

1. Accedete alle Google Analytics.

1. Fare clic su **Personalizzazione** nel menu principale.

1. Fare clic su **+Nuovo report personalizzato**.

![](assets/image2015-3-22-16-3a10-3a48.png)

## Report RTP B2B {#rtp-b-b-report}

1. Denominate il report **RTP B2B Report**.

1. Denominate la prima scheda **Industria**.

>[!NOTE]
>
>**Duplica questa scheda** e ne crei altre simili - passaggio 5)

1. Selezionare il tipo di rapporto **Explorer**.

   ![](assets/image2015-3-22-16-3a15-3a25.png)

1. Nella sezione **Gruppi di metriche**, seleziona le metriche rilevanti per la tua attività.

   a. Consigliamo quanto segue:

   ![](assets/image2015-3-22-16-3a16-3a40.png)

1. Duplica questa scheda 4 volte e denominale:

   1. **Industria**
   1. **Gruppo**
   1. **Categoria**
   1. **ABM**
   1. **Organizzazioni**

   ![](assets/image2015-3-22-16-3a17-3a41.png)

1. Nella sezione **Dimension Drill downs** impostare le dimensioni rilevanti per ciascuna scheda come indicato di seguito.

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Nome scheda 
    </div></th> 
   <th> 
    <div>
      Dimension Drill down
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Industria</td> 
   <td><img src="assets/1.png" data-linked-resource-id="7514675" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Gruppo</td> 
   <td><img src="assets/2.png" data-linked-resource-id="7514674" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Categoria</td> 
   <td><img src="assets/3.png" data-linked-resource-id="7514673" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>ABM</td> 
   <td><img src="assets/5.png" data-linked-resource-id="7514677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Organizzazioni</td> 
   <td><img src="assets/5.png" data-linked-resource-id="7514677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. Non impostare filtri e impostare il rapporto in modo che sia disponibile per **Tutti i dati del sito Web** (o modificare se pertinente per un account Analytics specifico).

1. Fare clic su **Salva**.

   ![](assets/image2015-3-22-16-3a21-3a23.png)

## Rapporto di coinvolgimento RTP {#rtp-engagement-report}

1. Denominate il report **Rapporto di coinvolgimento RTP**.

1. Impostate il nome della prima scheda su **All Engagement**.

>[!NOTE]
>
>Duplica questa scheda e ne crea altre simili - passaggio 5)

1. Selezionare il tipo di rapporto **Explorer**.

   ![](assets/image2015-3-22-16-3a23-3a36.png)

1. Nella sezione Gruppi di metriche, seleziona le metriche rilevanti per la tua attività. Di seguito è riportata una raccomandazione:

   ![](assets/image2015-3-22-16-3a24-3a57.png)

1. Duplica questa scheda 4 volte e denominale:

   1. **Tutto il coinvolgimento**
   1. **Coinvolgimento per settore**
   1. **Coinvolgimento per gruppo**
   1. **Coinvolgimento per categoria**
   1. **Engagement by ABM**

   ![](assets/image2015-3-22-16-3a26-3a21.png)

1. Nella sezione **Dimension Drill downs** impostare le dimensioni relative a ciascuna scheda come segue:

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Nome scheda 
    </div></th> 
   <th> 
    <div>
      Dimension Drill down 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Tutto il coinvolgimento</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Engagement by ABM</td> 
   <td><img width="277" src="assets/4.png" data-linked-resource-id="7514678" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Coinvolgimento per categoria</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Coinvolgimento per gruppo</td> 
   <td><img src="assets/c.png" data-linked-resource-id="7514681" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Coinvolgimento per settore</td> 
   <td><img src="assets/b.png" data-linked-resource-id="7514682" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. Impostate i seguenti filtri:

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Inc/Exc 
    </div></th> 
   <th> 
    <div>
      Field 
    </div></th> 
   <th> 
    <div>
      Tipo corrispondenza 
    </div></th> 
   <th> 
    <div>
      Valori 
    </div></th> 
   <th colspan="1"> 
    <div>
      Commenti 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><p>Includi</p></td> 
   <td><p>Categoria evento</p></td> 
   <td>Regex</td> 
   <td>RTP-Campaigns|RTP-Recommendations|RTP-Segments</td> 
   <td colspan="1">Filtrerà tutti gli altri eventi personalizzati non correlati a RTP</td> 
  </tr> 
  <tr> 
   <td>Escludi</td> 
   <td>Etichetta evento</td> 
   <td>Regex</td> 
   <td>#</td> 
   <td colspan="1">Consente di filtrare dalla campagna di report utilizzando # nel nome della campagna</td> 
  </tr> 
 </tbody> 
</table>

1. Impostate questo rapporto in modo che sia disponibile per **Tutti i dati del sito Web** (o modificate se necessario).

   ![](assets/image2015-3-22-16-3a29-3a5.png)

1. Fare clic su **Salva**.

![](assets/image2015-3-22-16-3a30-3a0.png)

>[!MORELIKETHIS]
>
>[Integrare RTP con Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)
>
>[Dashboard RTP personalizzati in Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-dashboards-in-google-universal-analytics.md)
