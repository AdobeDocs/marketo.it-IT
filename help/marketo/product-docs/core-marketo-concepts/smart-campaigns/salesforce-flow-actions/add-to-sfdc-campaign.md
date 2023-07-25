---
unique-page-id: 1147034
description: Aggiunta a una campagna SFDC - Documentazione di Marketo - Documentazione del prodotto
title: Aggiungi a campagna SFDC
exl-id: a5e14cc7-fd83-4a2c-aacb-e515669c9d21
feature: Smart Campaigns, Salesforce Integration
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 1%

---

# Aggiungi a campagna SFDC {#add-to-sfdc-campaign}

>[!NOTE]
>
>Disponibile solo se integrato con Salesforce.

## Panoramica {#overview}

Questo passaggio di flusso può essere utilizzato nelle campagne Marketo o come un singolo passaggio di flusso per aggiungere persone come lead in una campagna Salesforce. Se il lead non esiste ancora in Salesforce, verrà automaticamente sincronizzato e aggiunto alla campagna con lo stato specificato.

![](assets/image2014-9-22-15-3a43-3a36.png)

## Utilizzo {#usage}

1. Trova e seleziona la campagna Salesforce a cui desideri aggiungere i lead.

   ![](assets/image2014-9-22-15-3a43-3a45.png)

   >[!TIP]
   >
   >Se non riesci a visualizzare una campagna Salesforce nell’elenco Campaign:
   >
   >  1. Assicurati che le [la sincronizzazione della campagna è abilitata](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
   >  1. Conferma che il tuo [Utente Marketo Sync](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) è un [Utente marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) in Salesforce.

   >[!TIP]
   >
   >Puoi utilizzare la campagna Salesforce [I miei token](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) per semplificare la clonazione dei programmi.

1. Selezionare lo stato del membro della campagna Salesforce che si desidera assegnare ai lead quando vengono aggiunti.

   ![](assets/image2014-9-22-15-3a45-3a2.png)

   >[!CAUTION]
   >
   >Se una persona è già un membro principale della campagna Salesforce, verrà ignorata e il suo stato NON verrà aggiornato. È possibile utilizzare [cambiare il loro stato in una campagna SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md) invece.
