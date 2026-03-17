---
unique-page-id: 1147017
description: Scopri come creare un’attività Salesforce in un passaggio di flusso. Crea un'attività per il proprietario del lead quando qualcuno entra nel flusso.
title: Creare attività
exl-id: c484d913-1fd8-4716-8caa-0bf318218ca1
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 3efcb529cd3e35027f35e51dfd91f95e94af9d61
workflow-type: tm+mt
source-wordcount: '126'
ht-degree: 3%

---

# Creare attività {#create-task}

In qualità di addetto al marketing, hai a disposizione informazioni che possono essere di aiuto alle vendite per concludere un affare. Puoi creare attività per comunicare loro cosa dovrebbero fare e quando dovrebbero farlo.

![](assets/create-task-1.png)

>[!NOTE]
>
>Quando l&#39;utente di Marketo Sync crea attività, **[!UICONTROL Due In]** è un campo obbligatorio per la creazione dell&#39;attività in Salesforce. Marketo inserirà cinque giorni per impostazione predefinita se non è presente alcun valore.

Per impostazione predefinita, il passaggio del flusso si presenta così:

![](assets/create-task-2.png)

Personalizzare tutti i campi per creare l&#39;attività nel modo desiderato.

![](assets/create-task-3.png)

>[!TIP]
>
>È possibile utilizzare `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` e `{{system.tokens}}` in **[!UICONTROL Subject]** e **[!UICONTROL Description]**. Per ulteriori dettagli, consulta [Token per i passaggi del flusso](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"}.
