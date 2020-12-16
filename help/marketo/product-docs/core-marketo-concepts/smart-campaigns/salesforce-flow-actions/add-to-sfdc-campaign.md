---
unique-page-id: 1147034
description: Aggiungere alla campagna SFDC - Documenti Marketo - Documentazione del prodotto
title: Aggiungi a campagna SFDC
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# Aggiungi a campagna SFDC {#add-to-sfdc-campaign}

>[!NOTE]
>
>Disponibile solo se integrato con Salesforce.

## Panoramica {#overview}

Questo passaggio di flusso può essere utilizzato nelle campagne Marketo o come singolo passaggio di flusso per aggiungere persone come lead in una campagna Salesforce. Se il lead non esiste ancora in Salesforce, verrà sincronizzato e aggiunto automaticamente alla campagna con lo stato specificato.

![](assets/image2014-9-22-15-3a43-3a36.png)

## Utilizzo {#usage}

1. Trova e seleziona la campagna Salesforce alla quale vuoi aggiungere i lead.

   ![](assets/image2014-9-22-15-3a43-3a45.png)

   >[!TIP]
   >
   >Se non riesci a visualizzare una campagna Salesforce nell&#39;elenco Campaign:
   >
   >    
   >    
   >    1. Accertatevi che la sincronizzazione della [campagna sia abilitata](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
   >    1. Verifica che [Marketo Sync User](../../../../product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) sia un utente [](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) Marketing in Salesforce.


   >[!TIP]
   >
   >Puoi utilizzare la campagna Salesforce [My Tokens](../../../../product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) per semplificare la duplicazione dei programmi.

1. Seleziona lo stato del membro della campagna Salesforce a cui vuoi assegnare i lead quando vengono aggiunti.

   ![](assets/image2014-9-22-15-3a45-3a2.png)

   >[!CAUTION]
   >
   >Se una persona è già un membro principale della campagna Salesforce, verrà saltata e il suo stato NON verrà aggiornato. È invece possibile [modificarne lo stato in una campagna](change-status-in-sfdc-campaign.md) SFDC.

