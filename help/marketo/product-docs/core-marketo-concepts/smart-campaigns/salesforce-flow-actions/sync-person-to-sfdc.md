---
unique-page-id: 1147027
description: Sincronizza persona con SFDC - Documenti Marketo - Documentazione del prodotto
title: Sincronizza persona con SFDC
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 1%

---

# Sincronizza persona con SFDC {#sync-person-to-sfdc}

>[!NOTE]
>
>Disponibile solo se integrato con Salesforce.

## Panoramica {#overview}

Questo passaggio del flusso inserirà le persone create da Marketo come lead nel tuo CRM Salesforce.

![](assets/sync-person-to-sfdc.png)

## Utilizzo {#usage}

1. Per impostazione predefinita, questo passaggio di flusso viene assegnato ai proprietari dei lead in base alle regole di assegnazione automatica Salesforce.

   ![](assets/sync-person-to-sfdc.png)

   >[!TIP]
   >
   >Salesforce richiede la compilazione dei campi Azienda e Cognome della persona. In caso contrario, rifiuterà il record lead.

1. Puoi impostare come proprietario del lead un utente Salesforce specifico o una coda lead.

   ![](assets/sync-person-to-sfdc-2.png)

   Quando utilizzi questo passaggio di flusso, la persona viene sincronizzata immediatamente come lead Salesforce e non deve attendere la sincronizzazione regolare.

   >[!CAUTION]
   >
   >Salesforce non consente di assegnare &quot;Contatti&quot; alle code di lead. In questo caso, Marketo creerà un &quot;Lead&quot; duplicato in Salesforce.
