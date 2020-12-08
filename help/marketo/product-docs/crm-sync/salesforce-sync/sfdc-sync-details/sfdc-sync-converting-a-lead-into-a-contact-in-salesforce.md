---
unique-page-id: 2953465
description: Sincr. SFDC - Conversione di un lead in un contatto in Salesforce - Documenti Marketo - Documentazione del prodotto
title: Sincr. SFDC - Conversione di un lead in un contatto in Salesforce
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---


# Sincr. SFDC: Conversione di un lead in un contatto in Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

>[!NOTE]
>
>**FYI**
>
>Marketo sta standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che nell&#39;abbonamento siano presenti lead/lead e persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

Immagina tre diversi scenari in Salesforce: (non utilizzando il passaggio [di flusso](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) Converti persona in Marketo)

1. Conversione di un lead in un **nuovo contatto e nuovo account**
1. Conversione di un lead in un **nuovo contatto** in un account **esistente**

1. Conversione di un lead in un contatto **** esistente in un account **** esistente (operazione identica all&#39; [unione](sfdc-sync-merging-a-lead-contact-person.md))

In tutti e tre i casi si finisce con **1 contatto e nessun lead in Salesforce e 1 contatto e nessuna persona a Marketo.**

A Marketo, il record avrà un tipo SFDC = Contact.

>[!TIP]
>
>Durante la conversione in Salesforce, accertati che i campi personalizzati [lead siano mappati correttamente](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm). Non vuoi perdere dati.

È possibile attivare e filtrare utilizzando: &quot;Il lead è convertito&quot; e &quot;Il lead è stato convertito.&quot;