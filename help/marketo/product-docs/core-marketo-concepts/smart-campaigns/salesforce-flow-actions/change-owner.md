---
unique-page-id: 1147021
description: Modifica proprietario - Documentazione di Marketo - Documentazione del prodotto
title: Cambia proprietario
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---

# Cambia proprietario {#change-owner}

Se esistono persone già assegnate a un proprietario, è possibile utilizzare questo passaggio di flusso per riassegnarle a un altro proprietario.

![](assets/change-owner-1.png)

1. È sufficiente scegliere il proprietario o la coda di lead da modificare e andare.

   ![](assets/change-owner-2.png)

   >[!CAUTION]
   >
   >Salesforce non consente l&#39;assegnazione dei contatti alle code dei lead. Per un record che è un contatto SFDC:
   >
   >* Marketo creerà un lead duplicato **only** quando il contatto verrà sincronizzato con Salesforce. In altre parole, se si utilizza il passaggio di flusso **[Sincronizza persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** con `AssignTo=<a lead queue>`, Marketo creerà un lead duplicato in Salesforce e lo assegnerà alla coda lead.
   >
   >* Se si utilizza il passaggio di flusso **[!UICONTROL Modifica proprietario]** su un contatto, Marketo crea un lead duplicato in Salesforce. Per evitare questo problema, utilizza un filtro nel campo &quot;Tipo SFDC&quot; che limita l’azione ai soli lead.

   >[!NOTE]
   >
   >Se il record non esiste ancora nell’account Salesforce, lo sincronizzeremo e lo assegneremo all’utente selezionato.
