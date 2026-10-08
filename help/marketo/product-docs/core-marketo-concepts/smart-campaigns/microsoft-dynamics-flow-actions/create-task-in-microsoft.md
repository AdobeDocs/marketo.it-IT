---
unique-page-id: 37356429
description: Scopri come creare un’attività in Microsoft Dynamics da un passaggio del flusso. Crea un'attività per il proprietario quando qualcuno entra nel flusso.
title: Creare attività in Microsoft
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
TQID: 'https://experienceleague.adobe.com/qQL3O4Vi8ncdlXtk2gvraWzquz3oZx5B-1YWTkwdVac'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: d5c7388a-594e-4d15-9b39-98d6ce479e8b
    internal-label: Microsoft Dynamics
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 4%
---
# Creare attività in Microsoft {#create-task-in-microsoft}

In qualità di addetto al marketing, hai a disposizione informazioni che possono essere di aiuto alle vendite per concludere un affare. Puoi creare attività per comunicare loro cosa dovrebbero fare e quando dovrebbero farlo.

Crea attività in Microsoft crea un&#39;attività in Attività relative alla persona (lead o contatto) in [!DNL Microsoft].

>[!NOTE]
>
>Questo passaggio di flusso _funziona solo se utilizzato con trigger_, non con filtri, nella tua campagna avanzata.

Per impostazione predefinita, il passaggio del flusso si presenta così:

![](assets/create-task-in-microsoft-1.png)

>[!NOTE]
>
>Quando l&#39;utente di Marketo Sync crea attività, **[!UICONTROL Due In]** è un campo obbligatorio per la creazione dell&#39;attività in [!DNL Microsoft]. Marketo inserirà cinque giorni per impostazione predefinita se non viene immesso alcun valore.

Personalizzare tutti i campi per creare l&#39;attività nel modo desiderato.

![](assets/create-task-in-microsoft-2.png)

>[!NOTE]
>
>Il campo &quot;Stato&quot; specificato per l&#39;attività nell&#39;azione di flusso aggiorna il campo: &quot;Motivo stato&quot; in [!DNL Microsoft].

>[!TIP]
>
>È possibile utilizzare `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` e `{{system.tokens}}` in **[!UICONTROL Subject]** e **[!UICONTROL Description]**. Per ulteriori dettagli, consulta [Token per i passaggi del flusso](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"}.
