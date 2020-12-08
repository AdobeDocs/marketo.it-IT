---
unique-page-id: 4720108
description: Abilita la barra delle raccomandazioni sul contenuto - Documenti Marketo - Documentazione sul prodotto
title: Abilita la barra delle raccomandazioni del contenuto
translation-type: tm+mt
source-git-commit: 3c24395e55c756184615941327e15e050fa7d0ac
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---


# Abilita la barra delle raccomandazioni del contenuto {#enable-the-content-recommendation-bar}

Content Recommendation Engine utilizza gli algoritmi di analisi predittiva e machine learning per distribuire contenuti pertinenti a ogni visitatore Web. Il motore di raccomandazione prevede quale contenuto eseguirebbe meglio per visitatore. Il contenuto del motore è monitorato e controllato nella pagina Recommendations, aiutando a ottimizzare il ROI del contenuto.

>[!NOTE]
>
>**Prerequisiti**
>
>Prima di abilitare il contenuto predittivo, dovete:
>
>* [Preparare il contenuto predittivo](http://docs.marketo.com/display/docs/edit+predictive+content)
>* [Approvare un titolo per il contenuto predittivo](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)


## Abilitare e personalizzare la barra di raccomandazione del contenuto {#enable-and-customize-the-content-recommendation-bar}

1. Vai a Impostazioni **** contenuto.

   ![](assets/settings-dropdown-hand.png)

1. Fate clic su **Barra**.

   ![](assets/content-settings-bar-hand.png)

1. Per attivare la barra delle raccomandazioni per un URL, fate clic su **Attiva** e quindi su **Salva**.

   ![](assets/bar-enable.png)

1. Per personalizzare un URL, selezionate colori, stile, formato, frecce per la barra delle raccomandazioni e pagine da includere o escludere la barra. Adatta al marchio del sito Web. Fate clic su **Salva**.

   ![](assets/bar-customize-details-hands.png)

   >[!NOTE]
   >
   >**Includi/Escludi URL di visualizzazione**
   >
   >    * L&#39;URL di visualizzazione deve essere il percorso del dominio
   >    * Non includere http:// o https://
   >    * Usa * per i caratteri jolly
   * Usare il punto e virgola come separatore
   * Esempio: /contact_us*; *action=logout*
   * Questo campo fa distinzione tra maiuscole e minuscole


## Considerazioni sulla barra delle raccomandazioni {#recommendation-bar-considerations}

* Affinché il motore di raccomandazione funzioni, è necessario almeno un elemento di contenuto per la barra delle raccomandazioni impostata su **On** nella pagina Recommendations. Se non è attivato alcun contenuto e la barra è impostata su **Attivato**, l&#39;effetto Freccia viene visualizzato nella parte inferiore destra della pagina Web, ma non viene visualizzato alcun contenuto consigliato.

* Maggiore è il contenuto in esecuzione nel motore delle raccomandazioni, migliore sarà l&#39;algoritmo per testare e scoprire quale contenuto funziona meglio. È consigliabile iniziare con 10-20 contenuti in esecuzione e attivi e continuare ad aggiungerne di nuovi.
* Il contenuto abilitato per la raccomandazione deve includere il tag Javascript RTP. Questo consente all&#39;algoritmo di tenere traccia e ottimizzare il contenuto raccomandato.

>[!NOTE]
**Articoli correlati**
* [Abilita contenuto predittivo per contenuti multimediali Web](enable-predictive-content-for-web-rich-media.md)

