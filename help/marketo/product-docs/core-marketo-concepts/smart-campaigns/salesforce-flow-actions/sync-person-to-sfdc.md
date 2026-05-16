---
unique-page-id: 1147027
description: Scopri come sincronizzare una persona con Salesforce con un passaggio di flusso. Invia i dati del lead o del contatto a SFDC quando questo entra nel flusso.
title: Sincronizzare persona con SFDC
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
feature: Smart Campaigns, Salesforce Integration
TQID: https://experienceleague.adobe.com/jU7Hg1x8TUfxR4GnO1oxvJXh-8X3LVXll9z8k5Eck80
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 143
ht-degree: 5%

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
