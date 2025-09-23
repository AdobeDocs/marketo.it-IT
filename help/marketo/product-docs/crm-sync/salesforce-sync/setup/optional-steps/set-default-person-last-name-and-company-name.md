---
unique-page-id: 4719291
description: Impostare il cognome e il nome società della persona predefinita - Documenti Marketo - Documentazione del prodotto
title: Impostare cognome persona e nome azienda predefiniti
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '127'
ht-degree: 13%

---

# Impostare cognome persona e nome azienda predefiniti {#set-default-person-last-name-and-company-name}

[!DNL Salesforce] richiede (minimo) il cognome e il nome della società per i lead e i contatti. I record incompleti non verranno sincronizzati con [!DNL Salesforce]. Se si desidera sincronizzare i record parziali, è necessario impostare i valori predefiniti per Marketo da utilizzare con [!DNL Salesforce].

1. Vai a **[!UICONTROL Admin]** e fai clic su **[!DNL Salesforce]**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. Fai clic su **[!UICONTROL Edit Sync Options]**.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. Immettere **[!UICONTROL Default person last name]** e **[!UICONTROL Default person company]**, quindi fare clic su **[!UICONTROL Save]**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo Engage assegna un valore predefinito solo quando il record viene inizialmente sincronizzato con Salesforce e solo se uno dei campi obbligatori è vuoto.

E questo è quanto! Ogni volta che a una persona mancano un cognome e/o il nome della società, Marketo aggiungerà il valore predefinito mentre sincronizza il record.
