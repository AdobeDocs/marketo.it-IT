---
unique-page-id: 2360389
description: Rendere disponibile un programma senza un costo del periodo in Esplora ricavi e analisti - Marketo Docs - Documentazione del prodotto
title: Rendere disponibile un programma senza un costo del periodo in Esplora ricavi e analisti
exl-id: 45a24b9f-d92f-4f48-a7d1-0be14cd128b1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Rendere disponibile un programma senza un costo del periodo in Esplora ricavi e analisti {#make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers}

I costi del periodo di programma consentono di definire &quot;Quanto denaro&quot; e &quot;Quando&quot; per un programma. Questo viene visualizzato in Revenue Cycle Explorer e [analizzatori](/help/marketo/product-docs/reporting/revenue-cycle-analytics/opportunity-influence-analyzer/tell-the-marketing-story-with-an-opportunity-influence-analyzer.md).

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Alcuni programmi possono dover essere inclusi anche se non hanno un costo di periodo. Sebbene sia possibile immettere 0 per il costo del periodo, è stato più semplice includere questi programmi.

>[!NOTE]
>
>Analisi programma esegue il bucket Programma con successo per costo del periodo. Se non è disponibile alcun costo del periodo, il successo del programma non verrà visualizzato, indipendentemente dal comportamento di analisi del programma. Se è impostato il comportamento di analisi, i dati verranno visualizzati per le metriche delle opportunità (opportunità di pipeline, ricavi ottenuti, ecc.).

1. Nella sezione Amministrazione , fai clic su **Tag**.

   ![](assets/image2014-9-17-12-3a35-3a32.png)

1. Espandi i canali e fai doppio clic sul canale desiderato.

   >[!NOTE]
   >
   >Tutti i programmi che utilizzano questo canale, indipendentemente dal costo del periodo, saranno disponibili per l&#39;explorer dei ricavi e gli analizzatori. Questa modifica entrerà in vigore il giorno successivo.

   ![](assets/image2014-9-17-12-3a36-3a7.png)

1. Cambia il comportamento di Analytics in Inclusivo e fai clic su **Salva**.

   ![](assets/image2014-9-17-12-3a36-3a13.png)

>[!TIP]
>
>Hai notato l&#39;opzione Operativa? Questo fa il contrario. Esso esclude tali programmi indipendentemente dal costo del periodo.

Bel lavoro! Ora qualsiasi programma che utilizza il canale modificato sarà incluso in Revenue explorer e analyzers senza la necessità di un costo di periodo.

>[!MORELIKETHIS]
>
>[Ignorare il comportamento di Analytics a livello di programma](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/override-analytics-behavior-at-the-program-level.md)
