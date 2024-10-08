---
unique-page-id: 2953465
description: Sincronizzazione SFDC - Conversione di un lead in un contatto in Salesforce - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Conversione di un lead in un contatto in Salesforce
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 0%

---

# Sincronizzazione SFDC: convertire un lead in un contatto in Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Immagina tre scenari diversi in Salesforce: (non utilizzando il passaggio [Converti flusso persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"} nel Marketo Engage)

1. Conversione di un lead in **nuovo contatto e nuovo account**
1. Conversione di un lead in un **nuovo contatto** in un **account esistente**

1. Conversione di un lead in un **contatto esistente** in un **account esistente** (funziona in modo identico a [unione](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md){target="_blank"})

In tutti e tre i casi si ottiene **1 contatto e nessun lead in Salesforce e 1 contatto e nessuna persona in Marketo.**

In Marketo, il record avrà ora un SFDC Type = Contact (Tipo SFDC = Contatto).

>[!TIP]
>
>Durante la conversione in Salesforce, assicurati che i campi personalizzati [lead siano mappati correttamente](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm){target="_blank"}. Non vuoi perdere dati.

Puoi attivare e filtrare utilizzando: &quot;Il lead è convertito&quot; e &quot;Il lead è stato convertito&quot;.
