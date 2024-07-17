---
unique-page-id: 1147017
description: Crea attività - Documenti Marketo - Documentazione del prodotto
title: Crea attività
exl-id: c484d913-1fd8-4716-8caa-0bf318218ca1
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '113'
ht-degree: 0%

---

# Crea attività {#create-task}

In qualità di addetto al marketing, hai a disposizione informazioni che possono essere di aiuto alle vendite per concludere un affare. Puoi creare attività per comunicare loro cosa dovrebbero fare e quando dovrebbero farlo.

![](assets/create-task-1.png)

>[!NOTE]
>
>Quando l&#39;utente di Marketo Sync crea delle attività, **[!UICONTROL Scadenza]** è un campo obbligatorio per la creazione dell&#39;attività in Salesforce. Marketo inserirà cinque giorni per impostazione predefinita se non è presente alcun valore.

Per impostazione predefinita, il passaggio del flusso si presenta così:

![](assets/create-task-2.png)

Personalizzare tutti i campi per creare l&#39;attività nel modo desiderato.

![](assets/create-task-3.png)

>[!TIP]
>
>È possibile utilizzare `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` e `{{system.tokens}}` in **[!UICONTROL Subject]** e **[!UICONTROL Description]**. Per ulteriori dettagli, consulta [Token per i passaggi del flusso](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"}.
