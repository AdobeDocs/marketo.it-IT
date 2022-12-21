---
unique-page-id: 1147066
description: Escludere le restrizioni relative alle persone in una campagna avanzata - Documenti Marketo - Documentazione del prodotto
title: Escludere le restrizioni relative alle persone in una campagna avanzata
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 0%

---

# Escludere le restrizioni relative alle persone in una campagna avanzata {#override-person-restrictions-in-a-smart-campaign}

Marketo consente di impostare il numero massimo di persone idonee per una campagna intelligente; questo consente di evitare di inviare accidentalmente un&#39;e-mail all&#39;intero database. Se vuoi _override_ questo limite, ecco come.

>[!PREREQUISITES]
>
>Assicurati di [abilitare le restrizioni per le persone per le campagne intelligenti](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) in Marketo Admin.

1. In Attività di marketing, accedi alla tua campagna intelligente e fai clic su **Pianificazione**.

   ![](assets/one.png)

1. In Impostazioni di Smart Campaign, fai clic su **Modifica**.

   ![](assets/two.png)

   >[!NOTE]
   >
   >Il limite predefinito è quello impostato in Amministratore.

1. Inserisci un nuovo limite e fai clic su **Salva.**

   ![](assets/three.png)

   La campagna intelligente non verrà eseguita se il numero di persone idonee supera il limite impostato.

   >[!CAUTION]
   >
   >Presta attenzione con questa funzione in modo da non includere accidentalmente troppe persone.
