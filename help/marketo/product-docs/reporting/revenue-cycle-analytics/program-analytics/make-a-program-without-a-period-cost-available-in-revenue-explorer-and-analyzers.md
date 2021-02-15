---
unique-page-id: 2360389
description: Rendere disponibile un programma senza un costo periodo in Esplora ricavi e analisti - Documenti Marketo - Documentazione prodotto
title: Rendere disponibile un programma senza un costo periodo in Esplora ricavi e analizzatori
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---


# Rendere disponibile un programma senza un costo periodo in Esplora ricavi e analizzatori {#make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers}

I costi del periodo di programma consentono di definire &quot;Quanti soldi&quot; e &quot;Quando&quot; per un programma. Questo viene visualizzato in [prospettore del ciclo di ricavi](https://docs.marketo.com/display/docs/revenue+cycle+analytics) e [analizzatori](../../../../product-docs/reporting/revenue-cycle-analytics/opportunity-influence-analyzer/tell-the-marketing-story-with-an-opportunity-influence-analyzer.md).

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Alcuni programmi potrebbero dover essere inclusi anche se non hanno un costo periodo. Sebbene sia possibile inserire 0 per il costo del periodo, abbiamo reso più semplice l&#39;inclusione di questi programmi.

>[!NOTE]
>
>L&#39;analizzatore del programma esegue il programma Success in base al costo del periodo. Se non è disponibile alcun costo periodo, il Successo programma non verrà visualizzato, indipendentemente dal comportamento di analisi del programma. Se il comportamento di analisi è impostato, i dati verranno visualizzati per le metriche delle opportunità (opportunità di pipeline, ricavi ottenuti, ecc.).

1. Nella sezione Amministratore, fate clic su Tag.

   ![](assets/image2014-9-17-12-3a35-3a32.png)

1. Espandi i canali e fai doppio clic sul canale desiderato.

   >[!NOTE]
   >
   >**Promemoria**
   >
   >Tutti i programmi che utilizzano questo canale, indipendentemente dal costo del periodo, saranno disponibili per gli esperti di analisi delle entrate e gli analizzatori. La modifica avrà effetto il giorno successivo.

   ![](assets/image2014-9-17-12-3a36-3a7.png)

1. Cambia il comportamento di Analytics in Inclusivo e fai clic su Salva.

   ![](assets/image2014-9-17-12-3a36-3a13.png)

>[!TIP]
>
>Avete notato l&#39;opzione Operativa? Questo fa il contrario. Sono esclusi da tali programmi indipendentemente dal costo del periodo.

Bel lavoro! Ora qualsiasi programma che utilizza il canale modificato sarà incluso in elenco ricavi e analizzatori senza la necessità di un costo di periodo.

>[!MORELIKETHIS]
>
>* [Escludi comportamento Analytics a livello di programma](override-analytics-behavior-at-the-program-level.md)

>



