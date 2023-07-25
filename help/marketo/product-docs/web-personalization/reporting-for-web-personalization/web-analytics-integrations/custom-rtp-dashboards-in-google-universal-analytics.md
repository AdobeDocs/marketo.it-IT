---
unique-page-id: 7504238
description: Dashboard RTP personalizzati in Google Universal Analytics - Documentazione Marketo - Documentazione del prodotto
title: Dashboard RTP personalizzati in Google Universal Analytics
exl-id: 712c71b6-74eb-4743-9ca8-50c912278e62
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---

# Dashboard RTP personalizzati in Google Universal Analytics {#custom-rtp-dashboards-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Integrare RTP con Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

Questo post spiega come impostare dashboard RTP in Google Universal Analytics (GUA). I dati inviati dall’RTP alla GUA possono essere impostati come due dashboard personalizzati separati denominati:

* RTP B2B
* Coinvolgimento RTP

## Impostazione di un dashboard personalizzato {#setting-up-a-custom-dashboard}

1. Accedi alle Google Analytics. Fai clic su **Generazione rapporti** nel menu principale. Clic **Dashboard** e **+Nuovo dashboard personalizzato**.

   ![](assets/image2015-3-22-16-3a41-3a29.png)

1. Seleziona **Area di lavoro vuota**, aggiungi un **Nome dashboard** e fai clic su **Crea dashboard**.

1. Clic **Aggiungi widget** per creare un nuovo widget.

   ![](assets/image2015-3-22-16-3a46-3a48.png)

## Dashboard B2B RTP {#rtp-b-b-dashboard}

Questa dashboard consente agli utenti di analizzare le prestazioni del sito web dal punto di vista B2B.

Fornisce informazioni come il comportamento all’origine delle visite e sul sito per settore, ricavi, dimensioni, elenchi basati su account e segmenti di destinazione.

Il dashboard è costituito da 3 colonne

* Origine traffico
* Segmentazione
* Drill-down firmografico

1. Crea un nuovo dashboard denominato **Dashboard B2B RTP** e definisci i seguenti widget:

![](assets/image2015-3-22-16-3a50-3a3.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Colonna 1 - Origini del traffico
    </div></th> 
   <th> 
    <div> <strong>Colonna 2 - Segmentazione</strong> 
    </div></th> 
   <th> 
    <div> <strong>Colonna 3 - Espansione firmografica</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Nome: sessioni per segmenti e canali</li> 
     <li>Tipo widget: barra<br></li> 
     <li>Crea un grafico a barre che mostra: Sessione</li> 
     <li>Raggruppato per: etichetta evento</li> 
     <li>Pivot per: raggruppamento canali predefinito</li> 
     <li>Filtro: <br>Mostra solo | Categoria di eventi (contenente) segmenti RTP</li> 
    </ul><p><img width="300" src="assets/image2015-3-23-11-3a32-3a13.png" data-linked-resource-id="7504247" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: numero di utenti RTP segmentati</li> 
     <li>Tipo: 2.1 Metrica</li> 
     <li>Mostra la metrica seguente: Utenti<br></li> 
     <li>Filtro: <br>Mostra solo | Categoria di eventi (contenente) segmenti RTP</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a6.png" data-linked-resource-id="7504249" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: sessioni per settore</li> 
     <li>Tipo: Torta<br></li> 
     <li>Crea un grafico a torta che mostra: Sessioni</li> 
     <li>Raggruppato per: RTP-Industry</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a27.png" data-linked-resource-id="7504250" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <th> 
    <ul> 
     <li><strong>Nome: sessioni per settore e canali</strong></li> 
     <li><strong>Tipo widget: barra</strong></li> 
     <li><strong>Crea un grafico a barre che mostra: Sessione</strong></li> 
     <li><strong>Raggruppato per: RTP-Industry</strong></li> 
     <li><strong>Pivot per: raggruppamento canali predefinito</strong><br><img width="300" src="assets/image2015-3-23-11-3a33-3a52.png" data-linked-resource-id="7504252" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></li> 
    </ul></th> 
   <th> 
    <ul> 
     <li><strong>Nome: sessioni segmentate per paese</strong></li> 
     <li><strong>Tipo: Geomap</strong></li> 
     <li><strong>Traccia la metrica selezionata: Paese | Sessioni</strong></li> 
     <li><strong>Seleziona una regione: Il mondo</strong></li> 
     <li><strong>Filtro: Mostra solo | Categoria di eventi (contenente) segmenti RTP</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a34-3a18.png" data-linked-resource-id="7504253" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li><strong>Nome: sessioni per categoria RTP</strong></li> 
     <li><strong>Tipo: Torta</strong></li> 
     <li><strong>Crea un grafico a torta che mostra: Sessioni</strong></li> 
     <li><strong>Raggruppato per: categoria RTP</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a1.png" data-linked-resource-id="7504254" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nome: Segmenti di destinazione principali</li> 
     <li>Tipo: barra</li> 
     <li>Crea un grafico a barre che mostra: Utenti</li> 
     <li>Raggruppato per: azione evento</li> 
     <li>Filtro: Mostra solo | Categoria di eventi (contenente) segmenti RTP</li> 
    </ul><p><img width="350" src="assets/add-a-widget.png" data-linked-resource-id="11382874" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li>Nome: sessioni per gruppi RTP</li> 
     <li>Tipo: barra<br></li> 
     <li>Crea un grafico a barre che mostra: Sessioni</li> 
     <li>Raggruppato per: RTP-Group</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a35-3a54.png" data-linked-resource-id="7504256" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nome: sessioni e obiettivi per segmenti principali</li> 
     <li>Tipo: tabella<br></li> 
     <li>Visualizza le colonne seguenti: <br>Etichetta evento | Sessioni | Tasso di conversione obiettivo</li> 
     <li>Filtro: <br>Mostra solo | Categoria di eventi (contenente) segmenti RTP</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a36-3a15.png" data-linked-resource-id="7504257" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
   <th> </th> 
  </tr> 
 </tbody> 
</table>

## Dashboard del coinvolgimento RTP {#rtp-engagement-dashboard}

Questa dashboard consente agli utenti di analizzare le prestazioni della campagna RTP e il coinvolgimento con i motori di consigli. Fornisce un confronto tra media. durata della sessione e pagine per sessione tra:

* Non coinvolto
* Coinvolto (impression e clic su una campagna personalizzata)
* Fai clic sul motore di consigli e sui principali contenuti consigliati

Crea un nuovo dashboard denominato **Dashboard del coinvolgimento RTP** e definisci i seguenti widget:

![](assets/image2015-3-22-17-3a7-3a19.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div> <strong>Colonna 1 Esposizione campagne</strong> 
    </div></th> 
   <th> 
    <div> <strong>Clickthrough di campagne colonna 2</strong> 
    </div></th> 
   <th> 
    <div> <strong>Colonna 3 Motore di consigli</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Nome: <strong>CTA (coinvolgimento) totale</strong></li> 
     <li>Tipo: <strong>2.1 Metrica </strong></li> 
     <li>Mostra la metrica seguente: <strong>Eventi totali</strong></li> 
     <li>Filtri:<br><strong>[mostra solo] Categoria evento (contiene): Campagne RTP</strong><br><strong>[only show] Azione evento (corrispondenza esatta): Impression</strong><strong>[do not show] Etichetta evento (contenente): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a37-3a55.png" data-linked-resource-id="7504259" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>CTA (clickthrough) - Totale</strong></li> 
     <li>Tipo: <strong>2.1 Metrica </strong></li> 
     <li>Mostra la metrica seguente: <strong>Eventi totali</strong></li> 
     <li>Filtri:<br><strong>[mostra solo] Categoria evento (contiene): Campagne RTP</strong><br><strong>[only show] Azione evento (esattamente corrispondente): Clic</strong><strong>[do not show] Etichetta evento (contenente): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a38-3a12.png" data-linked-resource-id="7504261" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>CRE - Clic totali</strong></li> 
     <li>Tipo: <strong>2.1 Metrica</strong><br></li> 
     <li>Mostra la metrica seguente: <strong>Visualizzazioni pagina</strong></li> 
     <li>Filtro: <strong>[mostra solo] Pagina (contenente): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a30.png" data-linked-resource-id="7504262" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> 
    <ul> 
     <li>Nome: <strong>Media Durata della sessione (coinvolgimento)</strong></li> 
     <li>Tipo: <strong>2.1 Metrica </strong></li> 
     <li>Mostra la metrica seguente: <strong>Media Durata sessione</strong></li> 
     <li>Filtri:<br><strong>[only show] Categoria evento (esattamente corrispondente): Campagne RTP</strong><br><strong>[only show] Azione evento (corrispondenza esatta): impression</strong><strong>[do not show] Etichetta evento (contenente): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a21.png" data-linked-resource-id="7504264" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nome: <strong>Media Durata della sessione (click-through)</strong></li> 
     <li>Tipo: <strong>2.1 Metrica </strong></li> 
     <li>Mostra la metrica seguente: <strong>Media Durata sessione</strong></li> 
     <li>Filtri:<br><strong>[only show] Categoria evento (esattamente corrispondente): Campagne RTP</strong><br><strong>[only show] Azione evento (esattamente corrispondente): clic</strong><strong>[do not show] Etichetta evento (contenente): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a37.png" data-linked-resource-id="7504265" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nome: <strong>CRE - Contenuto consigliato principale</strong></li> 
     <li>Tipo: <strong>Tabella</strong><br></li> 
     <li>Visualizza le colonne seguenti: <br><strong>Titolo pagina | Pageview</strong><br></li> 
     <li>Filtri:<br>Filtro: <strong>[mostra solo] Pagina (contenente): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a51.png" data-linked-resource-id="7504266" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nome: <strong>Pagine/Sessione (Coinvolgimento)</strong></li> 
     <li>Tipo: <strong>2.1 Metrica </strong></li> 
     <li>Mostra la metrica seguente: <strong>Pagine/Sessione</strong></li> 
     <li>Filtri:<br><strong>[only show] Categoria evento (esattamente corrispondente): Campagne RTP</strong></li> 
     <li><strong>[only show] Azione evento (corrispondenza esatta): impression</strong></li> 
     <li><strong>[do not show] Etichetta evento (contenente): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a10.png" data-linked-resource-id="7504267" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>Pagine/Sessione (Clickthrough)</strong></li> 
     <li>Tipo: <strong>2.1 Metrica </strong></li> 
     <li>Mostra la metrica seguente: <strong>Pagine/Sessione</strong></li> 
     <li>Filtri:<br><strong>[only show] Categoria evento (esattamente corrispondente): Campagne RTP</strong></li> 
     <li><strong>[only show] Azione evento (esattamente corrispondente): clic</strong></li> 
     <li><strong>[do not show] Etichetta evento (contenente): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a42-3a32.png" data-linked-resource-id="7504268" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nome: <strong>Impression da parte di CTA</strong></li> 
     <li>Tipo: <strong>Tabella</strong></li> 
     <li>Visualizza le colonne seguenti: <strong>Etichetta evento | Totale eventi | Utenti</strong></li> 
     <li>Filtri:<br><strong>[only show] Categoria evento (esattamente corrispondente): Campagne RTP</strong><br><strong>[only show] Azione evento (corrispondenza esatta): impression</strong><strong>[do not show] Etichetta evento (contenente): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a48.png" data-linked-resource-id="7504269" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>Clickthrough da CTA</strong></li> 
     <li>Tipo: <strong>Tabella</strong></li> 
     <li>Visualizza le colonne seguenti: <strong>Etichetta evento | Totale eventi | Utenti</strong></li> 
     <li>Filtri:<br><strong>[only show] Categoria evento (esattamente corrispondente): Campagne RTP</strong><br><strong>[only show] Azione evento (esattamente corrispondente): clic</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a43-3a4.png" data-linked-resource-id="7504270" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Integrare RTP con Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
>
>[Rapporti RTP personalizzati in Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
