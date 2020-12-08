---
unique-page-id: 4719291
description: Imposta Cognome utente e Nome società predefiniti - Documenti Marketo - Documentazione prodotto
title: Imposta cognome persona e nome società predefiniti
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---


# Imposta cognome persona e nome società predefiniti {#set-default-person-last-name-and-company-name}

Per i lead e i contatti di Salesforce sono necessari (minimo) cognome e nome società. I record incompleti non verranno sincronizzati con Salesforce. Se desideri sincronizzare record parziali, devi impostare i valori predefiniti per Marketo da usare con Salesforce.

1. Vai ad **Admin** e fai clic su **Salesforce**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. Fate clic su **Modifica opzioni** sincronizzazione.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. Immettete un cognome **** predefinito per la persona e una società&#x200B;****** persona predefinita, quindi fate clic su **Salva**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo assegna un valore predefinito solo quando il record viene inizialmente sincronizzato con Salesforce e solo se uno dei campi obbligatori è vuoto.

Ed è questo! Ogni volta che a una persona manca un cognome e/o un nome della società, Marketo aggiunge il valore predefinito durante la sincronizzazione del record.
