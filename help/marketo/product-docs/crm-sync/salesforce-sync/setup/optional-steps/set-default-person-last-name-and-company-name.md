---
unique-page-id: 4719291
description: Impostare il cognome e il nome società della persona predefinita - Documenti Marketo - Documentazione del prodotto
title: Imposta cognome persona e nome società predefiniti
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---

# Imposta cognome persona e nome società predefiniti {#set-default-person-last-name-and-company-name}

Salesforce richiede (almeno) il cognome e il nome della società per i lead e i contatti. I record incompleti non verranno sincronizzati con Salesforce. Se si desidera sincronizzare record parziali, è necessario impostare i valori predefiniti per Marketo da utilizzare con Salesforce.

1. Vai a **Amministratore** e fai clic su **Salesforce**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. Clic **Modifica opzioni di sincronizzazione**.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. Immetti un **Cognome persona predefinito** e un **Società persona predefinita** quindi fai clic su **Salva**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo assegna un valore predefinito solo quando il record viene sincronizzato inizialmente con Salesforce e solo se uno dei campi obbligatori è vuoto.

E questo è quanto! Ogni volta che a una persona mancano un cognome e/o il nome della società, Marketo aggiungerà il valore predefinito mentre sincronizza il record.
