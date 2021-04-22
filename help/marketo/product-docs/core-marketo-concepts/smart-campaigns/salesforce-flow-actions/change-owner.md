---
unique-page-id: 1147021
description: Cambia proprietario - Documenti Marketo - Documentazione del prodotto
title: Cambia proprietario
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---

# Cambia proprietario {#change-owner}

Se si dispone di persone esistenti già assegnate a un proprietario, è possibile utilizzare questo passaggio di flusso per riassegnarle a un altro proprietario.

![](assets/image2014-9-22-15-3a1-3a3.png)

**Utilizzo**

1. Scegli semplicemente il proprietario o la coda di lead a cui vuoi cambiare e vai!

   ![](assets/image2014-9-22-15-3a1-3a6.png)

   >[!CAUTION]
   >
   >Salesforce non consente l&#39;assegnazione di contatti alle code di lead. Per un record che è un contatto SFDC:
   >
   >1. Marketo creerà un lead duplicato **solo** quando il contatto viene sincronizzato in Salesforce. In altre parole, se utilizzi il passaggio di flusso **[Sincronizza persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** con `AssignTo=<a lead queue>`, Marketo creerà un lead duplicato in Salesforce e lo assegnerà alla coda del lead.
      >
      >
   1. Se tenti di utilizzare il passaggio di flusso **Cambia proprietario** su un contatto, non verrà creato alcun duplicato in Salesforce.


   >[!NOTE]
   >
   >Se il record non esiste ancora nel tuo account Salesforce, lo sincronizzeremo e lo assegneremo all&#39;utente selezionato.
