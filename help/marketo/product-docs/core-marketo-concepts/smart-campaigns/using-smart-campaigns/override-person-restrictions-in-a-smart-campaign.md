---
unique-page-id: 1147066
description: Escludere le limitazioni di persona in una campagna intelligente - Documenti Marketo - Documentazione del prodotto
title: Escludere le limitazioni di persona in una campagna intelligente
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# Escludere le limitazioni di persona in una campagna intelligente {#override-person-restrictions-in-a-smart-campaign}

Marketo consente di impostare il numero massimo* *di persone idonee per una campagna intelligente; in questo modo si evita di inviare accidentalmente l&#39;intero database. Se vuoi *ignorare* questo limite, ecco come.

>[!NOTE]
>
>**FYI**
>
>Marketo sta standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che nell&#39;abbonamento siano presenti lead/lead e persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

>[!NOTE]
>
>**Prerequisiti**
>
>Assicurati di [abilitare le restrizioni per le persone per le campagne](../../../../product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) intelligenti in Marketo Admin.

1. In Marketing Activities (Attività di marketing), andate alla campagna** **smart e fate clic su **Schedule (Pianificazione**).

   ![](assets/one.png)

   In Impostazioni Smart Campaign, fai clic su Modifica .
   ![](assets/two.png)

   >[!NOTE]
   >
   >Il limite predefinito è quello impostato in Amministratore.

1. Immettete un nuovo limite e fate clic su **Salva.**

   ![](assets/three.png)

   La campagna smart non verrà eseguita se il numero di persone idonee supera il limite impostato.

   >[!CAUTION]
   >
   >Prestate attenzione con questa funzione in modo da non includere accidentalmente troppe persone.

