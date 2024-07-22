---
unique-page-id: 1147066
description: Sovrascrivere le restrizioni relative alla persona in una campagna intelligente - Documenti Marketo - Documentazione del prodotto
title: Sovrascrivere le restrizioni relative alla persona in una campagna intelligente
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
source-git-commit: 47bc93665a7efa0d64cd4d5f34b868895d407527
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---

# Sovrascrivere le restrizioni relative alla persona in una campagna intelligente {#override-person-restrictions-in-a-smart-campaign}

Il Marketo Engage consente di impostare il numero massimo di persone che possono qualificarsi per una campagna intelligente; in questo modo è possibile evitare di inviare accidentalmente e-mail all’intero database. Se desideri _ignorare_ questo limite, ecco come.

>[!PREREQUISITES]
>
>Assicurati di [abilitare le restrizioni per le persone per Smart Campaigns](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md){target="_blank"} in Marketo Admin.

1. In **[!UICONTROL Attività di marketing]**, vai alla tua Smart Campaign e fai clic su **[!UICONTROL Pianifica]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-1.png)

1. In Impostazioni Smart Campaign, fai clic su **[!UICONTROL Modifica]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >Il limite predefinito è quello impostato in Amministratore.

1. Inserisci un nuovo limite e fai clic su **[!UICONTROL Salva]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-3.png)

   La campagna avanzata non verrà eseguita se il numero di persone idonee supera il limite impostato.

   >[!CAUTION]
   >
   >Presta attenzione con questa funzione in modo da non includere accidentalmente troppe persone.
