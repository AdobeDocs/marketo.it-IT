---
unique-page-id: 1147031
description: Elimina persona da SFDC - Documentazione di Marketo - Documentazione del prodotto
title: Elimina persona da SFDC
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---

# Elimina persona da SFDC {#delete-person-from-sfdc}

Se devi rimuovere un set specifico di lead da Salesforce ma lasciarli come persone nel Marketo Engage, puoi utilizzare l’azione di flusso Elimina persona da SFDC.

>[!NOTE]
>
>Disponibile solo se integrato con Salesforce.

1. Nel database, fare clic sulla persona che si desidera rimuovere da Salesforce. Quindi fai clic su **[!UICONTROL Azioni persona]** e seleziona **[!DNL Salesforce]**.

   ![](assets/delete-person-from-sfdc-1.png)

1. Seleziona **[!UICONTROL Elimina persona da SFDC]**.

   ![](assets/delete-person-from-sfdc-2.png)

1. Assicurarsi che l&#39;impostazione **[!UICONTROL Elimina in Marketo]** sia **[!UICONTROL false]**, quindi fare clic su **[!UICONTROL Esegui ora]**.

   ![](assets/delete-person-from-sfdc-3.png)

   Dopo l’esecuzione del passaggio di flusso, la persona non sarà più un lead in Salesforce, ma rimarrà in Marketo.

   >[!CAUTION]
   >
   >Se imposti **[!UICONTROL Elimina in Marketo]** su **[!UICONTROL true]** ed elimini le persone da Marketo e i lead da Salesforce, non ci saranno più. Questa operazione non può essere annullata.
