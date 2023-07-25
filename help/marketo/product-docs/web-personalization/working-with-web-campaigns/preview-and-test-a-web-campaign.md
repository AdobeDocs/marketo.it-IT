---
unique-page-id: 10092925
description: Anteprima e test di una campagna web - Documenti Marketo - Documentazione del prodotto
title: Anteprima e test di una campagna web
exl-id: 6cc4ebd8-0d39-4a7d-bc3d-e8cd18157470
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Anteprima e test di una campagna web {#preview-and-test-a-web-campaign}

Questo articolo mostra diversi modi per visualizzare in anteprima una campagna web e anche come testarla utilizzando un segmento di sandbox in tempo reale sul sito web.

>[!NOTE]
>
>L’anteprima mostra solo l’aspetto della campagna sul sito scelto. I collegamenti e i widget non funzioneranno in modo da evitare clic o visualizzazioni errati nell’analisi.

## Visualizzare l’anteprima di una campagna web nella pagina di creazione {#preview-a-web-campaign-on-the-creation-page}

1. Vai a **Campagne web**.

   ![](assets/image2016-8-18-15-3a59-3a35.png)

1. Clic **Crea nuova campagna web** oppure l’icona per modificare una campagna esistente.

   ![](assets/create-new-or-edit-web-campaign.png)

1. In Anteprima sul sito, aggiungi l’URL della pagina e fai clic su **Anteprima**. Viene visualizzata una nuova finestra/scheda con l’anteprima della campagna.

   ![](assets/three-1.png)

   >[!TIP]
   >
   >Clic **Condividi** per aprire un messaggio e-mail con un URL fisso dell’anteprima della campagna.

   >[!NOTE]
   >
   >È inoltre possibile installare un plug-in del browser (uno [Chrome](https://chrome.google.com/webstore/detail/marketo-web-personalizati/ldiddonjplchallbngbccbfdfeldohkj) o [Firefox](https://rtp-static.marketo.com/rtp/libs/mwp-0.0.0.8.xpi)) per una migliore esperienza nell’anteprima della campagna. Consulta la sezione seguente.

## Visualizzare l’anteprima di una campagna web nella pagina di creazione utilizzando il plug-in del browser {#preview-a-web-campaign-on-the-creation-page-using-the-browser-plug-in}

1. Seguire i punti 1 e 2 della sezione precedente.

1. Fai clic sul collegamento al plug-in del browser (in questo caso si utilizza Chrome).

   ![](assets/4-1.png)

1. Viene visualizzata una nuova finestra o scheda. Clic **Aggiungi a Chrome**.

   ![](assets/five.png)

1. Clic **Aggiungi estensione**.

   ![](assets/six.png)

1. Torna a Marketo. Aggiungi l’URL della pagina e fai clic su **Anteprima**.

   ![](assets/seven.png)

1. Viene visualizzata una nuova finestra/scheda che consente di visualizzare in anteprima l’aspetto della campagna su un desktop, un telefono o un tablet.

   ![](assets/campaign-preview.png)

## Visualizzare l’anteprima di una campagna web nella pagina Campagne web {#preview-a-web-campaign-on-the-web-campaigns-page}

1. Osservando l’elenco delle campagne web, è sufficiente scegliere una campagna e fare clic sul pulsante **Anteprima** icona.

   ![](assets/web-campaigns-1-preview-hand.png)

   Facile!

## Visualizzare l’anteprima di una campagna web sul sito web {#preview-a-web-campaign-on-your-website}

Crea un segmento sandbox e una campagna.

1. Vai a **Segmenti**.

   ![](assets/new-dropdown-segments-hand.jpg)

1. Clic **Crea nuovo**.

   ![](assets/image2015-9-10-10-3a42-3a39.png)

1. Denomina il segmento.

1. In Comportamento trascinare Includi pagine nell&#39;area di lavoro. Aggiungi il valore &#42;sandbox=1&#42;. Clic **Salva e definisci campagna**.

   ![](assets/segment.png)

1. Nella pagina Imposta campagna web, imposta il segmento di destinazione sul segmento sandbox selezionandolo dall’elenco.

   ![](assets/set-web-campaign-target-segment.jpg)

1. Completa la creatività della campagna e fai clic su **Launch**.

   ![](assets/click-launch.jpg)

1. Vai al sito web e aggiungi il parametro URL &quot;?sandbox=1&quot; alla fine dell’URL. Esempio: `www.marketo.com?sandbox=1`.

1. Consulta la reazione alla campagna sul tuo sito web.

>[!NOTE]
>
>Le campagne reagiscono una sola volta durante una sessione del visitatore. Per visualizzare nuovamente la campagna, cancella i cookie del browser.

>[!NOTE]
>
>Non è possibile visualizzare in anteprima le campagne di reindirizzamento. L’unico modo per testarli è utilizzando un segmento di sandbox (che esegue il targeting per pagine specifiche). &#42;sandbox=redirect&#42;)
