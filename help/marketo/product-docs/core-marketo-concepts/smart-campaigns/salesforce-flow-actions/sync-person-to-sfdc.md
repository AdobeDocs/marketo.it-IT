---
unique-page-id: 1147027
description: Sincronizza persona con SFDC - Documentazione Marketo - Documentazione del prodotto
title: Sincronizza persona con SFDC
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 4bae0126d6b36720e170bea7b6b973508c855633
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 0%

---

# Sincronizza persona con SFDC {#sync-person-to-sfdc}

Questo passaggio di flusso inserirà le persone create da Marketo come lead nel CRM Salesforce.

![](assets/sync-person-to-sfdc.png)

>[!NOTE]
>
>Disponibile solo se integrato con Salesforce.

1. Per impostazione predefinita, questo passaggio di flusso assegna i lead owner (proprietari lead) in base alle regole di assegnazione automatica Salesforce.

   ![](assets/sync-person-to-sfdc.png)

   >[!TIP]
   >
   >Salesforce richiede che siano compilati i campi Società e Cognome della persona. In caso contrario, il record del lead verrà rifiutato.

1. Puoi impostare un utente Salesforce specifico o una coda di lead come proprietario del lead.

   ![](assets/sync-person-to-sfdc-2.png)

   Quando si utilizza questo passaggio di flusso, la persona viene sincronizzata immediatamente come lead Salesforce e non deve attendere la sincronizzazione regolare.

   >[!CAUTION]
   >
   >Salesforce non consente l&#39;assegnazione di &quot;Contatti&quot; alle code di lead. In questo caso, Marketo creerà un &quot;lead&quot; duplicato in Salesforce.
