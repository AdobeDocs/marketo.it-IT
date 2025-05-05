---
unique-page-id: 4720108
description: Abilitare la barra dei consigli per i contenuti - Documentazione di Marketo - Documentazione del prodotto
title: Abilitare la barra dei consigli dei contenuti
exl-id: f2244db1-51a9-4e26-9bf7-b2c79df25552
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# Abilitare la barra dei consigli dei contenuti {#enable-the-content-recommendation-bar}

Il motore di raccomandazione dei contenuti utilizza algoritmi di analisi predittiva e di apprendimento automatico per fornire contenuti rilevanti a ogni visitatore web. Il motore di consigli prevede quale contenuto avrebbe le migliori prestazioni per visitatore. Il contenuto del motore viene monitorato e controllato nella pagina Recommendations, consentendoti di ottimizzare il ROI dei contenuti.

>[!PREREQUISITES]
>
>Prima di abilitare il contenuto predittivo, è necessario:
>
>* **Prepara il contenuto predittivo**
>
>   * [Modifica contenuto predittivo per e-mail](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md) o
>   * [Modifica contenuto predittivo per contenuti rich media](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md) o
>   * [Modifica contenuto predittivo per la barra dei consigli](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md)
>
>* [Approva un titolo per il contenuto predittivo](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)

## Abilitare e personalizzare la barra dei consigli dei contenuti {#enable-and-customize-the-content-recommendation-bar}

1. Vai a **Impostazioni contenuto**.

   ![](assets/settings-dropdown-hand.png)

1. Fare clic su **Barra**.

   ![](assets/content-settings-bar-hand.png)

1. Per abilitare la barra dei consigli per un URL, fai clic su **Il** e quindi su **Salva**.

   ![](assets/bar-enable.png)

1. Per personalizzare un URL, seleziona colori, stile, formato, frecce per la barra dei consigli e pagine per includerla o escluderla. Personalizza per adattarti al tuo marchio del sito web. Fai clic su **Salva**.

   ![](assets/bar-customize-details-hands.png)

   >[!NOTE]
   >
   >**Includi/Escludi URL di visualizzazione**
   >
   >* L’URL di visualizzazione deve essere il percorso del dominio
   >* Non includere https:// o https://
   >* Usa &#42; per i caratteri jolly
   >* Utilizzare un punto e virgola come separatore
   >* Esempio: /contact_us&#42;; &#42;action=logout&#42;
   >* Questo campo distingue tra maiuscole e minuscole

## Considerazioni sulla barra dei consigli {#recommendation-bar-considerations}

* È necessario almeno un contenuto per il funzionamento della barra dei consigli impostata su **Il** nella pagina Recommendations. Se non è abilitato alcun contenuto e la barra è impostata su **Il**, l&#39;effetto Freccia verrà visualizzato in basso a destra della pagina Web, ma non verrà visualizzato alcun contenuto consigliato.

* Maggiore è il numero di contenuti in esecuzione nel motore di consigli, migliore sarà la possibilità per l’algoritmo di testare e scoprire quale contenuto funziona meglio. È consigliabile iniziare con 10-20 contenuti in esecuzione e attivi e continuare ad aggiungerne di nuovi.
* La parte di contenuto abilitata per i consigli deve includere il tag JavaScript RTP. In questo modo l’algoritmo può tenere traccia e ottimizzare il contenuto consigliato.

>[!MORELIKETHIS]
>
>[Abilita contenuto predittivo per contenuti multimediali avanzati Web](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
