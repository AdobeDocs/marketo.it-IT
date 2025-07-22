---
unique-page-id: 7504238
description: Dashboard RTP personalizzati in Google Universal Analytics - Documentazione Marketo - Documentazione del prodotto
title: Dashboard RTP personalizzati in Google Universal Analytics
exl-id: 712c71b6-74eb-4743-9ca8-50c912278e62
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '750'
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

1. Accedi a Google Analytics. Fai clic su **[!UICONTROL Reporting]** nel menu principale. Fare clic su **[!UICONTROL Dashboards]** e **[!UICONTROL New Dashboard]**.

   ![](assets/image2015-3-22-16-3a41-3a29.png)

1. Seleziona **Area di lavoro vuota**, aggiungi **Nome dashboard** e fai clic su **[!UICONTROL Create Dashboard]**.

1. Fare clic su **[!UICONTROL Add Widget]** per creare un nuovo widget.

   ![](assets/image2015-3-22-16-3a46-3a48.png)

## Dashboard B2B RTP {#rtp-b-b-dashboard}

Questa dashboard consente agli utenti di analizzare le prestazioni del sito web dal punto di vista B2B.

Fornisce informazioni come il comportamento all’origine delle visite e sul sito per settore, ricavi, dimensioni, elenchi basati su account e segmenti di destinazione.

Il dashboard è costituito da 3 colonne

* Traffic source
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
    <div> <strong>Colonna 3 - Espansione firmware</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Nome: sessioni per segmenti e canali</li> 
     <li>Tipo widget: <span class="uicontrol">Barra</span><br></li> 
     <li><span class="uicontrol">Crea un grafico a barre </span>: <span class="uicontrol">Sessione</span></li> 
     <li><span class="uicontrol">Raggruppato per</span>: <span class="uicontrol">Etichetta evento</span></li> 
     <li><span class="uicontrol">Pivot di</span>: <span class="uicontrol">Raggruppamento canali predefinito</span></li> 
     <li>Filtro: <br><span class="uicontrol">Mostra solo</span> | <span class="uicontrol">Categoria eventi</span> (<span class="uicontrol">contenente</span>) segmenti RTP</li> 
    </ul><p><img width="300" src="assets/image2015-3-23-11-3a32-3a13.png" data-linked-resource-id="7504247" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: numero di utenti RTP segmentati</li> 
     <li>Tipo: <span class="uicontrol">2.1 Metrica</span></li> 
     <li><span class="uicontrol">Mostra la metrica seguente</span>: <span class="uicontrol">Utenti</span><br></li> 
     <li>Filtro: <br><span class="uicontrol">Mostra solo</span> | <span class="uicontrol">Categoria eventi</span> (contenente) segmenti RTP</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a6.png" data-linked-resource-id="7504249" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: sessioni per settore</li> 
     <li>Tipo: <span class="uicontrol">Torta</span><br></li> 
     <li><span class="uicontrol">Crea un grafico a torta </span>: <span class="uicontrol">Sessioni</span></li> 
     <li><span class="uicontrol">Raggruppato per</span>: <span class="uicontrol">RTP-Industry</span></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a27.png" data-linked-resource-id="7504250" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <th> 
    <ul> 
     <li><strong>Nome: sessioni per settore e canali</strong></li> 
     <li><strong>Tipo widget: <span class="uicontrol">Barra</span></strong></li> 
     <li><strong><span class="uicontrol">Crea un grafico a barre </span>: <span class="uicontrol">Sessione</span></strong></li> 
     <li><strong><span class="uicontrol">Raggruppato per</span>: <span class="uicontrol">RTP-Industry</span></strong></li> 
     <li><strong><span class="uicontrol">Pivot di</span>: <span class="uicontrol">Raggruppamento canali predefinito</span></strong><br><img width="300" src="assets/image2015-3-23-11-3a33-3a52.png" data-linked-resource-id="7504252" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></li> 
    </ul></th> 
   <th> 
    <ul> 
     <li><strong>Nome: sessioni segmentate per paese</strong></li> 
     <li><strong>Tipo: <span class="uicontrol">Geomap</span></strong></li> 
     <li><strong><span class="uicontrol">Traccia la metrica selezionata</span>: <span class="uicontrol">Paese</span> | <span class="uicontrol">Sessioni</span></strong></li> 
     <li><strong><span class="uicontrol">Seleziona una regione</span>: <span class="uicontrol">Il mondo</span></strong></li> 
     <li><strong>Filtro: <span class="uicontrol">Mostra solo</span> | <span class="uicontrol">Categoria eventi</span> (contenente) segmenti RTP</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a34-3a18.png" data-linked-resource-id="7504253" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li><strong>Nome: sessioni per categoria RTP</strong></li> 
     <li><strong>Tipo: <span class="uicontrol">Torta</span></strong></li> 
     <li><strong><span class="uicontrol">Crea un grafico a torta </span>: <span class="uicontrol">Sessioni</span></strong></li> 
     <li><strong><span class="uicontrol">Raggruppato per</span>: <span class="uicontrol">Categoria-RTP</span></strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a1.png" data-linked-resource-id="7504254" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nome: Segmenti di destinazione principali</li> 
     <li>Tipo: <span class="uicontrol">Barra</span></li> 
     <li><span class="uicontrol">Crea un grafico a barre </span>: <span class="uicontrol">Utenti</span></li> 
     <li><span class="uicontrol">Raggruppato per</span>: <span class="uicontrol">Azione evento</span></li> 
     <li>Filtro: <span class="uicontrol">Mostra solo</span> | <span class="uicontrol">Categoria eventi</span> (contenente) segmenti RTP</li> 
    </ul><p><img width="350" src="assets/add-a-widget.png" data-linked-resource-id="11382874" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li>Nome: sessioni per gruppi RTP</li> 
     <li>Tipo: barra<br></li> 
     <li>Crea un grafico a barre che mostra: Sessioni</li> 
     <li>Raggruppato per: RTP-Group</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a54.png" data-linked-resource-id="7504256" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nome: sessioni e obiettivi per segmenti principali</li> 
     <li>Tipo: tabella<br></li> 
     <li>Visualizza le colonne seguenti: <br>Etichetta evento | Sessioni | Tasso di conversione obiettivo</li> 
     <li>Filtro: <br>Mostra solo | Categoria evento (contenente) segmenti RTP</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a36-3a15.png" data-linked-resource-id="7504257" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> </th> 
  </tr> 
 </tbody> 
</table>

## Dashboard del coinvolgimento RTP {#rtp-engagement-dashboard}

Questa dashboard consente agli utenti di analizzare le prestazioni della campagna RTP e il coinvolgimento con i motori di consigli. Fornisce un confronto tra media. durata della sessione e pagine per sessione tra:

* Non coinvolto
* Coinvolto (impression e clic su una campagna personalizzata)
* Fai clic sul motore di consigli e sui principali contenuti consigliati

Crea un nuovo dashboard denominato **Dashboard di coinvolgimento RTP** e definisci i seguenti widget:

![](assets/image2015-3-22-17-3a7-3a19.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div> <strong>Esposizione campagne colonna 1</strong> 
    </div></th> 
   <th> 
    <div> <strong>Clickthrough campagne colonna 2</strong> 
    </div></th> 
   <th> 
    <div> <strong>Motore di consigli colonna 3</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Nome: <strong>CTA totale (coinvolgimento)</strong></li> 
     <li>Tipo: <strong>2.1 Metrica </strong></li> 
     <li>Mostra la metrica seguente: <strong>Eventi totali</strong></li> 
     <li>Filtri:<br><strong>[show only] Categoria evento (contiene): RTP-Campaigns</strong><br><strong>[show only] Azione evento (corrispondenza esatta): Impression</strong>[don't show] Etichetta evento (contenente): #</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a37-3a55.png" data-linked-resource-id="7504259" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>Totale CTA (Clickthrough)</strong></li> 
     <li>Tipo: <strong>2.1 Metrica </strong></li> 
     <li>Mostra la metrica seguente: <strong>Eventi totali</strong></li> 
     <li>Filtri:<br><strong>[show only] Categoria evento (contiene): RTP-Campaigns</strong><br><strong>[show only] Azione evento (esattamente corrispondente): Clic</strong><strong>[don't show] Etichetta evento (contenente): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a12.png" data-linked-resource-id="7504261" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>CRE - Clic totali</strong></li> 
     <li>Tipo: <strong><span class="uicontrol">2.1 Metrica</span></strong><br></li> 
     <li><span class="uicontrol">Mostra la metrica seguente</span>: <strong><span class="uicontrol">Visualizzazioni pagina</span></strong></li> 
     <li>Filtro: <strong>[<span class="uicontrol">mostra solo</span>] <span class="uicontrol">Pagina</span> (<span class="uicontrol">contenente</span>): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a30.png" data-linked-resource-id="7504262" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> 
    <ul> 
     <li>Nome: <strong>Media Durata sessione (coinvolgimento)</strong></li> 
     <li>Tipo: <strong>2.1 Metrica </strong></li> 
     <li>Mostra la metrica seguente: <strong>Media Durata sessione</strong></li> 
     <li>Filtri:<br><strong>[show only] Categoria evento (esattamente corrispondente): RTP-Campaigns</strong><br><strong>[only show] Azione evento (esattamente corrispondente): impression</strong><strong>[don't show] Etichetta evento (contenente): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a21.png" data-linked-resource-id="7504264" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nome: <strong>Media Durata sessione (clickthrough)</strong></li> 
     <li>Tipo: <strong>2.1 Metrica </strong></li> 
     <li>Mostra la metrica seguente: <strong>Media Durata sessione</strong></li> 
     <li>Filtri:<br><strong>[show only] Categoria evento (esattamente corrispondente): RTP-Campaigns</strong><br><strong>[only show] Azione evento (esattamente corrispondente): clicks</strong><strong>[don't show] Etichetta evento (contenente): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a37.png" data-linked-resource-id="7504265" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nome: <strong>CRE - Contenuto consigliato principale</strong></li> 
     <li>Tipo: <strong><span class="uicontrol">Tabella</span></strong><br></li> 
     <li><span class="uicontrol">Visualizza le colonne seguenti</span>: <br><strong><span class="uicontrol">Titolo pagina</span> | <span class="uicontrol">Visualizzazioni pagina</span></strong><br></li> 
     <li>Filtri:<br>Filtro: <strong>[<span class="uicontrol">mostra solo</span>] <span class="uicontrol">Pagina</span> (<span class="uicontrol">contenente</span>): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a51.png" data-linked-resource-id="7504266" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nome: <strong>Pagine/Sessione (Coinvolgimento)</strong></li> 
     <li>Tipo: <strong><span class="uicontrol">2.1 Metrica</span> </strong></li> 
     <li><span class="uicontrol">Mostra la metrica seguente</span>: <strong><span class="uicontrol">Pagine / Sessione</span></strong></li> 
     <li>Filtri:<br><strong>[<span class="uicontrol">mostra solo</span>] <span class="uicontrol">Categoria evento</span> (<span class="uicontrol">corrisponde esattamente</span>): RTP-Campaigns</strong></li> 
     <li><strong>[<span class="uicontrol">only show</span>] <span class="uicontrol">Azione evento</span> (<span class="uicontrol">esattamente corrispondente</span>): impression</strong></li> 
     <li><strong>[<span class="uicontrol">non mostrare</span>] <span class="uicontrol">Etichetta evento</span> (<span class="uicontrol">contenente</span>): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a10.png" data-linked-resource-id="7504267" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>Pagine / Sessione (Clickthrough)</strong></li> 
     <li>Tipo: <strong>2.1 Metrica </strong></li> 
     <li>Mostra la metrica seguente: <strong>Pagine / Sessione</strong></li> 
     <li>Filtri:<br><strong>[show only] Categoria evento (esattamente corrispondente): RTP-Campaigns</strong></li> 
     <li><strong>[only show] Azione evento (esattamente corrispondente): clic</strong></li> 
     <li><strong>[do not show] Etichetta evento (contenente): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a32.png" data-linked-resource-id="7504268" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nome: <strong>Impression di CTA</strong></li> 
     <li>Tipo: <strong><span class="uicontrol">Tabella</span></strong></li> 
     <li><span class="uicontrol">Visualizza le colonne seguenti</span>: <strong><span class="uicontrol">Etichetta evento</span> | <span class="uicontrol">Eventi totali</span> | <span class="uicontrol">Utenti</span></strong></li> 
     <li>Filtri:<br><strong>[<span class="uicontrol">solo mostra</span>] <span class="uicontrol">Categoria evento</span> (<span class="uicontrol">esattamente corrispondente</span>): RTP-Campaigns</strong><br><strong>[<span class="uicontrol">solo mostra</span>] <span class="uicontrol">Azione evento</span> (<span class="uicontrol">esattamente corrispondente</span>): impression</strong><strong>[<span class="uicontrol">non mostra</span>] <span class="uicontrol">Etichetta evento</span> (<span class="uicontrol">contenente</span>): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a48.png" data-linked-resource-id="7504269" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>Clickthrough da CTA</strong></li> 
     <li>Tipo: <strong><span class="uicontrol">Tabella</span></strong></li> 
     <li><span class="uicontrol">Visualizza le colonne seguenti</span>: <strong><span class="uicontrol">Etichetta evento</span> | <span class="uicontrol">Eventi totali</span> | <span class="uicontrol">Utenti</span></strong></li> 
     <li>Filtri:<br><strong>[<span class="uicontrol">mostra solo</span>] <span class="uicontrol">Categoria evento</span> (<span class="uicontrol">corrisponde esattamente</span>): RTP-Campaigns</strong><br><strong>[<span class="uicontrol">mostra solo</span>] <span class="uicontrol">Azione evento</span> (<span class="uicontrol">corrisponde esattamente</span>): clic</strong></li> 
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
