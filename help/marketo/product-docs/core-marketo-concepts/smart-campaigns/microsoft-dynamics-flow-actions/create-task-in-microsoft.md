---
unique-page-id: 37356429
description: Crea attività in Microsoft - Documenti Marketo - Documentazione prodotto
title: Crea attività in Microsoft
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---


# Crea attività in Microsoft {#create-task-in-microsoft}

In qualità di esperto di marketing, hai informazioni che possono aiutare le vendite a concludere le trattative. È possibile creare attività che consentano loro di sapere cosa devono fare e quando devono farlo.

Crea attività in Microsoft crea un&#39;attività in Attività relative alla Persona (Lead o Contatto) in Microsoft.

>[!NOTE]
>
>Questo passaggio di flusso funziona **solo se utilizzato con trigger**, non con filtri, nella campagna smart.

Per impostazione predefinita, il passaggio di scorrimento avrà il seguente aspetto:

![](assets/msd1.png)

>[!NOTE]
>
>Quando l&#39;utente di sincronizzazione marketing sta creando attività, **Due in** è un campo obbligatorio per la creazione dell&#39;attività in Microsoft. Se non viene immesso alcun valore, per impostazione predefinita verrà immesso cinque giorni.

Personalizzate tutti i campi per creare l’attività nel modo desiderato.

![](assets/msd2.png)

>[!NOTE]
>
>Il campo &quot;Stato&quot; specificato per l’attività nell’azione Flusso aggiorna il campo: &quot;Motivo stato&quot; in Microsoft.

>[!TIP]
>
>È possibile utilizzare `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` e `{{system.tokens}}` in **Subject** e **Description**. Per ulteriori informazioni, vedere [Token per i passaggi di flusso](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).
