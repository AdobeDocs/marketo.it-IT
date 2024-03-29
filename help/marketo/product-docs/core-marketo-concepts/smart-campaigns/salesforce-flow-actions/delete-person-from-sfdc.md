---
unique-page-id: 1147031
description: Elimina persona da SFDC - Documentazione di Marketo - Documentazione del prodotto
title: Elimina persona da SFDC
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 4bae0126d6b36720e170bea7b6b973508c855633
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---

# Elimina persona da SFDC {#delete-person-from-sfdc}

Se devi rimuovere un set specifico di lead da Salesforce ma lasciarli come persone nel Marketo Engage, puoi utilizzare l’azione di flusso Elimina persona da SFDC.

>[!NOTE]
>
>Disponibile solo se integrato con Salesforce.

1. Nel database, fare clic sulla persona che si desidera rimuovere da Salesforce. Quindi fai clic su **[!UICONTROL Azioni della persona]** e seleziona **[!DNL Salesforce]**.

   ![](assets/person-actions-salesforce.png)

1. Seleziona **[!UICONTROL Elimina persona da SFDC]**.

   ![](assets/delete-person-from-sfdc.png)

1. Assicurarsi che **[!UICONTROL Elimina in Marketo]** impostazione è **[!UICONTROL false]**, quindi fai clic su **[!UICONTROL Esegui ora]**.

   ![](assets/run-action-delete-lead-from-sfdc.png)

   Dopo l’esecuzione del passaggio di flusso, la persona non sarà più un lead in Salesforce, ma rimarrà in Marketo.

   >[!CAUTION]
   >
   >Se si imposta **[!UICONTROL Elimina in Marketo]** a **[!UICONTROL true]** e cancellare le persone da Marketo e i lead da Salesforce, sono andati per sempre. Questa operazione non può essere annullata.
