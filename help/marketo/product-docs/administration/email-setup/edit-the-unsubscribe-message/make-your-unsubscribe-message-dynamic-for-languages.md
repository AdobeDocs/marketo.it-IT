---
unique-page-id: 6848782
description: Rendere dinamico il messaggio di annullamento dell’iscrizione per le lingue - Documentazione di Marketo - Documentazione del prodotto
title: Rendi dinamico il messaggio di annullamento dell’iscrizione per le lingue
exl-id: 953a7fd8-b1f2-4f3f-b889-87d1f0471e0d
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 1%

---

# Rendi dinamico il messaggio di annullamento dell’iscrizione per le lingue {#make-your-unsubscribe-message-dynamic-for-languages}

Il messaggio e il collegamento di annullamento dell’iscrizione predefiniti sono in inglese. Puoi utilizzare il contenuto dinamico per visualizzarlo in lingue diverse.

>[!NOTE]
>
>Questo articolo rappresenta una best practice, ma può essere eseguito in altri modi.

## Preparare i dati {#prepare-your-data}

1. [Crea un campo personalizzato](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) denominato &quot;Lingua preferita&quot;. (configuralo nel tuo CRM se vuoi che questo campo venga sincronizzato).

   >[!TIP]
   >
   >In futuro, utilizzare questo campo quando si [crea un modulo](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) per acquisire le preferenze della lingua.

## Crea segmentazione {#create-segmentation}

1. Vai al **[!UICONTROL database]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-1.png)

1. Nel menu a discesa **[!UICONTROL Nuovo]**, fai clic su **[!UICONTROL Nuova segmentazione]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-2.png)

1. Denomina la segmentazione **[!UICONTROL Lingua preferita]**. Fai clic su **[!UICONTROL Aggiungi segmento]**. Digita in una lingua.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-3.png)

   >[!NOTE]
   >
   >Il segmento predefinito sarà Inglese.

1. Continua ad aggiungere segmenti fino a quando non saranno rappresentate tutte le lingue. Fai clic su **[!UICONTROL Crea]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-4.png)

1. Seleziona un segmento.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-5.png)

1. Passa alla scheda **[!UICONTROL Elenco avanzato]**. Immetti **[!UICONTROL Lingua preferita]** nel campo di ricerca. Trascina e rilascia il filtro nell’area di lavoro.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-6.png)

1. Imposta la lingua corrispondente appropriata.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-7.png)

1. Ripeti per tutte le diverse lingue. Quindi, seleziona l&#39;elenco a discesa **[!UICONTROL Azioni di segmentazione]** e fai clic su **[!UICONTROL Approva]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-8.png)

## Creare uno snippet {#create-a-snippet}

1. Passare a **[!UICONTROL Design Studio]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-9.png)

1. Nel menu a discesa **[!UICONTROL Nuovo]**, fai clic su **[!UICONTROL Nuovo snippet]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-10.png)

1. Denomina il frammento **Messaggio di annullamento sottoscrizione**. Fai clic su **[!UICONTROL Crea]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-11.png)

1. Digita il messaggio predefinito di annullamento dell’iscrizione, evidenzialo e fai clic sull’icona del collegamento ipertestuale.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-12.png)

1. Copia e incolla questo token: `{{system.unsubscribeLink}}` nel campo **[!UICONTROL URL]**. Fare clic su **[!UICONTROL Inserisci]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-13.png)

1. Seleziona **[!UICONTROL Segmento di]** nella sezione **[!UICONTROL Segmentazione]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-14.png)

1. Dal menu a discesa **[!UICONTROL Segmentazione]**, digita in **[!UICONTROL Preferred]** e seleziona **[!UICONTROL Preferred Language]**. Fai clic su **[!UICONTROL Salva]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-15.png)

1. Seleziona un segmento dalla struttura. Fai clic sull’icona di annullamento dell’abbonamento e quindi sull’icona del collegamento.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-16.png)

1. Assicurarsi che `{{system.unsubscribeLink}}` sia ancora nel campo **[!UICONTROL URL]**. Modifica il **[!UICONTROL Testo visualizzato]** in base alla lingua selezionata. Fare clic su **[!UICONTROL Applica]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-17.png)

1. Ripeti per tutti i segmenti. Quindi, torna a **[!UICONTROL Design Studio]**, fai clic sul menu a discesa **[!UICONTROL Azioni snippet]** e fai clic su **[!UICONTROL Approva]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-18.png)

Fantastico. Ci siamo quasi!

## Utilizzare lo snippet in un messaggio e-mail {#use-snippet-in-an-email}

1. Nell’editor e-mail, fai clic sull’elemento modificabile. Fare quindi clic sull&#39;icona a forma di ingranaggio e selezionare **[!UICONTROL Sostituisci con snippet]**. Se selezioni un elemento snippet modificabile, fai clic sull&#39;icona a forma di ingranaggio e seleziona **[!UICONTROL Modifica]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-19.png)

1. Trova e seleziona il tuo frammento di codice dall&#39;elenco a discesa, quindi fai clic su **[!UICONTROL Salva]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-20.png)

1. Per eseguire il test, fare clic su **[!UICONTROL Indietro]**...

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-21.png)

1. ...quindi la scheda **[!UICONTROL Dynamic]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-22.png)

1. Fare clic sulle diverse lingue per visualizzare la modifica dello snippet.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-23.png)

   >[!TIP]
   >
   >Naturalmente, puoi modificare anche il resto dell’e-mail per il linguaggio dinamico. Mentre lo fai, utilizza la stessa tecnica nella pagina per annullare l’abbonamento.

## Personalizzazione della pagina per annullare l’iscrizione con contenuti dinamici {#customizing-your-unsubscribe-page-with-dynamic-content}

Se desideri che le persone visitino una pagina per l’annullamento dell’abbonamento nella lingua preferita, puoi utilizzare il contenuto dinamico nelle pagine di destinazione e di conferma.

1. Passare a **[!UICONTROL Design Studio]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-24.png)

1. Digitare _Annulla sottoscrizione_ nel campo di ricerca e selezionare la pagina di annullamento dell&#39;iscrizione desiderata.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-25.png)

1. Fare clic su **[!UICONTROL Modifica bozza]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-26.png)

1. Seleziona **[!UICONTROL Segmento Per]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-27.png)

1. Trova il segmento **[!UICONTROL Lingua preferita]**. Fai clic su **[!UICONTROL Salva]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-28.png)

   Modifica il contenuto per ogni pagina di destinazione, approva e non è necessario ripetere questa operazione.

   >[!NOTE]
   >
   >Ulteriori informazioni su [contenuti dinamici](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) e su tutte le operazioni più interessanti.
