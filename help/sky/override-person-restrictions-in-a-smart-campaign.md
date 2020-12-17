---
title: override-persona-restrictions-in-a-smart-campaign
description: Escludere le limitazioni di persona in una campagna intelligente
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '130'
ht-degree: 0%

---


# Escludere le limitazioni di persona in una campagna intelligente

<br> 

Marketo consente di impostare il numero massimo di persone idonee per una campagna intelligente; in questo modo si evita di inviare accidentalmente l&#39;intero database. Se vuoi superare questo limite, ecco come.

>[!IMPORTANT]
>
>Assicurati di [abilitare le restrizioni per le persone per le campagne intelligenti](https://docs.marketo.com/display/DOCS/Enable+Person+Restrictions+for+Smart+Campaigns) in Marketo [!UICONTROL Admin].

1. Individuate la campagna intelligente e fate clic su **[!UICONTROL Schedule]**.

   ![Immagine uno](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-1.png)

1. Fare clic su **[!UICONTROL Qualification Rules]**.

   ![Immagine due](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >Il limite predefinito è quello impostato in Amministratore.

1. Accanto a **[!UICONTROL Abort campaign if qualified leads exceed]**, immettere un nuovo limite.

   ![Immagine tre](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-3.png)

>[!NOTE]
>
>La campagna smart non verrà eseguita se il numero di persone idonee supera il limite impostato.

>[!CAUTION]
>
>Fai attenzione a questa funzione per non includere accidentalmente troppe persone.
