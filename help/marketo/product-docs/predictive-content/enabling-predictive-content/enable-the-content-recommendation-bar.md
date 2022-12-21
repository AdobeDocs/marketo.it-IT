---
unique-page-id: 4720108
description: Abilita la barra dei consigli sul contenuto - Documenti Marketo - Documentazione del prodotto
title: Abilita la barra delle raccomandazioni del contenuto
exl-id: f2244db1-51a9-4e26-9bf7-b2c79df25552
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Abilita la barra delle raccomandazioni del contenuto {#enable-the-content-recommendation-bar}

Il motore di consigli per i contenuti utilizza algoritmi di analisi predittiva e machine learning per fornire contenuti pertinenti a ogni visitatore web. Il motore di raccomandazione prevede quale contenuto avrebbe prestazioni migliori per visitatore. Il contenuto del motore viene monitorato e controllato nella pagina Recommendations, aiutandoti a ottimizzare il ROI dei contenuti.

>[!PREREQUISITES]
>
>Prima di abilitare il contenuto predittivo, devi:
>
>* **Preparare il contenuto predittivo**
   >
   >   * [Modifica del contenuto predittivo per le e-mail](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md) o
   >   * [Modifica di contenuti predittivi per contenuti rich media](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md) o
   >   * [Modifica contenuto predittivo per la barra delle raccomandazioni](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md)
>
>* [Approvare un titolo per il contenuto predittivo](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)


## Abilita e personalizza la barra delle raccomandazioni del contenuto {#enable-and-customize-the-content-recommendation-bar}

1. Vai a **Impostazioni contenuto**.

   ![](assets/settings-dropdown-hand.png)

1. Fai clic su **Barre**.

   ![](assets/content-settings-bar-hand.png)

1. Per abilitare la barra dei consigli per un URL, fai clic su **On** e poi **Salva**.

   ![](assets/bar-enable.png)

1. Per personalizzare un URL, selezionate i colori, lo stile, il formato, le frecce per la barra dei consigli e le pagine da includere o escludere la barra. Personalizza per adattarti al tuo marchio del sito web. Fai clic su **Salva**.

   ![](assets/bar-customize-details-hands.png)

   >[!NOTE]
   >
   >**URL di visualizzazione Includi/Escludi**
   >
   >* L&#39;URL di visualizzazione deve essere il percorso del dominio
   >* Non includere https:// o https://
   >* Utilizzo &#42; per caratteri jolly
   >* Utilizzare un punto e virgola come separatore
   >* Esempio: /contact_us&#42;; &#42;action=logout&#42;
   >* Questo campo è sensibile a maiuscole e minuscole


## Considerazioni sulle barre dei consigli {#recommendation-bar-considerations}

* È necessario almeno un elemento di contenuto per la barra dei consigli impostata su **On** nella pagina Recommendations per il funzionamento del motore di raccomandazioni. Se non è attivato alcun contenuto e la barra è impostata su **On**, l’effetto Freccia viene visualizzato in basso a destra della pagina web, ma non viene visualizzato alcun contenuto consigliato.

* Maggiore è il contenuto in esecuzione nel motore di raccomandazione, migliore sarà l&#39;algoritmo per testare e scoprire quale contenuto funziona meglio. È consigliabile iniziare con 10-20 contenuti in esecuzione e attivi e continuare ad aggiungerne di nuovi.
* Il contenuto abilitato per la raccomandazione deve includere il tag Javascript RTP. Questo consente all’algoritmo di tenere traccia e ottimizzare il contenuto consigliato.

>[!MORELIKETHIS]
>
>[Abilita contenuti predittivi per contenuti multimediali web](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
