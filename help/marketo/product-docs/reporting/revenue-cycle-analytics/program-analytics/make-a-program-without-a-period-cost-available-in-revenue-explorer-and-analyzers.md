---
unique-page-id: 2360389
description: Scopri come rendere disponibile un programma senza un costo di periodo in Esplora ricavi e analizzatori in Marketo Engage. Utilizza questa guida per completare il passaggio successivo.
title: Rendere disponibile un programma senza costo periodo in esploratore ricavi e analizzatori
exl-id: 45a24b9f-d92f-4f48-a7d1-0be14cd128b1
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 50befbf7339cd7a8b25b0942515497f6acc8f9ab
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 11%

---

# Rendere disponibile un programma senza costo periodo in esploratore ricavi e analizzatori {#make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers}

I costi del periodo del programma consentono di definire &quot;Quanto denaro&quot; e &quot;Quando&quot; per un programma. Questo viene visualizzato in Revenue Cycle Explorer e in [analizzatori](/help/marketo/product-docs/reporting/revenue-cycle-analytics/opportunity-influence-analyzer/tell-the-marketing-story-with-an-opportunity-influence-analyzer.md).

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Alcuni programmi possono dover essere inclusi anche se non hanno un costo di periodo. Anche se è possibile immettere 0 per il costo del periodo, è stato semplificato l&#39;inserimento di questi programmi.

>[!NOTE]
>
>L’analizzatore di programmi classifica il successo del programma in base al costo del periodo. Se non è disponibile alcun costo di periodo, il completamento del programma non verrà visualizzato, indipendentemente dal comportamento di analisi del programma. Se il comportamento di analisi è configurato, i dati verranno visualizzati per le metriche delle opportunità (opportunità pipeline, ricavi ottenuti, ecc.).

1. Nella sezione [!UICONTROL Admin] fare clic su **[!UICONTROL Tags]**.

   ![](assets/image2014-9-17-12-3a35-3a32.png)

1. Espandi i tuoi canali e fai doppio clic sul canale desiderato.

   >[!NOTE]
   >
   >Tutti i programmi che utilizzano questo canale, indipendentemente dal costo del periodo, saranno disponibili per gli analizzatori e gli esploratori di ricavi. Questa modifica entrerà in vigore il giorno successivo.

   ![](assets/image2014-9-17-12-3a36-3a7.png)

1. Cambia [!UICONTROL Analytics Behavior] in **Inclusive** e fai clic su **[!UICONTROL Save]**.

   ![](assets/image2014-9-17-12-3a36-3a13.png)

>[!TIP]
>
>Avete notato l&#39;opzione Operational? Questo fa l&#39;opposto. Sono esclusi questi programmi indipendentemente dal costo del periodo.

Bel lavoro! Ora qualsiasi programma che utilizza il canale modificato verrà incluso in Esplora ricavi e analizzatori senza la necessità di un costo di periodo.

>[!MORELIKETHIS]
>
>[Ignora comportamento di Analytics a livello di programma](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/override-analytics-behavior-at-the-program-level.md)
