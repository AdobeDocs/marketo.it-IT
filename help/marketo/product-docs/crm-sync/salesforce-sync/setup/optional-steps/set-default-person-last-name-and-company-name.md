---
unique-page-id: 4719291
description: Imposta il cognome e il nome della società predefiniti - Marketo Docs - Documentazione del prodotto
title: Imposta Cognome persona predefinito e Nome società
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---

# Imposta Cognome persona predefinito e Nome società {#set-default-person-last-name-and-company-name}

Salesforce richiede il cognome (minimo) e il nome della società per i suoi Lead e Contatti. I record incompleti non verranno sincronizzati con Salesforce. Se desideri sincronizzare i record parziali, devi impostare i valori predefiniti per Marketo da utilizzare con Salesforce.

1. Vai a **Amministratore** e fai clic su **Salesforce**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. Fai clic su **Modifica opzioni di sincronizzazione**.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. Inserisci un **Cognome persona predefinito** e **Società a persona predefinita** quindi fai clic su **Salva**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo assegna un valore predefinito solo quando il record viene inizialmente sincronizzato con Salesforce e solo se uno dei campi obbligatori è vuoto.

Ed è questo! Ogni volta che a una persona manca un cognome e/o un nome società, Marketo aggiunge il valore predefinito durante la sincronizzazione del record.
