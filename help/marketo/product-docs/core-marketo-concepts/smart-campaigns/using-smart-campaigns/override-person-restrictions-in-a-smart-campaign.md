---
unique-page-id: 1147066
description: Sovrascrivere le restrizioni relative alla persona in una campagna intelligente - Documenti Marketo - Documentazione del prodotto
title: Sovrascrivere le restrizioni relative alla persona in una campagna avanzata
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '132'
ht-degree: 10%

---

# Sovrascrivere le restrizioni relative alla persona in una campagna avanzata {#override-person-restrictions-in-a-smart-campaign}

Marketo Engage consente di impostare il numero massimo di persone idonee per una campagna avanzata, in modo da evitare di inviare accidentalmente e-mail all’intero database. Se desideri _ignorare_ questo limite, ecco come.

>[!PREREQUISITES]
>
>Assicurati di [abilitare le restrizioni per le persone per Smart Campaigns](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md){target="_blank"} in Marketo Admin.

1. In **[!UICONTROL Marketing Activities]**, vai alla tua Smart Campaign e fai clic su **[!UICONTROL Schedule]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-1.png)

1. In Impostazioni Smart Campaign, fare clic su **[!UICONTROL Edit]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >Il limite predefinito è quello impostato in Amministratore.

1. Immettere un nuovo limite e fare clic su **[!UICONTROL Save]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-3.png)

   La campagna avanzata non verrà eseguita se il numero di persone idonee supera il limite impostato.

   >[!CAUTION]
   >
   >Presta attenzione con questa funzione in modo da non includere accidentalmente troppe persone.
