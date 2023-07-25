---
unique-page-id: 1147066
description: Sovrascrivere le restrizioni relative alla persona in una campagna intelligente - Documenti Marketo - Documentazione del prodotto
title: Sovrascrivere le restrizioni relative alla persona in una campagna intelligente
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 0%

---

# Sovrascrivere le restrizioni relative alla persona in una campagna intelligente {#override-person-restrictions-in-a-smart-campaign}

Marketo consente di impostare il numero massimo di persone che possono qualificarsi per una campagna intelligente; in questo modo è possibile evitare di inviare accidentalmente e-mail all’intero database. Se vuoi _sostituire_ questo limite, ecco come.

>[!PREREQUISITES]
>
>Assicurati di [abilita restrizioni persona per campagne intelligenti](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) in Amministrazione Marketo.

1. In Attività di marketing, vai alla tua campagna intelligente e fai clic su **Pianificazione**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-1.png)

1. In Impostazioni campagna avanzata, fai clic su **Modifica**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >Il limite predefinito è quello impostato in Amministratore.

1. Inserisci un nuovo limite e fai clic su **Salva.**

   ![](assets/override-person-restrictions-in-a-smart-campaign-3.png)

   La campagna intelligente non verrà eseguita se il numero di persone idonee supera il limite impostato.

   >[!CAUTION]
   >
   >Presta attenzione con questa funzione in modo da non includere accidentalmente troppe persone.
