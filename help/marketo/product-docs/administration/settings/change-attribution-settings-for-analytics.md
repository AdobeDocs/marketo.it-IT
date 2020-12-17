---
unique-page-id: 2360217
description: Modifica delle impostazioni di attribuzione per Analytics - Marketo Docs - Documentazione prodotto
title: Modifica delle impostazioni di attribuzione per Analytics
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---


# Modifica delle impostazioni di attribuzione per Analytics {#change-attribution-settings-for-analytics}

Puoi cambiare il modo in cui Marketo collega i contatti alle opportunità per l’attribuzione iniziale e multi-touch, le metriche di conversione principali e il flag delle opportunità influenzato dal marketing.

Queste impostazioni interesseranno i report Revenue Explorer nelle aree [Program Opportunity Analysis](../../../product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Opportunity Analysis](../../../product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md) e Lead Analysis. Questo influirà anche sul rapporto di Program Analyzer.

1. Nella sezione **Admin** fare clic su **Analisi del ciclo di ricavi**.

   ![](assets/image2014-9-24-11-3a55-3a19.png)

1. Fare clic sul collegamento **Modifica** in **Attribuzione**.

   ![](assets/image2014-9-24-11-3a56-3a33.png)

   >[!TIP]
   >
   >La modifica di questa impostazione non modifica i dati Marketo; cambia semplicemente il modo in cui vengono eseguiti i rapporti. Può essere ripristinato in qualsiasi momento.

1. Selezionare un&#39;opzione e fare clic su **Salva**.

   ![](assets/image2014-9-24-11-3a57-3a39.png)

   >[!NOTE]
   >
   >**Definizione**
   >
   >
   >**Esplicito**: Solo i contatti con i ruoli (impostazione predefinita).
   >
   >
   >**Ibrido**: Contatti con i ruoli, se disponibili. Se non ne sono disponibili, vengono utilizzati tutti i contatti presenti negli account.
   >
   >
   >**Implicito**: Tutti i contatti, indipendentemente dal ruolo.

>[!CAUTION]
>
>Quando si utilizza **Implicit**, Marketo esaminerà sempre tutti i contatti associati all&#39;account, indipendentemente dal ruolo. **È consigliabile utilizzare la modalità Explicit.** L&#39;utilizzo di Implicit può creare falsi positivi; ovvero persone che hanno il merito di avere un&#39;opportunità nonostante non abbiano una reale influenza sull&#39;opportunità. Utilizzate Implicit con cautela.

