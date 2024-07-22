---
unique-page-id: 2360217
description: Modificare le impostazioni di attribuzione per Analytics - Documentazione di Marketo - Documentazione del prodotto
title: Modificare le impostazioni di attribuzione per Analytics
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 0%

---

# Modificare le impostazioni di attribuzione per Analytics {#change-attribution-settings-for-analytics}

Puoi modificare il modo in cui Marketo collega i contatti alle opportunità di attribuzione di primo e più contatti, alle metriche di conversione dei lead e al flag di opportunità influenzato dal marketing.

Queste impostazioni influiranno sui report di [!UICONTROL Gestione ricavi] nelle aree [Analisi opportunità programma](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Analisi opportunità](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md) e Analisi lead. Questo problema riguarda anche il report [!UICONTROL Analisi programmi].

1. Vai all&#39;area **[!UICONTROL Amministratore]**.

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. Fare clic su **[!UICONTROL Analisi ciclo ricavi]**.

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. Fai clic sul collegamento **[!UICONTROL Modifica]** in **[!UICONTROL Attribuzione]**.

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >La modifica di questa impostazione non comporta la modifica di alcun dato di Marketo, ma semplicemente modifica il modo in cui vengono eseguiti i rapporti. Questa funzione può essere ripristinata in qualsiasi momento.

1. Seleziona un&#39;opzione e fai clic su **[!UICONTROL Salva]**.

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**Definizione**
   >
   >**[!UICONTROL Esplicito]**: solo contatti con ruoli (impostazione predefinita).
   >
   >**[!UICONTROL Ibrido]**: contatti con i ruoli, se disponibili. Se non ne è disponibile alcuno, vengono utilizzati tutti i contatti negli account.
   >
   >**[!UICONTROL Implicito]**: tutti i contatti, indipendentemente dal ruolo.

>[!CAUTION]
>
>Quando si utilizza **[!UICONTROL Implicit]**, Marketo esaminerà sempre tutti i contatti associati all&#39;account indipendentemente dal ruolo. **Marketo consiglia vivamente di utilizzare la modalità [!UICONTROL Explicit]**. L&#39;utilizzo di [!UICONTROL Implicit] può creare falsi positivi, ovvero persone che hanno il merito di un&#39;opportunità pur non avendo una reale influenza sull&#39;opportunità stessa. Usare [!UICONTROL Implicit] con cautela.
