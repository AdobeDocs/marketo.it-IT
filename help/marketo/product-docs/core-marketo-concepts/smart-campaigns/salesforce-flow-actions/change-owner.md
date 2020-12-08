---
unique-page-id: 1147021
description: Cambia proprietario - Documenti Marketo - Documentazione prodotto
title: Cambia proprietario
translation-type: tm+mt
source-git-commit: f27e2bac90570f9f795dc6bdd5fcf208c446be14
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---


# Cambia proprietario {#change-owner}

Se a un proprietario sono già assegnate persone esistenti, puoi utilizzare questo passaggio di flusso per riassegnarle a un altro proprietario.

![](assets/image2014-9-22-15-3a1-3a3.png)

**Utilizzo**

1. È sufficiente selezionare il proprietario o la coda di lead a cui si desidera passare e andare!

   ![](assets/image2014-9-22-15-3a1-3a6.png)

   >[!CAUTION]
   >
   >Salesforce non consente l&#39;assegnazione dei contatti alle code principali. Per un record che si tratta di un contatto SFDC:
   >
   >1. Marketo creerà un lead duplicato **solo** quando il contatto viene sincronizzato con Salesforce. In altre parole, se utilizzate il passaggio di flusso **[Sincronizza persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** con `AssignTo=<a lead queue>`, Marketo creerà un lead duplicato in Salesforce e lo assegnerà alla coda di lead.
      >
      >
   2. Se tenti di utilizzare il passaggio di flusso **Modifica proprietario** su un contatto, non verrà creato alcun duplicato in Salesforce.


   >[!NOTE]
   >
   >Se il record non esiste ancora nel tuo account Salesforce, lo sincronizzeremo e lo assegneremo all&#39;utente selezionato.
