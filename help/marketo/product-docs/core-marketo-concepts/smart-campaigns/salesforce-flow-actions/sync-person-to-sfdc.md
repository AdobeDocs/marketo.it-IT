---
unique-page-id: 1147027
description: Sincronizza persona con SFDC - Documentazione Marketo - Documentazione del prodotto
title: Sincronizzare persona con SFDC
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 6%

---

# Sincronizzare persona con SFDC {#sync-person-to-sfdc}

Questo passaggio di flusso inserirà le persone create da Marketo come lead nel tuo Salesforce CRM.

>[!NOTE]
>
>Disponibile solo se integrato con [!DNL Salesforce].

1. Per impostazione predefinita, questo passaggio di flusso assegna ai proprietari dei lead in base alle regole di assegnazione automatica di Salesforce.

   ![](assets/sync-person-to-sfdc-1.png)

   >[!TIP]
   >
   >[!DNL Salesforce] richiede che la persona abbia compilati i campi Società e Cognome. In caso contrario, il record del lead verrà rifiutato.

1. È possibile impostare come proprietario del lead un utente o una coda lead [!DNL Salesforce] specifica.

   ![](assets/sync-person-to-sfdc-2.png)

   Quando si utilizza questo passaggio di flusso, la persona viene sincronizzata immediatamente come lead [!DNL Salesforce] e non deve attendere la sincronizzazione regolare.

   >[!CAUTION]
   >
   >[!DNL Salesforce] non consente l&#39;assegnazione di &quot;Contatti&quot; alle code di lead. In questo caso, Marketo creerà un &quot;lead&quot; duplicato in [!DNL Salesforce].
