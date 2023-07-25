---
unique-page-id: 1147021
description: Modifica proprietario - Documentazione di Marketo - Documentazione del prodotto
title: Cambia proprietario
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
feature: Smart Campaigns, Salesforce Integration
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# Cambia proprietario {#change-owner}

Se esistono persone già assegnate a un proprietario, è possibile utilizzare questo passaggio di flusso per riassegnarle a un altro proprietario.

![](assets/image2014-9-22-15-3a1-3a3.png)

**Utilizzo**

1. È sufficiente scegliere il proprietario o la coda di lead da modificare e andare.

   ![](assets/image2014-9-22-15-3a1-3a6.png)

   >[!CAUTION]
   >
   >Salesforce non consente l&#39;assegnazione dei contatti alle code dei lead. Per un record che è un contatto SFDC:
   >
   >1. Marketo creerà un lead duplicato **solo** quando il contatto viene sincronizzato con Salesforce. In altre parole, se utilizzi il **[Sincronizza persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** passaggio di flusso con `AssignTo=<a lead queue>`, Marketo creerà un lead duplicato in Salesforce e lo assegnerà alla coda lead.
   >
   >1. Se si utilizza **Cambia proprietario** passaggio di flusso su un contatto, Marketo crea un lead duplicato in Salesforce. Per evitare questo problema, utilizza un filtro nel campo &quot;Tipo SFDC&quot; che limita l’azione ai soli lead.

   >[!NOTE]
   >
   >Se il record non esiste ancora nell’account Salesforce, lo sincronizzeremo e lo assegneremo all’utente selezionato.
