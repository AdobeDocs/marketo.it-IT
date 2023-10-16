---
unique-page-id: 1147154
description: Sincronizzare una campagna SFDC con un programma - Documenti Marketo - Documentazione del prodotto
title: Sincronizzare una campagna SFDC con un programma
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
feature: Programs
source-git-commit: 9e51ece12742152040dbbcb6a1584fba28e863ff
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 0%

---

# Sincronizzare una campagna SFDC con un programma {#sync-an-sfdc-campaign-with-a-program}

Marketi Engage consente di sincronizzare i programmi con [!DNL Salesforce] campagne per mantenere lo stesso elenco di persone in entrambi i sistemi, inclusi i relativi stati. Iniziamo!

>[!PREREQUISITES]
>
>Sarà necessario [abilita [!DNL Salesforce] sincronizzazione campagne](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"} prima.

>[!CAUTION]
>
>Durante la sincronizzazione di una campagna SFDC con un programma di Marketo Engage, le azioni SFDC implicite (ad esempio, aggiungi a Campagna SFDC, Sincronizza con SFDC) verranno disabilitate per le campagne secondarie del programma.

1. Vai a **[!UICONTROL Attività di marketing]**.

   ![](assets/login-marketing-activities-1.png)

1. Seleziona il programma.

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. Clic **[!UICONTROL Azioni del programma]**, quindi seleziona **[!UICONTROL Sincronizzazione campagna Salesforce]**.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. Seleziona **[!UICONTROL Crea nuovo]** o scegli un elemento esistente [!DNL Salesforce] campagna.

   >[!TIP]
   >
   >Se si seleziona un elemento esistente [!DNL Salesforce] campagna, assicurati di [corrisponde agli stati del programma di [!DNL Salesforce] e il programma Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md){target="_blank"}.

1. Immetti un nome per la nuova campagna e fai clic su **[!UICONTROL Salva]**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. Ora puoi verificare i dettagli di sincronizzazione della campagna nella pagina di riepilogo del programma.

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   Eccellente! Ora tutte le modifiche di stato del programma in Marketo vengono sincronizzate con la campagna SFDC e viceversa.
