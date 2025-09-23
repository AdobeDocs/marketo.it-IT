---
description: Sovrascrittura delle priorità per le campagne Trigger - Documenti Marketo - Documentazione del prodotto
title: Sovrascrive priorità per campagne trigger
exl-id: cf9b4d27-0e4c-40cf-accd-4f4a102160cc
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 4%

---

# Sovrascrive priorità per campagne trigger {#priority-override-for-trigger-campaigns}

Gli amministratori possono ignorare la priorità determinata da Marketo Engage per Attivare le campagne per impostare priorità che si allineano meglio agli obiettivi aziendali.

>[!NOTE]
>
>Questa funzionalità è disponibile solo per le campagne Trigger e per gli utenti che dispongono dell&#39;autorizzazione [&quot;Modifica priorità campagna Trigger&quot;](#grant-priority-override-access).

>[!CAUTION]
>
>Si consiglia vivamente di utilizzare questa funzione su un set limitato di campagne aziendali critiche (25 è il massimo consigliato). L’utilizzo generico della funzione su un set di grandi dimensioni può influire negativamente sull’esecuzione complessiva della campagna.

## Concedi accesso di sostituzione priorità {#grant-priority-override-access}

>[!NOTE]
>
>Solo gli amministratori o gli utenti con responsabilità di amministratore devono avere accesso con priorità alla sostituzione della campagna.

1. Nell&#39;area **[!UICONTROL Admin]** fare clic su **[!UICONTROL Users & Roles]**.

   ![](assets/priority-override-for-trigger-campaigns-1.png)

1. Fare clic sulla scheda **[!UICONTROL Roles]**, selezionare l&#39;utente a cui si desidera concedere l&#39;accesso, quindi fare clic su **[!UICONTROL Edit Role]**.

   ![](assets/priority-override-for-trigger-campaigns-2.png)

1. In **[!UICONTROL Access Marketing Activities]**, selezionare **[!UICONTROL Edit Trigger Campaign Priority]**. Fai clic su **[!UICONTROL Save]**.

   ![](assets/priority-override-for-trigger-campaigns-3.png)

## Sovrascrivi priorità {#override-priority}

1. Individua la campagna Trigger. Fare clic con il pulsante destro del mouse e selezionare **[!UICONTROL Override Campaign Priority]**.

   ![](assets/priority-override-for-trigger-campaigns-4.png)

1. Fare clic sul dispositivo di scorrimento **[!UICONTROL Override Campaign Priority]** per attivarlo. Scegliere un nuovo livello di priorità e fare clic su **[!UICONTROL Confirm]**.

   ![](assets/priority-override-for-trigger-campaigns-5.png)

   Il nuovo livello di priorità verrà visualizzato nella scheda **[!UICONTROL Schedule]**.

   ![](assets/priority-override-for-trigger-campaigns-6.png)

>[!NOTE]
>
>* Puoi visualizzare la priorità predefinita della tua campagna in [!UICONTROL Campaign Queue] in [!UICONTROL Marketing Activities]. Per aumentare il tasso di esecuzione, si consiglia di impostare la priorità della campagna su un livello più alto del valore predefinito.
>* La priorità impostata dall&#39;utente si applica solo alle nuove persone che si qualificano per la campagna; le persone già in coda non saranno interessate.
>* Le sostituzioni di priorità vengono acquisite in [Audit Trail](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md){target="_blank"}.
