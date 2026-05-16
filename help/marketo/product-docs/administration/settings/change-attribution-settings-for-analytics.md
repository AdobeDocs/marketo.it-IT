---
unique-page-id: 2360217
description: Come impostare le opzioni di attribuzione di primo e più contatti, conversione dei lead e opportunità influenzate dal marketing in Revenue Cycle Analytics.
title: Modificare le impostazioni di attribuzione per Analytics
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
feature: Administration
TQID: https://experienceleague.adobe.com/AjpEYRzLKRQQsTmYdQUvAVnlcmG-Q6nbVjaZCuQYaUc
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
subfeature_v2:
  - id: e5d29014-8a81-4c0c-845b-2adc7a5d6258
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 160
ht-degree: 9%

---

# Modificare le impostazioni di attribuzione per Analytics {#change-attribution-settings-for-analytics}

Puoi modificare il modo in cui Marketo collega i contatti alle opportunità di attribuzione di primo e più contatti, alle metriche di conversione dei lead e al flag di opportunità influenzato dal marketing.

1. Passa alla schermata **[!UICONTROL Admin]**.

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. Fai clic su **[!UICONTROL Revenue Cycle Analytics]**.

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. Fare clic sul collegamento **[!UICONTROL Edit]** in **[!UICONTROL Attribution]**.

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >La modifica di questa impostazione non comporta la modifica di alcun dato di Marketo, ma modifica il modo in cui vengono eseguiti i rapporti. Questa funzione può essere ripristinata in qualsiasi momento.

1. Selezionare un&#39;opzione e fare clic su **[!UICONTROL Save]**.

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**Definizione**
   >
   >**[!UICONTROL Explicit]**: solo contatti con ruoli (impostazione predefinita).
   >
   >**[!UICONTROL Hybrid]**: contatti con i ruoli, se disponibili. Se non ne è disponibile alcuno, vengono utilizzati tutti i contatti negli account.
   >
   >**[!UICONTROL Implicit]**: tutti i contatti indipendentemente dal ruolo.

>[!CAUTION]
>
>Quando si utilizza **[!UICONTROL Implicit]**, Marketo esaminerà sempre tutti i contatti associati all&#39;account, indipendentemente dal ruolo. **Marketo consiglia di utilizzare la modalità [!UICONTROL Explicit]**. L&#39;utilizzo di [!UICONTROL Implicit] può creare falsi positivi, ovvero persone che hanno il merito di un&#39;opportunità pur non avendo una reale influenza su di essa. Usare [!UICONTROL Implicit] con cautela.
