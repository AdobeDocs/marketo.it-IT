---
unique-page-id: 10092925
description: Anteprima e test di una campagna Web - Marketo Docs - Documentazione prodotto
title: Anteprima e test di una campagna Web
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---


# Visualizzare in anteprima e testare una campagna Web {#preview-and-test-a-web-campaign}

Questo articolo mostra diversi modi per visualizzare l’anteprima di una campagna Web, nonché come testarla utilizzando un segmento sandbox live sul sito Web.

## Visualizzare l&#39;anteprima di una campagna Web nella pagina di creazione {#preview-a-web-campaign-on-the-creation-page}

1. Andate a **Web** **Campaigns**.

   ![](assets/image2016-8-18-15-3a59-3a35.png)

1. Fare clic su** Crea nuova campagna Web******* o sull&#39;icona per modificare una campagna esistente.

   ![](assets/create-new-or-edit-web-campaign.png)

1. In Anteprima sul sito, aggiungete l&#39;URL della pagina e fate clic su **Anteprima**. Viene visualizzata una nuova finestra/scheda con l’anteprima della campagna.

   ![](assets/three-1.png)

   >[!TIP]
   >
   >Fate clic su **Condividi** per aprire un&#39;e-mail con un URL fisso dell&#39;anteprima della campagna.

   >[!NOTE]
   >
   >Potete anche installare un plug-in del browser ([Chrome](https://chrome.google.com/webstore/detail/marketo-web-personalizati/ldiddonjplchallbngbccbfdfeldohkj) o [Firefox](https://docs.marketo.com/display/docs/assets/mwp-0.0.0.8.xpi)) per ottenere la migliore esperienza di visualizzazione dell&#39;anteprima della campagna. Vedere la sezione seguente.

## Visualizzare l&#39;anteprima di una campagna Web nella pagina di creazione utilizzando il plug-in del browser {#preview-a-web-campaign-on-the-creation-page-using-the-browser-plug-in}

1. Seguite i passaggi 1 e 2 dal percorso `section above`.
1. Fate clic sul collegamento al plug-in del browser (in questo caso stiamo utilizzando Chrome).

   ![](assets/4-1.png)

1. Si apre una nuova finestra/scheda. Fare clic su **Aggiungi a Chrome**.

   ![](assets/five.png)

1. Fate clic su **Aggiungi estensione**.

   ![](assets/six.png)

1. Torna a Marketo. Aggiungete l&#39;URL della pagina e fate clic su **Anteprima**.

   ![](assets/seven.png)

1. Si apre una nuova finestra/scheda che consente di visualizzare l&#39;anteprima dell&#39;aspetto della campagna su un computer desktop, un telefono o un tablet.

   ![](assets/campaign-preview.png)

## Anteprima di una campagna Web nella pagina Campagne Web {#preview-a-web-campaign-on-the-web-campaigns-page}

1. Osservando l&#39;elenco delle campagne Web, è sufficiente scegliere una campagna e fare clic sull&#39;icona **Preview**.

   ![](assets/web-campaigns-1-preview-hand.png)

   Facile!

## Visualizzare in anteprima una campagna Web sul sito Web {#preview-a-web-campaign-on-your-website}

Crea un segmento e una campagna sandbox.

1. Vai a **Segments**.

   ![](assets/new-dropdown-segments-hand.jpg)

1. Fare clic su **Crea nuovo**.

   ![](assets/image2015-9-10-10-3a42-3a39.png)

1. Denominate il segmento.
1. In Comportamento, trascinare Includi pagine nel quadro. Aggiungete il valore *sandbox=1*. Fate clic su Salva e definisci campagna.

   ![](assets/segment.png)

1. Nella pagina Imposta campagna Web, modifica il segmento Target nel segmento sandbox selezionandolo dall&#39;elenco.

   ![](assets/set-web-campaign-target-segment.jpg)

1. Completate la campagna creativa e fate clic su **Avvia**.\
   ![](assets/click-launch.jpg)

1. Andate al sito Web, aggiungete il parametro URL &quot;?sandbox=1&quot; alla fine dell’URL. Esempio: [www.marketo.com?sandbox=1](https://www.marketo.com/?sandbox=1)
1. Visualizzate la reazione della campagna sul vostro sito Web.

>[!NOTE]
>
>Le campagne reagiscono una sola volta durante una sessione del visitatore. Per visualizzare nuovamente la campagna, cancellare i cookie del browser.

>[!NOTE]
>
>Impossibile visualizzare l&#39;anteprima delle campagne di reindirizzamento. L&#39;unico modo per testarli è utilizzare un segmento sandbox (che esegue il targeting per pagine specifiche - *sandbox=redirect*)

