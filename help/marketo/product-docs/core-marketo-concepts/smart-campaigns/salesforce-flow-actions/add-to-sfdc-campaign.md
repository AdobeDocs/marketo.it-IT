---
unique-page-id: 1147034
description: Aggiungi a SFDC Campaign - Documentazione Marketo - Documentazione del prodotto
title: Aggiungi a SFDC Campaign
exl-id: a5e14cc7-fd83-4a2c-aacb-e515669c9d21
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 0%

---

# Aggiungi a SFDC Campaign {#add-to-sfdc-campaign}

Questo passaggio di flusso può essere utilizzato nelle campagne Marketo Engage o come singolo passaggio di flusso per aggiungere persone come lead in una campagna Salesforce. Se il lead non esiste ancora in Salesforce, verrà automaticamente sincronizzato e aggiunto alla campagna con lo stato specificato.

>[!NOTE]
>
>Disponibile solo se integrato con [!DNL Salesforce].

![](assets/add-to-sfdc-campaign-1.png)

## Utilizzo {#usage}

1. Trova e seleziona la campagna [!DNL Salesforce] a cui desideri aggiungere i lead.

   ![](assets/add-to-sfdc-campaign-2.png)

   >[!TIP]
   >
   >Se non riesci a visualizzare una campagna Salesforce nell’elenco delle campagne:
   >
   >  1. Assicurarsi che la sincronizzazione della [campagna sia abilitata](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}.
   >  1. Conferma che il tuo [utente Marketo Sync](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} è un [utente Marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"} in Salesforce.

   >[!TIP]
   >
   >Puoi utilizzare la campagna Salesforce [I miei token](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"} per semplificare la clonazione del programma.

1. Selezionare lo stato del membro della campagna [!DNL Salesforce] che si desidera assegnare ai lead quando vengono aggiunti.

   ![](assets/add-to-sfdc-campaign-3.png)

   >[!CAUTION]
   >
   >Se una persona è già un membro lead della campagna Salesforce, verrà ignorata e il suo stato NON verrà aggiornato. Puoi invece utilizzare [modificare il loro stato in una campagna SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"}.
