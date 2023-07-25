---
unique-page-id: 2953465
description: Sincronizzazione SFDC - Conversione di un lead in un contatto in Salesforce - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Conversione di un lead in un contatto in Salesforce
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Sincronizzazione SFDC: convertire un lead in un contatto in Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Immagina tre scenari diversi in Salesforce: (senza utilizzare il [Passaggio di flusso Converti persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) in Marketo)

1. Conversione di un lead in un **nuovo contatto e nuovo account**
1. Conversione di un lead in un **nuovo contatto** in un **account esistente**

1. Conversione di un lead in un **contatto esistente** in un **account esistente** (funziona come se [unione](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md))

In tutti e tre i casi si finisce con **1 contatto e nessun lead in Salesforce e 1 contatto e nessuna persona in Marketo.**

In Marketo, il record avrà ora un SFDC Type = Contact (Tipo SFDC = Contatto).

>[!TIP]
>
>Durante la conversione in Salesforce, assicurati che il [i campi personalizzati del lead sono mappati correttamente](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm). Non vuoi perdere dati.

Puoi attivare e filtrare utilizzando: &quot;Il lead è convertito&quot; e &quot;Il lead è stato convertito&quot;.
