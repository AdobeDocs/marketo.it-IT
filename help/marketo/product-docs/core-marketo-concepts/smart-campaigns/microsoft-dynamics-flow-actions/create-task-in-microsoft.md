---
unique-page-id: 37356429
description: Crea attività in Microsoft - Documentazione Marketo - Documentazione del prodotto
title: Crea attività in Microsoft
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Crea attività in Microsoft {#create-task-in-microsoft}

In qualità di addetto al marketing, hai a disposizione informazioni che possono essere di aiuto alle vendite per concludere un affare. Puoi creare attività per comunicare loro cosa dovrebbero fare e quando dovrebbero farlo.

Crea attività in Microsoft crea un’attività in Attività relative alla persona (lead o contatto) in Microsoft.

>[!NOTE]
>
>Questo passaggio di flusso **funziona solo con i trigger**, non i filtri, nella tua campagna avanzata.

Per impostazione predefinita, il passaggio del flusso si presenta così:

![](assets/msd1.png)

>[!NOTE]
>
>Quando l&#39;utente di Marketo Sync sta creando attività, **Scade tra** è un campo obbligatorio per la creazione dell’attività in Microsoft. Marketo inserirà cinque giorni per impostazione predefinita se non viene immesso alcun valore.

Personalizzare tutti i campi per creare l&#39;attività nel modo desiderato.

![](assets/msd2.png)

>[!NOTE]
>
>Il campo &quot;Stato&quot; specificato per l’attività nell’azione di flusso aggiorna il campo: &quot;Motivo stato&quot; in Microsoft.

>[!TIP]
>
>È possibile utilizzare `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` e `{{system.tokens}}` nel **Oggetto** e **Descrizione**. Consulta [Token per i passaggi del flusso](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md) per ulteriori dettagli.
