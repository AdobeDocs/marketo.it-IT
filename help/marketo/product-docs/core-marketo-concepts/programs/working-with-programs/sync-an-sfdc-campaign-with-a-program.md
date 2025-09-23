---
unique-page-id: 1147154
description: Sincronizzare una campagna SFDC con un programma - Documentazione Marketo - Documentazione del prodotto
title: Sincronizzare una campagna SFDC con un programma
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
feature: Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 10%

---

# Sincronizzare una campagna SFDC con un programma {#sync-an-sfdc-campaign-with-a-program}

Marketo Engage consente di sincronizzare i programmi con le campagne [!DNL Salesforce] per mantenere lo stesso elenco di persone in entrambi i sistemi, inclusi i relativi stati. Cominciamo.

>[!PREREQUISITES]
>
>Devi prima [abilitare [!DNL Salesforce] la sincronizzazione della campagna](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}.

>[!CAUTION]
>
>Quando si sincronizza una campagna SFDC con un programma Marketo Engage, le azioni implicite di SFDC (ad esempio, aggiungi a SFDC Campaign, Sincronizza con SFDC) verranno disabilitate per le campagne secondarie del programma.

1. Vai a **[!UICONTROL Marketing Activities]**.

   ![](assets/login-marketing-activities-1.png)

1. Seleziona il programma.

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. Fai clic su **[!UICONTROL Program Actions]**, quindi seleziona **[!UICONTROL Salesforce Campaign Sync]**.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. Seleziona **[!UICONTROL Create New]** o scegli una campagna [!DNL Salesforce] esistente.

   >[!TIP]
   >
   >Se selezioni una campagna [!DNL Salesforce] esistente, assicurati di [corrispondere agli stati del programma  [!DNL Salesforce] della campagna e del programma Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md){target="_blank"}.

1. Immettere un nome per la nuova campagna e fare clic su **[!UICONTROL Save]**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. Ora puoi verificare i dettagli di sincronizzazione della campagna nella pagina di riepilogo del programma.

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   Eccellente! Ora tutte le modifiche di stato del programma in Marketo vengono sincronizzate con la campagna SFDC e viceversa.
