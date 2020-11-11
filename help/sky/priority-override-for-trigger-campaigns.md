---
title: priorità-override-per-trigger-campaign
description: Override di priorità per le campagne di attivazione
translation-type: tm+mt
source-git-commit: 642fd57105afff1031f18883c5809206f136b7c6
workflow-type: tm+mt
source-wordcount: '320'
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

1. Nella campagna di attivazione, fare clic sulla scheda [!UICONTROL **Pianificazione**] , quindi su [!UICONTROL **Ignora priorità**].

   ![Immagine uno](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-1.png)

1. Scegliete un nuovo livello di priorità dal menu a discesa. Fate clic su [!UICONTROL **Conferma**].

   ![Immagine due](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-2.png)

   ![Immagine tre](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-3.png)

>[!NOTE]
>
>* Potete visualizzare la priorità predefinita della campagna nella [!UICONTROL Campaign Queue] sezione [!UICONTROL Marketing Activities]. Per aumentare il tasso di esecuzione, si consiglia di impostare la priorità della campagna su un livello superiore a quello predefinito.
>* La priorità definita dall&#39;utente si applica solo alle nuove persone idonee alla campagna; le persone che sono già in coda non ne verranno interessate.


## Ripristina priorità

1. Per ripristinare la priorità della campagna all&#39;impostazione predefinita del sistema, andate alla scheda [!UICONTROL **Pianificazione**] nella campagna di attivazione e fate clic su [!UICONTROL **Ripristina priorità**].

   ![Immagine quattro](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-4.png)

1. Fate clic su [!UICONTROL **Ripristina**] per confermare.

   ![Immagine cinque](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-5.png)

>[!NOTE]
>
>Le sostituzioni e i ripristini con priorità vengono acquisiti nella traccia di audit. Potete visualizzare la traccia di [controllo](https://docs.marketo.com/x/GZ2t) nell&#39;area [!UICONTROL Admin] dell&#39;esperienza classica.

## Accesso all&#39;override della priorità di sovvenzione

>[!CAUTION]
>
>Solo gli amministratori o gli utenti con responsabilità di amministratore devono avere la priorità della campagna come accesso alternativo.

1. Nell&#39; [!UICONTROL Admin] area fare clic su [!UICONTROL **Utenti e ruoli**].

   ![Immagine Sei](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-6.png)

1. Fare clic sulla scheda [!UICONTROL **Ruoli**] , selezionare l&#39;utente a cui si desidera concedere l&#39;accesso, quindi fare clic su [!UICONTROL **Modifica ruolo**].

   ![Immagine sette](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-7.png)

1. In [!UICONTROL Access Marketing Activities], seleziona [!UICONTROL **Modifica priorità**] campagna attivatore. Fate clic su [!UICONTROL **Salva**].

   ![Immagine otto](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-8.png)

## Visualizza priorità campagna in Marketo Classic

Per visualizzare la priorità della campagna nell&#39; [!DNL Classic] esperienza, fai clic sulla scheda [!UICONTROL **Pianificazione**] all&#39;interno di una campagna di attivazione.

![Image Nine](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-9.png)

>[!NOTE]
>
>La priorità nell&#39; [!DNL Classic] esperienza è di sola visualizzazione. La modifica o il ripristino della priorità della campagna è disponibile solo tramite Marketo Sky.
