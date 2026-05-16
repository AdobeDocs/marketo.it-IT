---
unique-page-id: 1147031
description: Scopri come eliminare una persona da Salesforce con un passaggio di flusso. Rimuovere il lead o il contatto da SFDC quando entrano nel flusso.
title: Eliminare persona da SFDC
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
TQID: https://experienceleague.adobe.com/f-Zvc4glfCtAagE314vrZjiWIcD3vaGIKmKGeZO18v0
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 133
ht-degree: 6%

---

# Eliminare persona da SFDC {#delete-person-from-sfdc}

Se è necessario rimuovere un set specifico di lead da Salesforce, ma lasciarli come persone in Marketo Engage, è possibile utilizzare l&#39;azione di flusso Elimina persona da SFDC.

>[!NOTE]
>
>Disponibile solo se integrato con [!DNL Salesforce].

1. Nel database fare clic sulla persona che si desidera rimuovere da Salesforce. Quindi fare clic su **[!UICONTROL Person Actions]** e selezionare **[!DNL Salesforce]**.

   ![](assets/delete-person-from-sfdc-1.png)

1. Seleziona **[!UICONTROL Delete Person from SFDC]**.

   ![](assets/delete-person-from-sfdc-2.png)

1. Assicurarsi che l&#39;impostazione **[!UICONTROL Delete in Marketo]** sia **[!UICONTROL false]**, quindi fare clic su **[!UICONTROL Run Now]**.

   ![](assets/delete-person-from-sfdc-3.png)

   Dopo l&#39;esecuzione del passaggio di flusso, la persona non sarà più un lead in [!DNL Salesforce] ma rimarrà in Marketo.

   >[!CAUTION]
   >
   >Se imposti **[!UICONTROL Delete in Marketo]** su **[!UICONTROL true]** ed elimini le persone da Marketo e i lead da Salesforce, non ci saranno più. Questa operazione non può essere annullata.
