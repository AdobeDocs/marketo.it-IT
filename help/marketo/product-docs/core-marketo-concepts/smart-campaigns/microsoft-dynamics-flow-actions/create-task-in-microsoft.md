---
unique-page-id: 37356429
description: Crea attività in Microsoft - Documentazione Marketo - Documentazione del prodotto
title: Creare attività in Microsoft
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '164'
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
