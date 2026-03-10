---
unique-page-id: 2953465
description: Scopri cosa accade quando si converte un lead in un contatto in Salesforce. Scopri in che modo Marketo riflette la modifica e come utilizzare Lead in Trigger e filtri convertiti.
title: Sincronizzazione SFDC - Conversione di un lead in un contatto in Salesforce
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
feature: Salesforce Integration
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Sincronizzazione SFDC: conversione di un lead in un contatto in [!DNL Salesforce] {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Immagina tre scenari diversi in [!DNL Salesforce]: (non si utilizza il [passaggio del flusso Converti persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) in Marketo)

1. Conversione di un lead in **nuovo contatto e nuovo account**
1. Conversione di un lead in un **nuovo contatto** in un **account esistente**

1. Conversione di un lead in un **contatto esistente** in un **account esistente** (funziona in modo identico a [unione](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md){target="_blank"})

In tutti e tre i casi si ottiene **1 contatto e nessun lead in [!DNL Salesforce] e 1 contatto e nessuna persona in Marketo.**

In Marketo, il record avrà ora un SFDC Type = Contact.

>[!TIP]
>
>Durante la conversione in [!DNL Salesforce], assicurati che i campi personalizzati di [lead siano mappati correttamente](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm). Non vuoi perdere dati.

È possibile attivare e filtrare utilizzando: &quot;[!UICONTROL Lead is Converted]&quot; e &quot;[!UICONTROL Lead was Converted]&quot;.&quot;
