---
unique-page-id: 37356429
description: Crea attività in Microsoft - Documentazione Marketo - Documentazione del prodotto
title: Crea attività in Microsoft
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Crea attività in Microsoft {#create-task-in-microsoft}

In qualità di addetto al marketing, hai informazioni che possono aiutare le vendite a concludere le offerte. È possibile creare attività per informarli di ciò che dovrebbero fare e di quando dovrebbero farlo.

Crea attività in Microsoft crea un’attività in Attività relative alla persona (lead o contatti) in Microsoft.

>[!NOTE]
>
>Questo passaggio del flusso **funziona solo con i trigger**, non filtri, nella campagna intelligente.

Per impostazione predefinita, il passaggio di flusso si presenta così:

![](assets/msd1.png)

>[!NOTE]
>
>Quando l&#39;utente di sincronizzazione Marketo sta creando attività, **Ingresso** è un campo obbligatorio per l’attività da creare in Microsoft. Se non viene inserito alcun valore, Marketo immetterà cinque giorni per impostazione predefinita.

Personalizza tutti i campi per creare l’attività nel modo desiderato.

![](assets/msd2.png)

>[!NOTE]
>
>Il campo &quot;Status&quot; specificato per l’attività nell’azione di flusso aggiorna il campo: &quot;Motivo dello stato&quot; in Microsoft.

>[!TIP]
>
>È possibile utilizzare `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` e `{{system.tokens}}` in **Oggetto** e **Descrizione**. Vedi [Token per i passaggi del flusso](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md) per ulteriori dettagli.
