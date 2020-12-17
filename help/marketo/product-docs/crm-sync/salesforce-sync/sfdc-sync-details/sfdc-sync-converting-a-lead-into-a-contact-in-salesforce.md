---
unique-page-id: 2953465
description: Sincr. SFDC - Conversione di un lead in un contatto in Salesforce - Documenti Marketo - Documentazione del prodotto
title: Sincr. SFDC - Conversione di un lead in un contatto in Salesforce
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# Sincr. SFDC: Conversione di un lead in un contatto in Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Immagina tre diversi scenari in Salesforce: (non utilizzando il passaggio [Converti persona flusso](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) in Marketo)

1. Conversione di un lead in un **nuovo contatto e nuovo account**
1. Conversione di un lead in un **nuovo contatto** in un **account esistente**

1. Conversione di un lead in un **contatto esistente** in un **account esistente** (funziona identica a [unione](sfdc-sync-merging-a-lead-contact-person.md))

In tutti e tre i casi si finisce con un **1 contatto e nessun lead in Salesforce e 1 contatto e nessuna persona in Marketo.**

A Marketo, il record avrà un tipo SFDC = Contact.

>[!TIP]
>
>Durante la conversione in Salesforce, verifica che i campi [lead personalizzati siano mappati correttamente](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm). Non vuoi perdere dati.

È possibile attivare e filtrare utilizzando: &quot;Il lead è convertito&quot; e &quot;Il lead è stato convertito.&quot;