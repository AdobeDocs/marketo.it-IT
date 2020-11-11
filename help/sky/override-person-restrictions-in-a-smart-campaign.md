---
title: override-persona-restrictions-in-a-smart-campaign
description: Escludere le limitazioni di persona in una campagna intelligente
translation-type: tm+mt
source-git-commit: 642fd57105afff1031f18883c5809206f136b7c6
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---


# Escludere le limitazioni di persona in una campagna intelligente

<br> 

Marketo consente di impostare il numero massimo di persone idonee per una campagna intelligente; in questo modo si evita di inviare accidentalmente l&#39;intero database. Se vuoi superare questo limite, ecco come.

>[!IMPORTANT]
>
>Assicurati di [abilitare le restrizioni per le persone per le campagne](https://docs.marketo.com/display/DOCS/Enable+Person+Restrictions+for+Smart+Campaigns) intelligenti in Marketo [!UICONTROL Admin].

1. Individuate la campagna intelligente e fate clic su [!UICONTROL **Pianificazione**].

   ![Immagine uno](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-1.png)

1. Fate clic su Regole [!UICONTROL **di qualifica**].

   ![Immagine due](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >Il limite predefinito è quello impostato in Amministratore.

1. Accanto a [!UICONTROL **Interrompi campagna se i lead qualificati superano**], immettete un nuovo limite.

   ![Immagine tre](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-3.png)

>[!NOTE]
>
>La campagna smart non verrà eseguita se il numero di persone idonee supera il limite impostato.

>[!CAUTION]
>
>Fai attenzione a questa funzione per non includere accidentalmente troppe persone.
