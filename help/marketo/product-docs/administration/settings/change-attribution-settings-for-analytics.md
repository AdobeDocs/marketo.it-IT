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

Queste impostazioni avranno un impatto [!UICONTROL Gestione ricavi] rapporti in [Analisi opportunità programma](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Analisi dell’opportunità](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md), e Analisi dei lead. Questo inciderà anche sulla [!UICONTROL Analizzatore di programmi] rapporto.

1. Vai a **[!UICONTROL Amministratore]** area.

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. Clic **[!UICONTROL Analisi del ciclo dei ricavi]**.

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. Fai clic su **[!UICONTROL Modifica]** collega in **[!UICONTROL Attribuzione]**.

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >La modifica di questa impostazione non comporta la modifica di alcun dato di Marketo, ma semplicemente modifica il modo in cui vengono eseguiti i rapporti. Questa funzione può essere ripristinata in qualsiasi momento.

1. Seleziona un’opzione e fai clic su **[!UICONTROL Salva]**.

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**Definizione**
   >
   >**[!UICONTROL Esplicito]**: solo contatti con ruoli (impostazione predefinita).
   >
   >**[!UICONTROL Ibrido]**: contatti con i ruoli, se disponibili. Se non ne è disponibile alcuno, vengono utilizzati tutti i contatti negli account.
   >
   >**[!UICONTROL Implicito]**: tutti i contatti indipendentemente dal ruolo.

>[!CAUTION]
>
>Quando si utilizza **[!UICONTROL Implicito]**, Marketo esaminerà sempre tutti i contatti associati all’account, indipendentemente dal ruolo. **Marketo consiglia vivamente di [!UICONTROL Esplicito] modalità**. Utilizzo di [!UICONTROL Implicito] può creare falsi positivi, ovvero persone che hanno il merito di un’opportunità pur non avendo una reale influenza su di essa. Utilizzare [!UICONTROL Implicito] con cautela.
