---
unique-page-id: 1147154
description: Sincronizzare una campagna SFDC con un programma - Marketo Docs - Documentazione del prodotto
title: Sincronizzazione di una campagna SFDC con un programma
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# Sincronizzazione di una campagna SFDC con un programma {#sync-an-sfdc-campaign-with-a-program}

Marketo consente di sincronizzare i programmi con le campagne Salesforce per mantenere lo stesso elenco di persone in entrambi i sistemi, inclusi i relativi stati. Cominciamo!

>[!PREREQUISITES]
>
>Devi prima [abilitare la sincronizzazione della campagna Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).

>[!CAUTION]
>
>Quando si sincronizza una campagna SFDC con un programma Marketo, le azioni SFDC implicite (ad esempio, aggiungi alla campagna SFDC, Sincronizza con SFDC) verranno disabilitate per le campagne figlio del programma.

1. Vai a **Attività di marketing**.

   ![](assets/login-marketing-activities-1.png)

1. Selezionare il programma.

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. Fai clic su **Azioni programma**, quindi seleziona **Salesforce Campaign Sync**.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. Seleziona **Crea nuovo** o scegli una campagna Salesforce esistente.

   >[!TIP]
   >
   >Se selezioni una campagna Salesforce esistente, assicurati di [corrispondere agli stati del programma della campagna Salesforce e del programma Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-errors/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

1. Inserisci un nome per la nuova campagna e fai clic su **Salva**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. Ora puoi verificare i dettagli di sincronizzazione della campagna nella pagina di riepilogo del programma.

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   Eccellente! Ora qualsiasi modifica dello stato del programma in Marketo viene sincronizzata con la campagna SFDC e viceversa.
