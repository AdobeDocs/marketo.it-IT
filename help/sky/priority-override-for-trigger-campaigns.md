---
title: priority-override-for-trigger-campagne
description: Override prioritario per le campagne trigger
exl-id: 4468868c-33d7-4b5e-b524-bfcc2785c8ce
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---

# Override prioritario per le campagne trigger

<br> 

Gli amministratori possono ignorare la priorità determinata di Marketo per attivare le campagne al fine di impostare priorità più allineate con gli obiettivi aziendali.

>[!NOTE]
>
>Questa funzione è disponibile solo per le campagne trigger e per gli utenti a cui è stata concessa l’autorizzazione &quot;Modifica priorità campagna trigger&quot;.

>[!CAUTION]
>
>È consigliabile utilizzare questa funzione in un set limitato di campagne business critical (25 è il massimo consigliato). L’utilizzo approssimativo della funzione su un set di grandi dimensioni può influenzare negativamente l’esecuzione complessiva della campagna.

## Ignora priorità

1. Nella campagna trigger, fai clic sulla scheda **[!UICONTROL Schedule]** , quindi fai clic su **[!UICONTROL Override Priority]**.

   ![Immagine uno](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-1.png)

1. Scegli un nuovo livello di priorità dal menu a discesa. Fai clic **[!UICONTROL Confirm]**.

   ![Immagine 2](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-2.png)

   ![Immagine tre](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-3.png)

>[!NOTE]
>
>* Puoi visualizzare la priorità predefinita della campagna in [!UICONTROL Campaign Queue] in [!UICONTROL Marketing Activities]. Per incrementare il tasso di esecuzione, ti consigliamo di impostare la priorità della campagna su un livello superiore rispetto a quello predefinito.
>* La priorità definita dall&#39;utente si applica solo alle nuove persone che si qualificano per la campagna; le persone già in coda non saranno interessate.


## Reimposta priorità

1. Per ripristinare la priorità della campagna all’impostazione predefinita del sistema, vai alla scheda **[!UICONTROL Schedule]** nella campagna trigger e fai clic su **[!UICONTROL Reset Priority]**.

   ![Immagine quattro](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-4.png)

1. Fai clic su **[!UICONTROL Reset]** per confermare.

   ![Immagine cinque](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-5.png)

>[!NOTE]
>
>Le sostituzioni e i reinsiemi con priorità vengono acquisiti in Audit Trail. Puoi visualizzare [Audit Trail](https://docs.marketo.com/x/GZ2t) attraverso l&#39;area [!UICONTROL Admin] nell&#39;esperienza classica.

## Accesso alla priorità di sovvenzione

>[!CAUTION]
>
>Solo gli amministratori o gli utenti con responsabilità di amministratore devono avere la priorità della campagna che sovrascrivono l’accesso.

1. Nell’area [!UICONTROL Admin], fai clic su **[!UICONTROL Users & Roles]**.

   ![Immagine Sei](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-6.png)

1. Fare clic sulla scheda **[!UICONTROL Roles]**, selezionare l&#39;utente a cui si desidera concedere l&#39;accesso, quindi fare clic su **[!UICONTROL Edit Role]**.

   ![Immagine sette](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-7.png)

1. Sotto [!UICONTROL Access Marketing Activities], controllare **[!UICONTROL Edit Trigger Campaign Priority]**. Fai clic **[!UICONTROL Save]**.

   ![Immagine otto](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-8.png)

## Visualizzare la priorità della campagna in Marketo Classic

Per visualizzare la priorità della campagna nell’ esperienza [!DNL Classic] , fai clic sulla scheda **[!UICONTROL Schedule]** all’interno di una campagna trigger.

![Immagine nove](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-9.png)

>[!NOTE]
>
>La priorità nell’ esperienza [!DNL Classic] è solo visualizzazione. La modifica o il ripristino della priorità della campagna è disponibile solo tramite Marketo Sky.
