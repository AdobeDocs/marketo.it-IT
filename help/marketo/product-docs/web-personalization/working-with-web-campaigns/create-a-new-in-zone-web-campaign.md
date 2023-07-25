---
unique-page-id: 4719400
description: Creazione di una nuova campagna web nell’area - Documentazione di Marketo - Documentazione del prodotto
title: Crea una nuova campagna web nell’area
exl-id: 5cbe80a2-5e20-4e35-a722-b4cb479b4df7
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---

# Crea una nuova campagna web nell’area {#create-a-new-in-zone-web-campaign}

Una campagna web è una reazione personalizzata associata a un segmento specifico e può essere una [finestra di dialogo](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) sul sito web, un sostituto di zona, un [funzione widget](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md) o un avviso e-mail. Una campagna web In Zone sostituisce un elemento del sito web basato sull’ID zona con contenuti o banner grafici.

## Creare una campagna web in area {#create-an-in-zone-web-campaign}

1. Vai a **Campagne web**.

   ![](assets/image2016-8-18-15-3a54-3a21.png)

1. Seleziona **Creare una nuova campagna web.**

   ![](assets/create-new-web-campaign-hand.png)

1. Seleziona la **Nella zona** tipo di campagna. Personalizza e aggiungi un **ID zona.** Imposta la campagna su **Sticky** e aggiungi il tuo contenuto creativo nell’editor. Aggiungi l’URL della pagina da visualizzare in anteprima e fai clic su **Anteprima** per vedere come reagirà la campagna sul tuo sito.

   ![](assets/new-3-1.png)

   >[!NOTE]
   >
   >**Che cos&#39;è un ID zona?**
   >
   >Un ID zona è il luogo in cui desideri che la campagna web &quot;In Zone&quot; si trovi sul sito. Per trovare un &quot;ID zona&quot;, vai al tuo sito web e seleziona l’area che desideri sostituire con una campagna web e fai clic con il pulsante destro del mouse. In Chrome, l’opzione è &quot;Inspect Element&quot; (Elemento), ma può variare in altri browser.
   >
   >Quindi, vuoi trovare il &quot;id&quot; associato a questa sezione del sito web, che viene evidenziato perché stai esaminando quell’elemento. Ad esempio, se una volta fatto clic con il pulsante destro del mouse in Chrome il testo evidenziato riporta `<div id="featured-slider">` nella sezione &quot;id zona&quot;, digita quindi &quot;feature-slider&quot;. In genere viene utilizzato &quot;div id&quot;, ma può essere utilizzato anche qualsiasi ID, ad esempio h1 id, p id e così via.

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">Nome</th> 
   <th colspan="1" rowspan="1">Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><strong> ID zona </strong></td> 
   <td colspan="1" rowspan="1"><p>Immetti il nome dell'ID trovato nel codice HTML dell'elemento del sito web che la campagna sostituisce.</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> Sticky </strong></p></td> 
   <td colspan="1" rowspan="1">La casella di controllo Sticky è selezionata per impostazione predefinita per la campagna In Zone e mantiene la campagna In Zone nella sua posizione ID zona per tutta la sessione del visitatore sul sito web. Si consiglia di impostare sempre la zona di entrata su Sticky.</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> Scolorimento</strong> </p></td> 
   <td colspan="1" rowspan="1">Selezionando la casella di controllo Usa effetto e l'opzione Scolorimento si ottiene un effetto di dissolvenza sull'area ID zona del sito Web. Se la zona In è un banner grafico, la pagina viene prima caricata e quindi la campagna si attiva con un effetto di dissolvenza.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>Scorrimento</strong></td> 
   <td colspan="1">Selezionando la casella di controllo Usa effetto e l'opzione Scorrimento, viene attivata una scorrevole per l'area ID zona del sito Web. Se la zona In è un banner grafico, la pagina viene prima caricata e quindi la campagna si attiva con un effetto scorrevole da sinistra a destra.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> Editor Rich Text  </strong></td> 
   <td colspan="1">L’editor Rich Text consente la formattazione del testo, il collegamento e l’inserimento di immagini. <a href="/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md">Fai clic qui per ulteriori informazioni</a> .</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> Anteprima sul sito   </strong></td> 
   <td colspan="1">Visualizza l’anteprima delle campagne prima che vengano avviate. <br> 
    <ul> 
     <li> URL: immetti un URL di esempio in cui eseguire la campagna per visualizzare un esempio di anteprima dell’aspetto della campagna dal vivo.</li> 
     <li>Dispositivo: visualizza in anteprima come verrà visualizzata la campagna per dispositivo: Desktop, Verticale mobile, Orizzontale mobile, Verticale tablet, Orizzontale verticale.</li> 
     <li> Anteprima - Clic <strong>Anteprima</strong> per aprire una nuova finestra dell’URL di esempio per vedere come reagisce la campagna.</li> 
     <li> Condividi: utilizza il pulsante Condividi per inviare un’e-mail a un collega con un collegamento per visualizzare la campagna proxy.</li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Accelera e semplifica il processo di creazione delle campagne utilizzando [modelli incorporati](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) o da [salvataggio della campagna esistente](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) come modello da riutilizzare.

>[!NOTE]
>
>**Desideri testare le tue campagne web?** Una o più campagne web possono essere [Test A/B per risultati ottimali](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/ab-test-your-web-campaign.md). Con la funzione di ottimizzazione automatica, la piattaforma riconosce automaticamente le campagne con prestazioni migliori, continua con le campagne di conversione più elevate e mette in pausa le altre.

## Modificare una campagna web {#edit-a-web-campaign}

Dalla sezione **Campagne web** pagina, fai clic su **Modifica** nella campagna.

![](assets/in-zone-web-campaign-edit.png)

>[!NOTE]
>
>Per trovare più facilmente la campagna desiderata, utilizza [funzione filtro](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/filter-web-campaigns.md).

## Visualizzare l’anteprima di una campagna web {#preview-a-web-campaign}

1. Dalla pagina Campagne web, fai clic su **Anteprima** nella campagna web che desideri visualizzare.

   ![](assets/in-zone-web-campaign-preview.png)

## Clonare una campagna web {#clone-a-web-campaign}

Consulta [Clonare una campagna web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/clone-a-web-campaign.md).

## Eliminare una campagna web {#delete-a-web-campaign}

1. Dalla pagina Campagne web, fai clic su **Elimina** nella campagna che desideri eliminare.

   ![](assets/in-zone-web-campaign-delete.png)

1. Viene visualizzato un messaggio di conferma per confermare se desideri eliminare la campagna.

>[!MORELIKETHIS]
>
>* [Crea una nuova campagna web widget](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
>* [Creare una nuova campagna web per finestre di dialogo](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
