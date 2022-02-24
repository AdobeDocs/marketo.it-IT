---
description: Override prioritario per campagne trigger - Documenti Marketo - Documentazione del prodotto
title: Override prioritario per le campagne trigger
hide: true
hidefromtoc: true
source-git-commit: f2b6e0ae4759ed279d4c02ae922e9deba838b1ff
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Override prioritario per le campagne trigger {#priority-override-for-trigger-campaigns}

Gli amministratori possono ignorare la priorità determinata di Marketo per attivare le campagne al fine di impostare priorità più allineate con gli obiettivi aziendali.

>[!NOTE]
>
>Questa funzione è disponibile solo per le campagne di attivazione e per gli utenti a cui è stato concesso il [Autorizzazione &quot;Modifica priorità impulso campagna&quot;](#grant-priority-override-access).

>[!CAUTION]
>
>È consigliabile utilizzare questa funzione in un set limitato di campagne business critical (25 è il massimo consigliato). L’utilizzo approssimativo della funzione su un set di grandi dimensioni può influenzare negativamente l’esecuzione complessiva della campagna.

## Accesso alla priorità di sovvenzione {#grant-priority-override-access}

>[!CAUTION]
>
>Solo gli amministratori o gli utenti con responsabilità di amministratore devono avere la priorità della campagna che sovrascrivono l’accesso.

1. In [!UICONTROL Amministratore] area, fai clic su **[!UICONTROL Utenti e ruoli]**.

   ![](assets/priority-override-for-trigger-campaigns-1.png)

1. Fai clic sul pulsante **[!UICONTROL Ruoli]** selezionare l&#39;utente a cui si desidera concedere l&#39;accesso, quindi fare clic su **[!UICONTROL Modifica ruolo]**.

   ![](assets/priority-override-for-trigger-campaigns-2.png)

1. Sotto [!UICONTROL Accedere alle attività di marketing], seleziona **[!UICONTROL Modifica priorità campagna trigger]**. Fai clic su **[!UICONTROL Salva]**.

   ![](assets/priority-override-for-trigger-campaigns-3.png)

## Ignora priorità {#override-priority}

1. Individua la campagna trigger. Fai clic con il pulsante destro del mouse su di esso e seleziona **[!UICONTROL Ignora priorità campagna]**.

   ![](assets/priority-override-for-trigger-campaigns-4.png)

1. Fai clic sul pulsante **[!UICONTROL Ignora priorità campagna]** cursore per attivare. Scegli un nuovo livello di priorità e fai clic su **[!UICONTROL Conferma]**.

   ![](assets/priority-override-for-trigger-campaigns-5.png)

   Il nuovo livello di priorità verrà visualizzato nella scheda Pianificazione .

   ![](assets/priority-override-for-trigger-campaigns-6.png)

>[!NOTE]
>
>* Puoi visualizzare la priorità predefinita della campagna nella [!UICONTROL Coda campagna] sotto [!UICONTROL Attività di marketing]. Per incrementare il tasso di esecuzione, ti consigliamo di impostare la priorità della campagna su un livello superiore rispetto a quello predefinito.
>* La priorità definita dall&#39;utente si applica solo alle nuove persone che si qualificano per la campagna; le persone già in coda non saranno interessate.
>* Le sostituzioni prioritarie vengono acquisite in [Audit Trail](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md).

