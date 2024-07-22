---
unique-page-id: 4718683
description: Approvazione degli stadi e assegnazione di lead a un modello di ricavi - Documenti Marketo - Documentazione del prodotto
title: Approvazione di fasi e assegnazione di lead a un modello di ricavi
exl-id: 0c93dfe4-8950-444c-a65b-080620816ba2
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 0%

---

# Approvazione di fasi e assegnazione di lead a un modello di ricavi {#approving-stages-and-assigning-leads-to-a-revenue-model}

Rendi operativo il **modello di ricavi** aggiungendo lead esistenti e creando regole di assegnazione per eventuali nuovi lead.

## Fasi di approvazione {#approving-stages}

Approviamo le fasi del modello prima di aggiungere qualsiasi lead.

1. Vai all&#39;area **Analytics**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Seleziona il modello di cui desideri approvare gli stadi.

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. In **Azioni modello**, selezionare **Approva fasi**.

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. Riceverai un avviso; fai clic su **Assegna lead**.

   ![](assets/image2015-4-28-17-3a5-3a39.png)

Eccellente! Passiamo all&#39;assegnazione dei lead.

## Assegnazione di lead esistenti {#assigning-existing-leads}

[Crea un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) per identificare i lead per una fase del modello nel database dei lead.

1. Dopo aver [creato l&#39;elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md), fare clic sulla scheda **Lead**.

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. Fare clic su **Seleziona tutto** per selezionare i lead.

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. Apri il menu a discesa **Azioni lead** e seleziona **Speciale**. Fare clic su **Modifica fase ricavi**.

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. Selezionare il **Modello** corretto e il **Stadio** corretto. Fare clic su **Esegui ora**.

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. Ripetere l&#39;operazione finché tutti i lead non vengono assegnati alle varie fasi del modello.

Fantastico! Per specificare la modalità di assegnazione dei nuovi lead alle fasi, creare le regole di assegnazione.

>[!NOTE]
>
>Se il modello è nello stato Fasi approvate, non verranno visualizzati eventi di fase Modifica ricavi nei registri attività dei lead. Se il modello è stato approvato completamente, questo passaggio di flusso viene ignorato se si sposta un lead nella stessa fase in cui si trova attualmente.

## Nuovi lead: crea regole di assegnazione  {#new-leads-create-assignment-rules}

1. Fai di nuovo clic su **Home di Marketo**, quindi seleziona **Analytics**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Fai clic sul modello nell&#39;albero, quindi sul menu **Azioni modello**, selezionando **Regole di assegnazione**.

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. Se le regole di assegnazione contengono più di una scelta predefinita, fare clic su **Fase**, selezionare, quindi fare clic su **Aggiungi scelta**.

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## Esempio di regola di assegnazione {#example-assignment-rule}

Crea una regola Punteggio lead per assegnare i nuovi lead con un punteggio minimo a un passaggio appropriato.

1. In **If**, selezionare **Punteggio lead**. Quindi scegli **almeno**.

   ![](assets/image2015-4-29-13-3a27-3a8.png)

1. Immetti **40** nel campo e seleziona **Lead vendite** come fase. Fai clic su **Salva** per completare l&#39;operazione.

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!MORELIKETHIS]
>
>Per approvare il tuo modello, leggi la pagina della guida in **[Approvazione e annullamento dell&#39;approvazione di un modello di ricavi](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/approve-unapprove-a-revenue-model.md)**.
