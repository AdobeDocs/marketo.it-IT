---
unique-page-id: 7504238
description: Dashboard RTP personalizzati in Google Universal Analytics - Documenti Marketo - Documentazione del prodotto
title: Dashboard RTP personalizzati in Google Universal Analytics
exl-id: 712c71b6-74eb-4743-9ca8-50c912278e62
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---

# Dashboard RTP personalizzati in Google Universal Analytics {#custom-rtp-dashboards-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Integrare RTP con Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

Questo post spiega come configurare le dashboard RTP in Google Universal Analytics (GUA). I dati inviati da RTP a GUA possono essere impostati come due dashboard personalizzati separati, denominati:

* RTP B2B
* Coinvolgimento RTP

## Configurazione di un dashboard personalizzato {#setting-up-a-custom-dashboard}

1. Accedi a Google Analytics. Fai clic su **Reporting** nel menu principale. Fai clic su **Dashboard** e **+Nuovo dashboard personalizzato**.

   ![](assets/image2015-3-22-16-3a41-3a29.png)

1. Seleziona **Canvas vuoto**, aggiungi un **Nome dashboard** e fai clic su **Crea dashboard**.

1. Fai clic su **Aggiungi widget** per creare un nuovo widget.

   ![](assets/image2015-3-22-16-3a46-3a48.png)

## Dashboard RTP B2B {#rtp-b-b-dashboard}

Questo dashboard consente agli utenti di analizzare le prestazioni del sito web dal punto di vista B2B.

Fornisce informazioni come il comportamento di origine delle visite e in loco per settore, ricavi, dimensioni, elenchi basati su account e segmenti di destinazione.

Il dashboard è costituito da 3 colonne

* Origine traffico
* Segmentazione
* Andamento a scatto

1. Crea un nuovo dashboard denominato **Dashboard RTP B2B** e definire i widget seguenti:

![](assets/image2015-3-22-16-3a50-3a3.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Colonna 1 - Sorgenti Di Traffico
    </div></th> 
   <th> 
    <div> <strong>Colonna 2 - Segmentazione</strong> 
    </div></th> 
   <th> 
    <div> <strong>Colonna 3 - Foratura Firmografica verso il basso</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Nome: Sessioni per segmenti e canali</li> 
     <li>Tipo di widget: Barre<br></li> 
     <li>Crea un grafico a barre che mostra: Sessione</li> 
     <li>Raggruppato da: Etichetta evento</li> 
     <li>Pivot per: Raggruppamento canali predefinito</li> 
     <li>Filtro: <br>Mostra solo | Categoria evento (contenente) Segmenti RTP</li> 
    </ul><p><img width="300" src="assets/image2015-3-23-11-3a32-3a13.png" data-linked-resource-id="7504247" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: Numero di utenti segmentati RTP</li> 
     <li>Tipo: 2.1 Metrica</li> 
     <li>Mostra la metrica seguente: Utenti<br></li> 
     <li>Filtro: <br>Mostra solo | Categoria evento (contenente) Segmenti RTP</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a6.png" data-linked-resource-id="7504249" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: Sessioni per settore</li> 
     <li>Tipo: Torta<br></li> 
     <li>Crea un grafico a torta che mostra: Sessioni</li> 
     <li>Raggruppato da: RTP-Industry</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a27.png" data-linked-resource-id="7504250" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <th> 
    <ul> 
     <li><strong>Nome: Sessioni per settore e canali</strong></li> 
     <li><strong>Tipo di widget: Barre</strong></li> 
     <li><strong>Crea un grafico a barre che mostra: Sessione</strong></li> 
     <li><strong>Raggruppato da: RTP-Industry</strong></li> 
     <li><strong>Pivot per: Raggruppamento canali predefinito</strong><br><img width="300" src="assets/image2015-3-23-11-3a33-3a52.png" data-linked-resource-id="7504252" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></li> 
    </ul></th> 
   <th> 
    <ul> 
     <li><strong>Nome: Sessioni segmentate per paese</strong></li> 
     <li><strong>Tipo: Geomap</strong></li> 
     <li><strong>Tracciare la metrica selezionata: Paese | Sessioni</strong></li> 
     <li><strong>Selezionare un'area: Il mondo</strong></li> 
     <li><strong>Filtro: Mostra solo | Categoria evento (contenente) Segmenti RTP</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a34-3a18.png" data-linked-resource-id="7504253" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li><strong>Nome: Sessioni per categoria RTP</strong></li> 
     <li><strong>Tipo: Torta</strong></li> 
     <li><strong>Crea un grafico a torta che mostra: Sessioni</strong></li> 
     <li><strong>Raggruppato da: Categoria RTP</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a1.png" data-linked-resource-id="7504254" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nome: Segmenti di destinazione principali</li> 
     <li>Tipo: Barre</li> 
     <li>Crea un grafico a barre che mostra: Utenti</li> 
     <li>Raggruppato da: Azione evento</li> 
     <li>Filtro: Mostra solo | Categoria evento (contenente) Segmenti RTP</li> 
    </ul><p><img width="350" src="assets/add-a-widget.png" data-linked-resource-id="11382874" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li>Nome: Sessioni per gruppi RTP</li> 
     <li>Tipo: Barre<br></li> 
     <li>Crea un grafico a barre che mostra: Sessioni</li> 
     <li>Raggruppato da: Gruppo RTP</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a35-3a54.png" data-linked-resource-id="7504256" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nome: Sessioni e obiettivi per segmenti principali</li> 
     <li>Tipo: Tabella<br></li> 
     <li>Visualizza le colonne seguenti: <br>Etichetta evento | Sessioni | Tasso di conversione obiettivo</li> 
     <li>Filtro: <br>Mostra solo | Categoria evento (contenente) Segmenti RTP</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a36-3a15.png" data-linked-resource-id="7504257" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
   <th> </th> 
  </tr> 
 </tbody> 
</table>

## Dashboard di coinvolgimento RTP {#rtp-engagement-dashboard}

Questo dashboard consente agli utenti di analizzare le prestazioni della campagna RTP e i relativi coinvolgimenti nei motori di raccomandazione. Fornisce il confronto della media. durata della sessione e pagine per sessione tra:

* Non attivato
* Coinvolto (impression e clic su una campagna personalizzata)
* Clic sul motore di raccomandazione e sul contenuto principale consigliato

Crea un nuovo dashboard denominato **Dashboard di coinvolgimento RTP** e definire i widget seguenti:

![](assets/image2015-3-22-17-3a7-3a19.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div> <strong>Esposizione colonna 1 Campagne</strong> 
    </div></th> 
   <th> 
    <div> <strong>Clickthrough colonna 2 campagne</strong> 
    </div></th> 
   <th> 
    <div> <strong>Motore di raccomandazione della colonna 3</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Nome: <strong>CTA totale (coinvolgimento)</strong></li> 
     <li>Tipo: <strong>2.1 Metrica </strong></li> 
     <li>Mostra la metrica seguente: <strong>Totale eventi</strong></li> 
     <li>Filtri:<br><strong>[Mostra solo] Categoria evento (contiene): Campagne RTP</strong><br><strong>[Mostra solo] Azione evento (corrispondente esattamente a: Impression</strong><strong>[non mostrare] Etichetta evento (contenente): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a37-3a55.png" data-linked-resource-id="7504259" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>CTA totale (click-through)</strong></li> 
     <li>Tipo: <strong>2.1 Metrica </strong></li> 
     <li>Mostra la metrica seguente: <strong>Totale eventi</strong></li> 
     <li>Filtri:<br><strong>[Mostra solo] Categoria evento (contiene): Campagne RTP</strong><br><strong>[Mostra solo] Azione evento (esattamente corrispondente): Clic</strong><strong>[non mostrare] Etichetta evento (contenente): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a38-3a12.png" data-linked-resource-id="7504261" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>CRE - Clic Totale</strong></li> 
     <li>Tipo: <strong>2.1 Metrica</strong><br></li> 
     <li>Mostra la metrica seguente: <strong>Pageviews</strong></li> 
     <li>Filtro: <strong>[Mostra solo] Pagina (contenente): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a30.png" data-linked-resource-id="7504262" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> 
    <ul> 
     <li>Nome: <strong>Media Durata della sessione (coinvolgimento)</strong></li> 
     <li>Tipo: <strong>2.1 Metrica </strong></li> 
     <li>Mostra la metrica seguente: <strong>Media Durata sessione</strong></li> 
     <li>Filtri:<br><strong>[Mostra solo] Categoria evento (esattamente corrispondente): Campagne RTP</strong><br><strong>[Mostra solo] Azione evento (esattamente corrispondente): impression</strong><strong>[non mostrare] Etichetta evento (contenente): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a21.png" data-linked-resource-id="7504264" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nome: <strong>Media Durata sessione (click-through)</strong></li> 
     <li>Tipo: <strong>2.1 Metrica </strong></li> 
     <li>Mostra la metrica seguente: <strong>Media Durata sessione</strong></li> 
     <li>Filtri:<br><strong>[Mostra solo] Categoria evento (esattamente corrispondente): Campagne RTP</strong><br><strong>[Mostra solo] Azione evento (esattamente corrispondente): click</strong><strong>[non mostrare] Etichetta evento (contenente): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a37.png" data-linked-resource-id="7504265" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nome: <strong>CRE - Contenuto più consigliato</strong></li> 
     <li>Tipo: <strong>Tabella</strong><br></li> 
     <li>Visualizza le colonne seguenti: <br><strong>Titolo pagina | Pageviews</strong><br></li> 
     <li>Filtri:<br>Filtro: <strong>[Mostra solo] Pagina (contenente): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a51.png" data-linked-resource-id="7504266" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nome: <strong>Pagine / Sessione (Coinvolgimento)</strong></li> 
     <li>Tipo: <strong>2.1 Metrica </strong></li> 
     <li>Mostra la metrica seguente: <strong>Pagine/Sessione</strong></li> 
     <li>Filtri:<br><strong>[Mostra solo] Categoria evento (esattamente corrispondente): Campagne RTP</strong></li> 
     <li><strong>[Mostra solo] Azione evento (esattamente corrispondente): impression</strong></li> 
     <li><strong>[non mostrare] Etichetta evento (contenente): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a10.png" data-linked-resource-id="7504267" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>Pagine / Sessione (Clickthrough)</strong></li> 
     <li>Tipo: <strong>2.1 Metrica </strong></li> 
     <li>Mostra la metrica seguente: <strong>Pagine/Sessione</strong></li> 
     <li>Filtri:<br><strong>[Mostra solo] Categoria evento (esattamente corrispondente): Campagne RTP</strong></li> 
     <li><strong>[Mostra solo] Azione evento (esattamente corrispondente): click</strong></li> 
     <li><strong>[non mostrare] Etichetta evento (contenente): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a42-3a32.png" data-linked-resource-id="7504268" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nome: <strong>Impressioni di CTA</strong></li> 
     <li>Tipo: <strong>Tabella</strong></li> 
     <li>Visualizza le colonne seguenti: <strong>Etichetta evento | Totale eventi | Utenti</strong></li> 
     <li>Filtri:<br><strong>[Mostra solo] Categoria evento (esattamente corrispondente): Campagne RTP</strong><br><strong>[Mostra solo] Azione evento (esattamente corrispondente): impression</strong><strong>[non mostrare] Etichetta evento (contenente): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a48.png" data-linked-resource-id="7504269" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>Clickthrough da CTA</strong></li> 
     <li>Tipo: <strong>Tabella</strong></li> 
     <li>Visualizza le colonne seguenti: <strong>Etichetta evento | Totale eventi | Utenti</strong></li> 
     <li>Filtri:<br><strong>[Mostra solo] Categoria evento (esattamente corrispondente): Campagne RTP</strong><br><strong>[Mostra solo] Azione evento (esattamente corrispondente): click</strong></li> 
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
