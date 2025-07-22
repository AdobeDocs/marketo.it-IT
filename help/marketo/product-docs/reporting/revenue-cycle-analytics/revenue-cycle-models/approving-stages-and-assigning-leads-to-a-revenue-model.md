---
unique-page-id: 4718683
description: Approvazione degli stadi e assegnazione di lead a un modello di ricavi - Documenti Marketo - Documentazione del prodotto
title: Approvazione di fasi e assegnazione di lead a un modello di ricavi
exl-id: 0c93dfe4-8950-444c-a65b-080620816ba2
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---

# Approvazione di fasi e assegnazione di lead a un modello di ricavi {#approving-stages-and-assigning-leads-to-a-revenue-model}

Rendi operativo il **modello di ricavi** aggiungendo lead esistenti e creando regole di assegnazione per eventuali nuovi lead.

## Fasi di approvazione {#approving-stages}

Approviamo le fasi del modello prima di aggiungere qualsiasi lead.

1. Passare all&#39;area **[!UICONTROL Analytics]**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Seleziona il modello di cui desideri approvare gli stadi.

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. In **[!UICONTROL Model Actions]**, selezionare **[!UICONTROL Approve Stages]**.

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. Verrà visualizzato un avviso. Fare clic su **[!UICONTROL Assign Leads]**.

   ![](assets/image2015-4-28-17-3a5-3a39.png)

Eccellente! Passiamo all&#39;assegnazione dei lead.

## Assegnazione di lead esistenti {#assigning-existing-leads}

[Crea un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) per identificare i lead per una fase del modello nel database dei lead.

1. Dopo aver [creato l&#39;elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md), fare clic sulla scheda **[!UICONTROL Leads]**.

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. Fare clic su **[!UICONTROL Select All]** per selezionare i lead.

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. Aprire il menu a discesa **[!UICONTROL Lead Actions]** e selezionare **[!UICONTROL Special]**. Fai clic su **[!UICONTROL Change Revenue Stage...]**.

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. Selezionare il **[!UICONTROL Model]** corretto e il **[!UICONTROL Stage]** corretto. Fai clic su **[!UICONTROL Run Now]**.

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. Ripetere l&#39;operazione finché tutti i lead non vengono assegnati alle varie fasi del modello.

Fantastico! Per specificare la modalità di assegnazione dei nuovi lead alle fasi, creare le regole di assegnazione.

>[!NOTE]
>
>Se il modello è nello stato Fasi approvate, non verranno visualizzati eventi di fase Modifica ricavi nei registri attività dei lead. Se il modello è stato approvato completamente, questo passaggio di flusso viene ignorato se si sposta un lead nella stessa fase in cui si trova attualmente.

## Nuovi lead: crea regole di assegnazione  {#new-leads-create-assignment-rules}

1. Fai di nuovo clic su **Home di Marketo**, quindi seleziona **[!UICONTROL Analytics]**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Fare clic sul modello nell&#39;albero, quindi sul menu **[!UICONTROL Model Actions]**, selezionando **[!UICONTROL Assignment Rules]**.

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. Se le regole di assegnazione contengono più di una scelta predefinita, fare clic su **[!UICONTROL Stage]**, effettuare la selezione, quindi fare clic su **[!UICONTROL Add Choice]**.

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## Esempio di regola di assegnazione {#example-assignment-rule}

Creare una regola [!UICONTROL Lead Score] per assegnare i nuovi lead con un punteggio minimo al passaggio appropriato.

1. In **[!UICONTROL If]**, selezionare **[!UICONTROL Lead Score]**. Quindi scegliere **[!UICONTROL at least]**.

   ![](assets/image2015-4-29-13-3a27-3a8.png)

1. Immetti **40** nel campo e seleziona **[!UICONTROL Sales Lead]** come [!UICONTROL Stage]. Fare clic su **[!UICONTROL Save]** per completare.

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!MORELIKETHIS]
>
>Per approvare il tuo modello, leggi la pagina della guida in **[Approvazione e annullamento dell&#39;approvazione di un modello di ricavi](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/approve-unapprove-a-revenue-model.md)**.
