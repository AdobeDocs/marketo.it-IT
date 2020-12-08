---
unique-page-id: 37356429
description: Crea attività in Microsoft - Documenti Marketo - Documentazione prodotto
title: Crea attività in Microsoft
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# Crea attività in Microsoft {#create-task-in-microsoft}

In qualità di esperto di marketing, hai informazioni che possono aiutare le vendite a concludere le trattative. È possibile creare attività che consentano loro di sapere cosa devono fare e quando devono farlo.

Crea attività in Microsoft crea un&#39;attività in Attività relative alla Persona (Lead o Contatto) in Microsoft.

>[!NOTE]
>
>Questo passaggio di flusso funziona **solo se utilizzato con attivatori**, non con filtri, nella campagna smart.

Per impostazione predefinita, il passaggio di scorrimento avrà il seguente aspetto:   ![](assets/msd1.png)

>[!NOTE]
>
>Quando l&#39;utente di sincronizzazione Marketo sta creando attività, **Due in **è un campo obbligatorio per l&#39;attività da creare in Microsoft. Se non viene immesso alcun valore, per impostazione predefinita verrà immesso cinque giorni.

Personalizzate tutti i campi per creare l’attività nel modo desiderato.   ![](assets/msd2.png)

>[!NOTE]
>
>Il campo &quot;Stato&quot; specificato per l’attività nell’azione Flusso aggiorna il campo: &quot;Motivo stato&quot; in Microsoft.

>[!TIP]
>
>È possibile utilizzare `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` e `{{system.tokens}}` in **Oggetto** e **Descrizione**. Per ulteriori informazioni, consulta [Token per i passaggi](http://docs.marketo.com/x/c4AR) di flusso.

