---
unique-page-id: 2953465
description: Sincr. SFDC - Conversione di un lead in un contatto in Salesforce - Marketo Docs - Documentazione del prodotto
title: Sincr. SFDC - Conversione di un lead in un contatto in Salesforce
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Sincr. SFDC: Conversione di un lead in un contatto in Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Immaginate tre diversi scenari in Salesforce: (non utilizzando il [passaggio di flusso Converti persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) in Marketo)

1. Conversione di un lead in un **nuovo contatto e nuovo account**
1. Conversione di un lead in un **nuovo contatto** in un **account esistente**

1. Conversione di un lead in un **contatto esistente** in un **account esistente** (funziona esattamente come [unione](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md))

In tutti e tre i casi si finisce con **1 contatto e nessun lead in Salesforce e 1 contatto e nessuna persona in Marketo.**

In Marketo, il record avrà ora un tipo SFDC = Contatto.

>[!TIP]
>
>Durante la conversione in Salesforce, assicurati che i campi [personalizzati lead siano mappati correttamente](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm). Non volete perdere dati.

Puoi attivare e filtrare utilizzando: &quot;Il piombo è convertito&quot; e &quot;Il piombo è stato convertito&quot;.
