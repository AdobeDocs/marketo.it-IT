---
unique-page-id: 1147154
description: Sincronizzare una campagna SFDC con un programma - Documenti Marketo - Documentazione del prodotto
title: Sincronizzare una campagna SFDC con un programma
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# Sincronizzare una campagna SFDC con un programma {#sync-an-sfdc-campaign-with-a-program}

Marketo consente di sincronizzare i programmi con le campagne Salesforce per mantenere lo stesso elenco di persone in entrambi i sistemi, inclusi i relativi stati. Iniziamo!

>[!PREREQUISITES]
>
>Sarà necessario [abilita sincronizzazione campagne Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md) prima.

>[!CAUTION]
>
>Durante la sincronizzazione di una campagna SFDC con un programma Marketo, le azioni SFDC implicite (ad esempio, aggiungi a Campagna SFDC, Sincronizza con SFDC) verranno disabilitate per le campagne secondarie del programma.

1. Vai a **Attività di marketing**.

   ![](assets/login-marketing-activities-1.png)

1. Seleziona il programma.

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. Clic **Azioni del programma**, quindi seleziona **Sincronizzazione campagna Salesforce**.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. Seleziona **Crea nuovo** o scegli una campagna Salesforce esistente.

   >[!TIP]
   >
   >Se selezioni una campagna Salesforce esistente, assicurati di [corrisponde agli stati del programma della campagna Salesforce e del programma Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

1. Immetti un nome per la nuova campagna e fai clic su **Salva**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. Ora puoi verificare i dettagli di sincronizzazione della campagna nella pagina di riepilogo del programma.

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   Eccellente! Ora tutte le modifiche di stato del programma in Marketo vengono sincronizzate con la campagna SFDC e viceversa.
