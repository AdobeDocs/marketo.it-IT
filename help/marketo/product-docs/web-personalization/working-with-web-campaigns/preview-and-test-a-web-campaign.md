---
unique-page-id: 10092925
description: Anteprima e test di una campagna web - Documenti Marketo - Documentazione del prodotto
title: Anteprima e test di una campagna web
exl-id: 6cc4ebd8-0d39-4a7d-bc3d-e8cd18157470
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 4%

---

# Anteprima e test di una campagna web {#preview-and-test-a-web-campaign}

Questo articolo mostra diversi modi per visualizzare in anteprima una campagna web e anche come testarla utilizzando un segmento di sandbox in tempo reale sul sito web.

>[!NOTE]
>
>L’anteprima mostra solo l’aspetto della campagna sul sito scelto. I collegamenti e i widget non funzioneranno in modo da evitare clic o visualizzazioni errati nell’analisi.

## Visualizzare l’anteprima di una campagna web nella pagina di creazione {#preview-a-web-campaign-on-the-creation-page}

1. Vai a **[!UICONTROL Web Campaigns]**.

   ![](assets/image2016-8-18-15-3a59-3a35.png)

1. Fare clic su **[!UICONTROL Create New Web Campaign]** o sull&#39;icona per modificare una campagna esistente.

   ![](assets/create-new-or-edit-web-campaign.png)

1. In Anteprima sul sito aggiungere l&#39;URL della pagina e fare clic su **[!UICONTROL Preview]**. Viene visualizzata una nuova finestra/scheda con l’anteprima della campagna.

   ![](assets/three-1.png)

   >[!TIP]
   >
   >Fare clic su **[!UICONTROL Share]** per aprire un&#39;e-mail con un URL fisso dell&#39;anteprima della campagna.

   >[!NOTE]
   >
   >È inoltre possibile installare un plug-in del browser ([[!DNL Chrome]](https://chrome.google.com/webstore/detail/marketo-web-personalizati/ldiddonjplchallbngbccbfdfeldohkj) o [[!DNL Firefox]](https://rtp-static.marketo.com/rtp/libs/mwp-0.0.0.8.xpi)) per una migliore esperienza di visualizzazione della campagna. Consulta la sezione seguente.

## Visualizzare l’anteprima di una campagna web nella pagina di creazione utilizzando il plug-in del browser {#preview-a-web-campaign-on-the-creation-page-using-the-browser-plug-in}

1. Seguire i punti 1 e 2 della sezione precedente.

1. Fare clic sul collegamento al plug-in del browser (in questo caso si sta utilizzando [!DNL Chrome]).

   ![](assets/4-1.png)

1. Viene visualizzata una nuova finestra o scheda. Fai clic su **[!UICONTROL Add to Chrome]**.

   ![](assets/five.png)

1. Fai clic su **[!UICONTROL Add Extension]**.

   ![](assets/six.png)

1. Torna a Marketo. Aggiungere l&#39;URL della pagina e fare clic su **[!UICONTROL Preview]**.

   ![](assets/seven.png)

1. Viene visualizzata una nuova finestra/scheda che consente di visualizzare in anteprima l’aspetto della campagna su un desktop, un telefono o un tablet.

   ![](assets/campaign-preview.png)

## Visualizzare l’anteprima di una campagna web nella pagina Campagne web {#preview-a-web-campaign-on-the-web-campaigns-page}

1. Per visualizzare l&#39;elenco delle campagne Web, è sufficiente scegliere una campagna e fare clic sull&#39;icona **[!UICONTROL Preview]**.

   ![](assets/web-campaigns-1-preview-hand.png)

   Facile!

## Visualizzare l’anteprima di una campagna web sul sito web {#preview-a-web-campaign-on-your-website}

Crea un segmento sandbox e una campagna.

1. Vai a **[!UICONTROL Segments]**.

   ![](assets/new-dropdown-segments-hand.jpg)

1. Fai clic su **[!UICONTROL Create New]**.

   ![](assets/image2015-9-10-10-3a42-3a39.png)

1. Denomina il segmento.

1. In [!UICONTROL Behavioral] trascinare [!UICONTROL Include Pages] nell&#39;area di lavoro. Aggiungi il valore &#42;sandbox=1&#42;. Fai clic su **[!UICONTROL Save & Define Campaign]**.

   ![](assets/segment.png)

1. Nella pagina Imposta campagna web, imposta il segmento di destinazione sul segmento sandbox selezionandolo dall’elenco.

   ![](assets/set-web-campaign-target-segment.jpg)

1. Completare la creatività della campagna e fare clic su **[!UICONTROL Launch]**.

   ![](assets/click-launch.jpg)

1. Vai al sito web e aggiungi il parametro URL &quot;?sandbox=1&quot; alla fine dell’URL. Esempio: `www.marketo.com?sandbox=1`.

1. Consulta la reazione alla campagna sul tuo sito web.

>[!NOTE]
>
>Le campagne reagiscono una sola volta durante una sessione del visitatore. Per visualizzare nuovamente la campagna, cancella i cookie del browser.

>[!NOTE]
>
>Non è possibile visualizzare in anteprima le campagne di reindirizzamento. L&#39;unico modo per testarli è utilizzando un segmento di sandbox (destinato a pagine specifiche - &#42;sandbox=redirect&#42;)
