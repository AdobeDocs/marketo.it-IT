---
unique-page-id: 6848782
description: Rendi dinamico il messaggio di annullamento dell’abbonamento per le lingue - Documenti Marketo - Documentazione del prodotto
title: Rendi il messaggio di annullamento dell’abbonamento dinamico per le lingue
exl-id: 953a7fd8-b1f2-4f3f-b889-87d1f0471e0d
source-git-commit: aeaf1f55b81da70ac8415cab265165a3848b5a0e
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 1%

---

# Rendi il messaggio di annullamento dell’abbonamento dinamico per le lingue {#make-your-unsubscribe-message-dynamic-for-languages}

Il messaggio e il collegamento di annullamento dell’abbonamento predefiniti sono in inglese. È possibile utilizzare il contenuto dinamico per visualizzarlo in lingue diverse.

>[!NOTE]
>
>Questo articolo rappresenta una best practice, ma può essere eseguito in altri modi.

## Preparare i dati {#prepare-your-data}

1. [Creazione di un campo personalizzato](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) denominato &quot;Lingua preferita&quot;. (Configuralo nel tuo CRM se desideri che questo campo si sincronizzi).

   >[!TIP]
   >
   >In futuro, utilizza questo campo quando [creare un modulo](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) per acquisire le preferenze relative alla lingua.

## Creare segmentazione {#create-segmentation}

1. Vai a **Database**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-1.png)

1. In **Nuovo** a discesa, fai clic su **Nuova segmentazione**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-2.png)

1. Denomina la segmentazione **Lingua preferita**. Fai clic su **Aggiungi segmento**. Digita una lingua.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-3.png)

   >[!NOTE]
   >
   >Il segmento predefinito è Inglese.

1. Continua ad aggiungere segmenti finché non vengono rappresentate tutte le lingue. Fai clic su **Crea**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-4.png)

1. Seleziona un segmento.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-5.png)

1. Vai a **Elenco avanzato** scheda . Invio **Lingua preferita** nel campo di ricerca. Trascina e rilascia il filtro sull’area di lavoro.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-6.png)

1. Impostare la lingua corrispondente appropriata.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-7.png)

1. Ripeti per tutte le tue diverse lingue. Quindi, seleziona la **Azioni di segmentazione** a discesa e fai clic su **Approva**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-8.png)

## Creare un frammento {#create-a-snippet}

1. Vai a **Design Studio**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-9.png)

1. In **Nuovo** a discesa, fai clic su **Nuovo frammento**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-10.png)

1. Denomina lo snippet **Annulla sottoscrizione messaggio**. Fai clic su **Crea**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-11.png)

1. Digita il messaggio di annullamento sottoscrizione predefinito, evidenzialo e fai clic sull’icona del collegamento ipertestuale.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-12.png)

1. Copia e incolla questo token: `{{system.unsubscribeLink}}` nel **URL** campo . Fai clic su **Inserisci**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-13.png)

1. Seleziona **Segmento per** nella sezione Segmentazione .

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-14.png)

1. Dall’elenco a discesa Segmentazione , digita in **Preferito** e seleziona **Lingua preferita**. Fai clic su **Salva**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-15.png)

1. Seleziona un segmento dalla struttura. Fai clic sull’iscrizione e quindi sull’icona del collegamento.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-16.png)

1. Assicurati `{{system.unsubscribeLink}}` si trova ancora nel campo URL. Modificare il testo visualizzato in modo che corrisponda alla lingua selezionata. Fai clic su **Applica**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-17.png)

1. Ripeti per tutti i segmenti. Quindi, torna a Design Studio e fai clic sul pulsante **Azioni frammento** a discesa e fai clic su **Approva**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-18.png)

Fantastico. Quasi lì!

## Utilizzare un frammento in un messaggio e-mail {#use-snippet-in-an-email}

1. All’interno dell’editor e-mail, fai clic sull’elemento modificabile . Quindi fai clic sull’icona a forma di ingranaggio e seleziona **Sostituisci con frammento**. Se selezioni un elemento snippet modificabile, fai clic sull’icona a forma di ingranaggio e seleziona **Modifica**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-19.png)

1. Trova e seleziona lo snippet dal menu a discesa e fai clic su **Salva**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-20.png)

1. Per eseguire il test, fai clic su **Indietro**...

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-21.png)

1. ...quindi il **Dinamico** scheda .

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-22.png)

1. Fai clic sulle diverse lingue per visualizzare la modifica dello snippet.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-23.png)

   >[!TIP]
   >
   >Naturalmente, puoi modificare il resto dell’e-mail anche per la lingua dinamica. Mentre ti trovi, procedi con la stessa tecnica nella pagina di annullamento dell’abbonamento.

## Personalizzazione della pagina di annullamento dell’abbonamento con contenuto dinamico {#customizing-your-unsubscribe-page-with-dynamic-content}

Se desideri che le persone accedano a una pagina di annullamento dell’abbonamento nella lingua preferita, puoi utilizzare il contenuto dinamico nella pagina di destinazione e nella pagina di conferma.

1. Passa a **Design Studio**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-24.png)

1. Digitare in _Annulla sottoscrizione_ nel campo di ricerca e seleziona la pagina Annulla sottoscrizione desiderata.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-25.png)

1. Fai clic su **Modifica bozza**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-26.png)

1. Seleziona **Segmento per**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-27.png)

1. Trova il segmento Lingua preferita . Fai clic su **Salva**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-28.png)

   Modifica il contenuto per ogni pagina di destinazione, approva e sei pronto a partire!

   >[!NOTE]
   >
   >Ulteriori informazioni [contenuto dinamico](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) e tutta la roba fantastica che potete fare.
