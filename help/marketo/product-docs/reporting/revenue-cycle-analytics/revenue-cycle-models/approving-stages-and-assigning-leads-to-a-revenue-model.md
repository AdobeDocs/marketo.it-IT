---
unique-page-id: 4718683
description: Approvazione delle fasi e assegnazione dei lead a un modello di ricavi - Documenti Marketo - Documentazione prodotto
title: Approvazione di fasi e assegnazione di lead a un modello di ricavi
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---


# Approvazione di fasi e assegnazione di lead a un modello di ricavi {#approving-stages-and-assigning-leads-to-a-revenue-model}

Avviate **Revenue** **Model** aggiungendo lead esistenti, creando regole di assegnazione per eventuali nuovi lead.

## Approvazione delle fasi {#approving-stages}

Approviamo le fasi del modello prima di aggiungere eventuali lead.

1. Andate all&#39; **area **Analytics.** **

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Selezionare il modello di cui si desidera approvare gli stadi.

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. In Azioni **** modello, selezionare **Approva** **fasi**.

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. Sarete accolti con un allarme; fate clic su **Assegna lead**.

   ![](assets/image2015-4-28-17-3a5-3a39.png)

Eccellente! Andiamo avanti e assegniamo questi lead.

## Assegnazione di lead esistenti {#assigning-existing-leads}

[Create un Smart List](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) per identificare i lead per una fase del modello nel database lead.

1. Dopo aver [creato l’Elenco](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)avanzato, fate clic sulla scheda **Lead** .

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. Fate clic su **Seleziona tutto** per selezionare i lead.

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. Aprite il menu a discesa Azioni **** lead e selezionate **Speciale**. Fare clic su **Modifica fase** ricavi.

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. Selezionare il **modello** corretto e lo **stage** corretto. Fate clic su **Esegui ora**.

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. Ripetere questa procedura finché tutti i lead non vengono assegnati alle varie fasi del modello.

Fantastico! Per specificare in che modo i nuovi lead vengono assegnati alle fasi, creare regole di assegnazione.

>[!NOTE]
>
>Se il modello è nello stato Fasi approvate, nei registri attività dei lead non verranno visualizzati eventi dell&#39;area Entrate modifiche. Se il modello è completamente approvato, questo passaggio di flusso verrà ignorato se si sposta un lead nello stesso passaggio in cui si trova attualmente.

## Nuovi lead: Crea regole di assegnazione  {#new-leads-create-assignment-rules}

1. Fai di nuovo clic su** Marketo Home**, quindi seleziona **Analytics**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. `Click your model in the tree, then the`**`Model Actions`**`menu, selecting`**`Assignment Rules`** `.`

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. `If your assignment rules contain more than just one default choice click **Stage, **make your selection, then click`**`Add Choice`**`.`

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## Regola di assegnazione esempio {#example-assignment-rule}

Create una regola Punteggio lead per assegnare i nuovi lead con un punteggio minimo a un passaggio appropriato.

1. In **Se**, selezionate Valutazione **lead**. Quindi scegliete **almeno**.
` ![](assets/image2015-4-29-13-3a27-3a8.png)

   `

1. Immettere **40** nel campo e selezionare Lead **** di vendita come fase. Fai clic su **Salva** per completare l&#39;operazione.

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!NOTE]
>
>**Articoli correlati**
>
>Per approvare il modello, consultare la nostra pagina della guida in ** [Approvazione e annullamento dell&#39;approvazione di un modello](approve-unapprove-a-revenue-model.md)di ricavi**.

