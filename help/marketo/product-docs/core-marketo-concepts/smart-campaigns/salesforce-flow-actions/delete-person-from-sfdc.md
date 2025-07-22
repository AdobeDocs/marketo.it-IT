---
unique-page-id: 1147031
description: Elimina persona da SFDC - Documentazione Marketo - Documentazione del prodotto
title: Elimina persona da SFDC
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 0%

---

# Elimina persona da SFDC {#delete-person-from-sfdc}

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
