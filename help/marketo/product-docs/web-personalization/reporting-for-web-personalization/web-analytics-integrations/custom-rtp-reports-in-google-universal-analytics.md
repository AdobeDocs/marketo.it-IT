---
unique-page-id: 7504218
description: Rapporti RTP personalizzati in Google Universal Analytics - Documentazione Marketo - Documentazione del prodotto
title: Rapporti RTP personalizzati in Google Universal Analytics
exl-id: c8b1e653-03b8-48bc-b80d-3e6cdf3485c3
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 2%

---

# Rapporti RTP personalizzati in Google Universal Analytics {#custom-rtp-reports-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Integrare RTP con Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

Questo articolo spiega come impostare rapporti personalizzati RTP per Google Universal Analytics (GUA).  I dati inviati dall’RTP alla GUA possono essere impostati come due rapporti personalizzati separati, denominati:

* RTP B2B
* Coinvolgimento RTP

## Impostazione di un rapporto personalizzato {#setting-up-a-custom-report}

1. Accedi alle Google Analytics.

1. Fai clic su **Personalizzazione** nel menu principale.

1. Fare clic su **+Nuovo report personalizzato**.

![](assets/image2015-3-22-16-3a10-3a48.png)

## Rapporto B2B RTP {#rtp-b-b-report}

1. Denomina il rapporto **Rapporto B2B RTP**.

1. Denomina la prima scheda **Settore**.

>[!NOTE]
>
>**Duplicare questa scheda** e crearne altre simili - passaggio 5)

1. Selezionare il tipo di report **Explorer**.

   ![](assets/image2015-3-22-16-3a15-3a25.png)

1. Nella sezione **Gruppi di metriche**, seleziona le metriche rilevanti per la tua azienda.

   a. Si raccomanda quanto segue:

   ![](assets/image2015-3-22-16-3a16-3a40.png)

1. Duplica questa scheda 4 volte e denominale:

   1. **Settore**
   1. **Gruppo**
   1. **Categoria**
   1. **ABM**
   1. **Organizzazioni**

   ![](assets/image2015-3-22-16-3a17-3a41.png)

1. Nella sezione **Drill down dei Dimension**, imposta le dimensioni rilevanti per ogni scheda come indicato di seguito.

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Nome scheda 
    </div></th> 
   <th> 
    <div>
      Espansioni Dimension
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Settore</td> 
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
   <td>Organismi</td> 
   <td><img src="assets/5.png" data-linked-resource-id="7514677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. Non impostare alcun filtro e impostare questo report come disponibile per **Tutti i dati del sito Web** (o modificarlo in base all&#39;account Analytics specifico).

1. Fai clic su **Salva**.

   ![](assets/image2015-3-22-16-3a21-3a23.png)

## Rapporto sul coinvolgimento RTP {#rtp-engagement-report}

1. Denomina il report **Report di coinvolgimento RTP**.

1. Impostare il nome della prima scheda su **Tutto il coinvolgimento**.

>[!NOTE]
>
>Questa scheda verrà duplicata e ne verranno create altre simili (passaggio 5)

1. Selezionare il tipo di report **Explorer**.

   ![](assets/image2015-3-22-16-3a23-3a36.png)

1. Nella sezione Gruppi di metriche, seleziona le metriche rilevanti per la tua azienda. Ecco un consiglio:

   ![](assets/image2015-3-22-16-3a24-3a57.png)

1. Duplica questa scheda 4 volte e denominale:

   1. **Tutto il coinvolgimento**
   1. **Coinvolgimento per settore**
   1. **Coinvolgimento per gruppo**
   1. **Coinvolgimento per categoria**
   1. **Coinvolgimento da ABM**

   ![](assets/image2015-3-22-16-3a26-3a21.png)

1. Nella sezione **Drill down dei Dimension**, imposta le dimensioni rilevanti per ogni scheda come segue:

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Nome scheda 
    </div></th> 
   <th> 
    <div>
      Espansioni Dimension 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Tutto il coinvolgimento</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Coinvolgimento da parte di ABM</td> 
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

1. Imposta i seguenti filtri:

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Inc/Exc 
    </div></th> 
   <th> 
    <div>
      Campo 
    </div></th> 
   <th> 
    <div>
      Tipo di corrispondenza 
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
   <td>RTP-Campaigns|RTP-Recommendations|Segmenti RTP</td> 
   <td colspan="1">Filtra tutti gli altri eventi personalizzati non correlati a RTP</td> 
  </tr> 
  <tr> 
   <td>Escludi</td> 
   <td>Etichetta evento</td> 
   <td>Regex</td> 
   <td>N.</td> 
   <td colspan="1">Consente di filtrare dalla campagna di rapporti utilizzando # nel nome della campagna</td> 
  </tr> 
 </tbody> 
</table>

1. Impostare questo report affinché sia disponibile per **Tutti i dati del sito Web** (o modificarlo se necessario).

   ![](assets/image2015-3-22-16-3a29-3a5.png)

1. Fai clic su **Salva**.

![](assets/image2015-3-22-16-3a30-3a0.png)

>[!MORELIKETHIS]
>
>[Integrare RTP con Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)
>
>[Dashboard RTP personalizzati in Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-dashboards-in-google-universal-analytics.md)
