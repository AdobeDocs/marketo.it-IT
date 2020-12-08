---
unique-page-id: 1147154
description: Sincronizzazione di una campagna SFDC con un programma - Marketo Docs - Documentazione del prodotto
title: Sincronizzazione di una campagna SFDC con un programma
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---


# Sincronizzazione di una campagna SFDC con un programma {#sync-an-sfdc-campaign-with-a-program}

Marketo consente di sincronizzare i programmi con le campagne Salesforce per mantenere lo stesso elenco di persone in entrambi i sistemi, inclusi i loro stati. Cominciamo!

>[!NOTE]
>
>**Prerequisiti**
>
>Devi prima [abilitare la sincronizzazione](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md) della campagna Salesforce.

>[!CAUTION]
>
>Quando si sincronizza una campagna SFDC con un programma Marketo, le azioni implicite della DSC (ad esempio, aggiungere alla campagna SFDC, sincronizzare con la DSC) verranno disattivate per le campagne figlio del programma.

1. Vai a Attività **** di marketing.

   ![](assets/login-marketing-activities-1.png)

1. Selezionare il programma.

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. Fai clic su Azioni **** programma, quindi seleziona Sincronizzazione **campagna** Salesforce.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. Seleziona **Crea nuovo **o scegli una campagna Salesforce esistente.

   >[!TIP]
   >
   >Se selezioni una campagna Salesforce esistente, accertati di [corrispondere agli stati del programma della campagna Salesforce e del programma](../../../../product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-errors/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md)Marketo.

1. Immettete un nome per la nuova campagna e fate clic su **Salva**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. Ora potete verificare i dettagli di sincronizzazione della campagna nella pagina di riepilogo del programma.

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   Eccellente! Le modifiche dello stato dei programmi apportate a Marketo vengono ora sincronizzate con la campagna SFDC e viceversa.

