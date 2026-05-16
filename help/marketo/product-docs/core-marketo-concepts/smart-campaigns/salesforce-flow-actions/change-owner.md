---
unique-page-id: 1147021
description: Scopri come cambiare il proprietario di Salesforce in un passaggio di flusso. Assegna un nuovo lead o proprietario del contatto quando le persone entrano nel flusso.
title: Modificare proprietario
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
feature: Smart Campaigns, Salesforce Integration
TQID: https://experienceleague.adobe.com/VU0fT4giNqfkF5g15q0IGIh8XuO2505nz89UuUfqZro
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 182
ht-degree: 2%

---

# Modificare proprietario {#change-owner}

Se esistono persone già assegnate a un proprietario, è possibile utilizzare questo passaggio di flusso per riassegnarle a un altro proprietario.

![](assets/change-owner-1.png)

1. È sufficiente scegliere il proprietario o la coda di lead da modificare e andare.

   ![](assets/change-owner-2.png)

   >[!CAUTION]
   >
   >[!DNL Salesforce] non consente l&#39;assegnazione di contatti alle code lead. Per un record corrispondente a un contatto SFDC:
   >
   >* Marketo creerà un lead duplicato **only** quando il contatto verrà sincronizzato con Salesforce. In altre parole, se si utilizza il passaggio di flusso **[Sincronizza persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** con `AssignTo=<a lead queue>`, Marketo creerà un lead duplicato in Salesforce e lo assegnerà alla coda dei lead.
   >
   >* Se si utilizza il passaggio di flusso **[!UICONTROL Change Owner]** su un contatto, Marketo crea un lead duplicato in Salesforce. Per evitare questo problema, utilizza un filtro nel campo &quot;Tipo SFDC&quot; che limita l’azione ai soli lead.

   >[!NOTE]
   >
   >Se il record non esiste ancora nell&#39;account [!DNL Salesforce], verrà sincronizzato e assegnato all&#39;utente selezionato.
