---
unique-page-id: 1147027
description: Sincr. la persona in SFDC - Marketo Docs - Documentazione del prodotto
title: Sincronizza persona con SFDC
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 0%

---


# Sincronizza persona con SFDC {#sync-person-to-sfdc}

>[!NOTE]
>
>Disponibile solo se integrato con Salesforce.

## Panoramica {#overview}

Questo passaggio di flusso inserirà le persone create da Marketo come lead in Salesforce CRM.

![](assets/sync-person-to-sfdc.png)

## Utilizzo {#usage}

1. Per impostazione predefinita, questo passaggio di flusso verrà assegnato ai proprietari principali in base alle regole di assegnazione automatica di Salesforce.

   ![](assets/sync-person-to-sfdc.png)

   >[!TIP]
   >
   >Salesforce richiede che siano compilati i campi Società e Cognome della persona. In caso contrario, rifiuterà il record lead.

1. Puoi impostare un utente Salesforce specifico o una coda lead come proprietario principale.

   ![](assets/sync-person-to-sfdc-2.png)

   Quando si utilizza questo passaggio di flusso, la persona viene sincronizzata immediatamente come lead Salesforce e non deve attendere la sincronizzazione regolare.

   >[!CAUTION]
   >
   >Salesforce non consente di assegnare &quot;Contatti&quot; alle code principali. In questo caso, Marketo creerà un &quot;Lead&quot; duplicato in Salesforce.

