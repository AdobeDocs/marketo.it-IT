---
title: priorità-override-per-trigger-campaign
description: Override di priorità per le campagne di attivazione
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---


# Override di priorità per le campagne di attivazione

<br> 

Gli amministratori possono ignorare la priorità determinata di Marketo per attivare le campagne per impostare priorità che meglio si allineano con gli obiettivi aziendali.

>[!NOTE]
>
>Questa funzione è disponibile solo per le campagne di attivazione e per gli utenti ai quali è stata concessa l&#39;autorizzazione &quot;Modifica priorità campagna trigger&quot;.

>[!CAUTION]
>
>Si consiglia vivamente di utilizzare questa funzione in una serie limitata di campagne business critical (25 rappresenta il massimo consigliato). L&#39;utilizzo della funzione vagamente su un set di grandi dimensioni può influenzare negativamente l&#39;esecuzione della campagna nel suo complesso.

## Priorità di sostituzione

1. Nella campagna di attivazione, fare clic sulla **[!UICONTROL Schedule]** scheda, quindi su **[!UICONTROL Override Priority]**.

   ![Immagine uno](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-1.png)

1. Scegliete un nuovo livello di priorità dal menu a discesa. Fate clic **[!UICONTROL Confirm]**.

   ![Immagine due](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-2.png)

   ![Immagine tre](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-3.png)

>[!NOTE]
>
>* Potete visualizzare la priorità predefinita della campagna nella [!UICONTROL Campaign Queue] sezione [!UICONTROL Marketing Activities]. Per aumentare il tasso di esecuzione, si consiglia di impostare la priorità della campagna su un livello superiore a quello predefinito.
>* La priorità definita dall&#39;utente si applica solo alle nuove persone idonee alla campagna; le persone che sono già in coda non ne verranno interessate.


## Ripristina priorità

1. Per ripristinare la priorità della campagna all&#39;impostazione predefinita del sistema, andate alla **[!UICONTROL Schedule]** scheda nella campagna di attivazione e fate clic su **[!UICONTROL Reset Priority]**.

   ![Immagine quattro](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-4.png)

1. Fate clic **[!UICONTROL Reset]** per confermare.

   ![Immagine cinque](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-5.png)

>[!NOTE]
>
>Le sostituzioni e i ripristini con priorità vengono acquisiti nella traccia di audit. Potete visualizzare la traccia di [controllo](https://docs.marketo.com/x/GZ2t) nell&#39;area [!UICONTROL Admin] dell&#39;esperienza classica.

## Accesso all&#39;override della priorità di sovvenzione

>[!CAUTION]
>
>Solo gli amministratori o gli utenti con responsabilità di amministratore devono avere la priorità della campagna come accesso alternativo.

1. Nell&#39; [!UICONTROL Admin] area fare clic su **[!UICONTROL Users & Roles]**.

   ![Immagine Sei](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-6.png)

1. Fate clic sulla **[!UICONTROL Roles]** scheda, selezionate l&#39;utente a cui concedere l&#39;accesso, quindi fate clic su **[!UICONTROL Edit Role]**.

   ![Immagine sette](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-7.png)

1. Sotto [!UICONTROL Access Marketing Activities], check **[!UICONTROL Edit Trigger Campaign Priority]**. Fate clic **[!UICONTROL Save]**.

   ![Immagine otto](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-8.png)

## Visualizza priorità campagna in Marketo Classic

Per visualizzare la priorità della campagna nell&#39; [!DNL Classic] esperienza, fai clic sulla **[!UICONTROL Schedule]** scheda all&#39;interno di una campagna di attivazione.

![Image Nine](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-9.png)

>[!NOTE]
>
>La priorità nell&#39; [!DNL Classic] esperienza è di sola visualizzazione. La modifica o il ripristino della priorità della campagna è disponibile solo tramite Marketo Sky.
