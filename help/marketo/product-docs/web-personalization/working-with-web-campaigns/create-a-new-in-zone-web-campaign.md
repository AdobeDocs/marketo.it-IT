---
unique-page-id: 4719400
description: Creare una nuova campagna Web in zona - Marketo Docs - Documentazione prodotto
title: Creare una nuova campagna Web nella zona
translation-type: tm+mt
source-git-commit: b33f5ed707a1377daad51191cc6dd9f093138258
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---


# Creare una nuova campagna Web nella zona {#create-a-new-in-zone-web-campaign}

Una campagna Web è una reazione personalizzata associata a un segmento specifico e può essere una [finestra di dialogo](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) sul sito Web, una sostituzione della zona, una [funzione widget](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md) o un avviso e-mail. Una campagna Web In Zone sostituisce un elemento del sito Web basato sull&#39;ID zona con contenuti o banner grafici.

## Creazione di una campagna Web nella zona {#create-an-in-zone-web-campaign}

1. Vai a **Campagne Web**.

   ![](assets/image2016-8-18-15-3a54-3a21.png)

1. Selezionare **Crea nuova campagna Web.**

   ![](assets/create-new-web-campaign-hand.png)

1. Selezionare il tipo di campagna **In Zone**. Personalizzare e aggiungere un **ID zona.** Impostate la campagna su  **** Stickyy e aggiungete i vostri creativi nell&#39;editor. Aggiungete l&#39;URL della pagina da visualizzare in anteprima e fate clic su **Anteprima** per vedere come reagirà la campagna sul sito.

   ![](assets/new-3-1.png)

   >[!NOTE]
   >
   >**Cos&#39;è un ID di zona?**
   >
   >L&#39;ID di zona è il punto in cui si desidera che la campagna Web &quot;In Zone&quot; si trovi sul sito. Per trovare un &quot;ID zona&quot;, basta andare al sito Web e selezionare l&#39;area da sostituire con una campagna Web e fare clic con il pulsante destro del mouse. In Chrome, l&#39;opzione è &quot; elemento Inspect&quot;, in altri browser può variare.
   >
   >Quindi, desiderate trovare l&#39;&quot;id&quot; associato a questa sezione del sito Web, che viene evidenziato perché state ispezionando quell&#39;elemento. Ad esempio, se dopo aver fatto clic con il pulsante destro del mouse in Chrome, il testo evidenziato riporta `<div id="featured-slider">`, &quot;featured-slider&quot; è quello che dovrebbe essere digitato nella sezione &quot;zone id&quot;. In genere viene utilizzato &quot;div id&quot;, ma è possibile utilizzare anche qualsiasi ID, ad esempio h1 id, p id e così via.

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
   <td colspan="1" rowspan="1"><p>Immettete il nome dell’ID trovato nel codice HTML dell’elemento del sito Web che la campagna sostituisce.</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> Sticky </strong></p></td> 
   <td colspan="1" rowspan="1">La casella di controllo Sticky (Sticky) è selezionata per impostazione predefinita per la campagna In Zone (In Zone) e mantiene la campagna In Zone (In Zone) nella sua posizione ID Zona per tutta la sessione del visitatore sul sito Web. Si consiglia di impostare sempre l'opzione Nella zona su Sticky.</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> Dissolvenza</strong> </p></td> 
   <td colspan="1" rowspan="1">Selezionando la casella di controllo Usa effetto e la dissolvenza si verifica un effetto di dissolvenza nell’area ID zona del sito Web. Se l'area di attacco è un banner grafico, la pagina viene caricata e la campagna viene attivata con un effetto di dissolvenza.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>Scorrevole</strong></td> 
   <td colspan="1">Selezionando la casella di controllo Usa effetto e l’opzione Scorrimento viene applicato un effetto di scorrimento all’area ID zona del sito Web. Se l'area di attacco è un banner grafico, la pagina viene caricata e quindi la campagna viene attivata con un effetto di scorrimento da sinistra a destra.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> Editor Rich Text  </strong></td> 
   <td colspan="1">L’editor Rich Text consente la formattazione del testo, il collegamento e l’inserimento di immagini. <a href="/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md">Leggi tutto qui</a> .</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> Anteprima sul sito   </strong></td> 
   <td colspan="1">Anteprima delle campagne prima del loro avvio. <br> 
    <ul> 
     <li> URL - Immettete un URL di esempio in cui verrebbe eseguita la campagna per visualizzare un esempio di anteprima dell'aspetto della campagna in diretta.</li> 
     <li>Dispositivo - Anteprima dell'aspetto della campagna in base al dispositivo: Desktop, Verticale Mobile, Orizzontale Mobile, Verticale Tablet, Orizzontale Verticale.</li> 
     <li> Anteprima - Fare clic su <strong>Anteprima</strong> per aprire una nuova finestra dell'URL di esempio per vedere come reagisce la campagna.</li> 
     <li> Condivisione - Utilizzate il pulsante Condividi per inviare un'e-mail a un collega con un collegamento per visualizzare la campagna proxy.</li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Velocizzate e semplificate il processo di creazione delle campagne utilizzando i nostri [modelli integrati](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) o [salvando la campagna esistente](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) come modello da riutilizzare.

>[!NOTE]
>
>**Vuoi testare A/B le tue campagne web?** Una o più campagne Web possono essere testate  [A/B per ottenere risultati](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/ab-test-your-web-campaign.md) ottimali. Con la funzione Auto-Tune, la piattaforma riconosce automaticamente le campagne più performanti, continua con le campagne di conversione più elevate e mette in pausa le altre.

## Modifica di una campagna Web {#edit-a-web-campaign}

Dalla pagina **Campagne Web**, fare clic su **Modifica** nella campagna.

![](assets/in-zone-web-campaign-edit.png)

>[!NOTE]
>
>Per trovare più facilmente la campagna desiderata, utilizzate la [funzione filtro](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/filter-web-campaigns.md).

## Anteprima di una campagna Web {#preview-a-web-campaign}

1. Dalla pagina Campagne Web, fare clic su **Anteprima** nella campagna Web che si desidera visualizzare.

   ![](assets/in-zone-web-campaign-preview.png)

## Clona una campagna Web {#clone-a-web-campaign}

Vedere [Clonare una campagna Web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/clone-a-web-campaign.md).

## Eliminare una campagna Web {#delete-a-web-campaign}

1. Nella pagina Campagne Web, fare clic su **Elimina** nella campagna da eliminare.

   ![](assets/in-zone-web-campaign-delete.png)

1. Viene visualizzato un messaggio di conferma per confermare se si desidera eliminare la campagna.

>[!MORELIKETHIS]
>
>* [Creare una nuova campagna Web Widget](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
>* [Creazione di una nuova finestra di dialogo Web Campaign](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)

