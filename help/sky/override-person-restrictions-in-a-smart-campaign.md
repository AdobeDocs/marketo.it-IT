---
title: override-person-limits-in-a-smart-campaign
description: Escludere le restrizioni relative alle persone in una campagna avanzata
exl-id: efdd6c68-a95e-4b2a-9249-e2e1f550b628
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '130'
ht-degree: 0%

---

# Escludere le restrizioni relative alle persone in una campagna avanzata

<br> 

Marketo consente di impostare il numero massimo di persone idonee per una campagna intelligente; questo consente di evitare di inviare accidentalmente un&#39;e-mail all&#39;intero database. Se desideri ignorare questo limite, ecco come.

>[!IMPORTANT]
>
>Assicurati di [abilitare le restrizioni alle persone per le campagne intelligenti](https://docs.marketo.com/display/DOCS/Enable+Person+Restrictions+for+Smart+Campaigns) in Marketo [!UICONTROL Admin].

1. Trova la tua campagna avanzata e fai clic su **[!UICONTROL Schedule]**.

   ![Immagine uno](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-1.png)

1. Fai clic **[!UICONTROL Qualification Rules]**.

   ![Immagine 2](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >Il limite predefinito è quello impostato in Amministratore.

1. Accanto a **[!UICONTROL Abort campaign if qualified leads exceed]**, immetti un nuovo limite.

   ![Immagine tre](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-3.png)

>[!NOTE]
>
>La campagna intelligente non verrà eseguita se il numero di persone idonee supera il limite impostato.

>[!CAUTION]
>
>Presta attenzione con questa funzione in modo da non includere accidentalmente troppe persone.
