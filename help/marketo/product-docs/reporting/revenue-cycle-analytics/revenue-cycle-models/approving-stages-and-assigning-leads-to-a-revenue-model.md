---
unique-page-id: 4718683
description: Approvazione delle fasi e assegnazione dei lead a un modello di ricavi - Documenti Marketo - Documentazione del prodotto
title: Approvazione delle fasi e assegnazione dei lead a un modello di ricavi
exl-id: 0c93dfe4-8950-444c-a65b-080620816ba2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Approvazione delle fasi e assegnazione dei lead a un modello di ricavi {#approving-stages-and-assigning-leads-to-a-revenue-model}

Ottieni il tuo **Modello dei ricavi** è possibile aggiungere lead esistenti e creare regole di assegnazione per eventuali nuovi lead.

## Approvazione delle fasi {#approving-stages}

Approviamo le fasi del modello prima di aggiungere eventuali lead.

1. Vai a **Analytics** area.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Selezionare il modello di cui si desidera approvare gli stadi.

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. Sotto **Azioni modello**, seleziona **Approva fasi**.

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. Sarai accolto con un avviso; click **Assegna lead**.

   ![](assets/image2015-4-28-17-3a5-3a39.png)

Eccellente! Andiamo avanti e assegniamo questi lead.

## Assegnazione di lead esistenti {#assigning-existing-leads}

[Creare un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) per identificare i lead per una fase del modello nel database lead.

1. Una volta [creato il tuo Smart List](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md), fai clic su **Lead** scheda .

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. Fai clic su **Seleziona tutto** per selezionare i lead.

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. Apri **Azioni lead** a discesa e seleziona **Speciale**. Fai clic su **Cambia fase ricavi**.

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. Selezionare la risposta corretta **Modello** e la **Stage**. Fai clic su **Esegui ora**.

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. Ripetete questa operazione fino a quando tutti i lead non vengono assegnati alle varie fasi del modello.

Fantastico! Per specificare la modalità di assegnazione dei nuovi lead alle fasi, creare regole di assegnazione.

>[!NOTE]
>
>Se il modello si trova nello stato Stadi approvati, nei registri attività dei lead non verranno visualizzati eventi della fase di modifica dei ricavi. Se il modello è completamente approvato, questo passaggio di flusso verrà ignorato se si sposta un lead nello stesso stadio in cui si trova attualmente.

## Nuovi lead: Crea regole di assegnazione  {#new-leads-create-assignment-rules}

1. Fai clic su **Pagina principale di Marketo** di nuovo, seleziona **Analytics**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Fai clic sul modello nell&#39;albero, quindi sul **Azioni modello** menu, selezione **Regole di assegnazione**.

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. Se le regole di assegnazione contengono più di una scelta predefinita, fai clic su **Stage**, effettua la selezione, quindi fai clic su **Aggiungi scelta**.

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## Esempio di regola di assegnazione {#example-assignment-rule}

Crea una regola Punteggio lead per assegnare i nuovi lead con un punteggio minimo a un passaggio appropriato.

1. Sotto **Se**, seleziona **Punteggio lead**. Quindi scegli **almeno**.

   ![](assets/image2015-4-29-13-3a27-3a8.png)

1. Invio **40** nel campo e seleziona **Lead di vendita** come stage. Fai clic su **Salva** da completare.

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!MORELIKETHIS]
>
>Per approvare il modello, consulta la nostra pagina di aiuto in **[Approvazione e annullamento dell’approvazione di un modello di ricavi](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/approve-unapprove-a-revenue-model.md)**.
