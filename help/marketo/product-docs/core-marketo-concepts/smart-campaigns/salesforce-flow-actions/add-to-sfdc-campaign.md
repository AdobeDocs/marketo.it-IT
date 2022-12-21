---
unique-page-id: 1147034
description: Aggiungi alla campagna SFDC - Documenti Marketo - Documentazione del prodotto
title: Aggiungi alla campagna SFDC
exl-id: a5e14cc7-fd83-4a2c-aacb-e515669c9d21
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 1%

---

# Aggiungi alla campagna SFDC {#add-to-sfdc-campaign}

>[!NOTE]
>
>Disponibile solo se integrato con Salesforce.

## Panoramica {#overview}

Questo passaggio di flusso può essere utilizzato nelle campagne Marketo o come singolo passaggio di flusso per aggiungere persone come lead in una campagna Salesforce. Se il lead non esiste ancora in Salesforce, viene sincronizzato automaticamente e aggiunto alla campagna con lo stato specificato.

![](assets/image2014-9-22-15-3a43-3a36.png)

## Utilizzo {#usage}

1. Trova e seleziona la campagna Salesforce a cui desideri aggiungere i lead.

   ![](assets/image2014-9-22-15-3a43-3a45.png)

   >[!TIP]
   >
   >Se non puoi visualizzare una campagna Salesforce nell’elenco Campaign:
   >
   >  1. Assicurati che [la sincronizzazione della campagna è abilitata](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
   >  1. Conferma che la tua [Marketo Sync User](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) è un [Utente marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) a Salesforce.


   >[!TIP]
   >
   >Puoi utilizzare la campagna Salesforce [Token personali](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) per semplificare la clonazione dei programmi.

1. Selezionare lo stato del membro della campagna Salesforce che si desidera assegnare ai lead quando vengono aggiunti.

   ![](assets/image2014-9-22-15-3a45-3a2.png)

   >[!CAUTION]
   >
   >Se una persona è già un membro principale della campagna Salesforce, verrà saltata e il suo stato NON verrà aggiornato. È possibile utilizzare [modificare il loro stato in una campagna SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md) invece.
