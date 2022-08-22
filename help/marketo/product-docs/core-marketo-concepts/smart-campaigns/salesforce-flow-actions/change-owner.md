---
unique-page-id: 1147021
description: Cambia proprietario - Documenti Marketo - Documentazione del prodotto
title: Cambia proprietario
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
source-git-commit: 44c134811242b4136a3137cdd60e60edeb838c8c
workflow-type: tm+mt
source-wordcount: '170'
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
   >1. Marketo creerà un lead duplicato **only** quando il contatto viene sincronizzato con Salesforce. In altre parole, se utilizzi il **[Sincronizza persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** passo di flusso con `AssignTo=<a lead queue>`, Marketo creerà un lead duplicato in Salesforce e lo assegnerà alla coda del lead.
   >
   >1. Se utilizzi **Cambia proprietario** passaggio di flusso su un contatto, Marketo crea un lead duplicato in Salesforce. Per evitare questo problema, utilizza un filtro sul campo &quot;Tipo SFDC&quot; che limita l’azione ai soli lead.


   >[!NOTE]
   >
   >Se il record non esiste ancora nel tuo account Salesforce, lo sincronizzeremo e lo assegneremo all&#39;utente selezionato.
