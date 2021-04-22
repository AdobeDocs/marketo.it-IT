---
unique-page-id: 6848782
description: Rendi dinamico il messaggio di annullamento dell’abbonamento per le lingue - Documenti Marketo - Documentazione del prodotto
title: Rendi il messaggio di annullamento dell’abbonamento dinamico per le lingue
exl-id: 953a7fd8-b1f2-4f3f-b889-87d1f0471e0d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# Rendi il messaggio di annullamento dell’abbonamento dinamico per le lingue {#make-your-unsubscribe-message-dynamic-for-languages}

Il messaggio e il collegamento di annullamento dell’abbonamento predefiniti sono in inglese. È possibile utilizzare il contenuto dinamico per visualizzarlo in lingue diverse.

>[!NOTE]
>
>Abbiamo impostato questo piccolo tutorial qui sotto per voi. Rappresenta una best practice, ma può essere eseguita in altri modi.

## Prepara i dati {#prepare-your-data}

1. [Crea un ](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) campo personalizzato denominato &quot;Lingua preferita&quot;. (Configuralo nel tuo CRM se desideri che questo campo si sincronizzi).

   >[!TIP]
   >
   >In futuro, utilizza questo campo quando [crei un modulo](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) per acquisire le preferenze relative alla lingua.

## Crea segmentazione {#create-segmentation}

1. Vai al **Database**.

   ![](assets/db.png)

1. Nel menu a discesa **Nuovo** , fai clic su **Nuova segmentazione**.

   ![](assets/two.png)

1. Denomina la segmentazione **Lingua preferita**. Fai clic su **Aggiungi segmento**. Digita una lingua.

   ![](assets/image2015-3-9-8-3a33-3a44.png)

   >[!NOTE]
   >
   >Il segmento predefinito è Inglese.

1. Continua ad aggiungere segmenti finché non vengono rappresentate tutte le lingue. Fare clic su **Crea**.

   ![](assets/image2015-3-9-8-3a38-3a5.png)

1. Seleziona un segmento.

   ![](assets/image2015-3-9-8-3a38-3a17.png)

1. Vai alla scheda **Smart List** . Inserisci **Lingua preferita** nel campo di ricerca. Trascina e rilascia il filtro sull’area di lavoro.

   ![](assets/six.png)

1. Impostare la lingua corrispondente appropriata.

   ![](assets/seven.png)

1. Ripeti per tutte le tue diverse lingue. Quindi, seleziona il menu a discesa **Azioni di segmentazione** e fai clic su **Approva**.

   ![](assets/image2015-3-9-8-3a39-3a36.png)

## Creare un frammento {#create-a-snippet}

1. Vai a **Design Studio**.

   ![](assets/ds.png)

1. Nel menu a discesa **Nuovo**, fai clic su **Nuovo frammento**.

   ![](assets/ten.png)

1. Denomina lo snippet **Annulla sottoscrizione messaggio**. Fare clic su **Crea**.

   ![](assets/image2015-3-9-8-3a40-3a54.png)

1. Digita il messaggio di annullamento sottoscrizione predefinito, evidenzialo e fai clic sull’icona del collegamento ipertestuale.

   ![](assets/image2015-3-9-8-3a41-3a47.png)

1. Copia e incolla questo token: `{{system.unsubscribeLink}}` nel campo **Collega URL** . Fare clic su **Inserisci**.

   ![](assets/image2015-3-9-8-3a43-3a17.png)

1. Seleziona **Segmento per** nella sezione Segmentazione .

   ![](assets/image2015-3-9-8-3a44-3a16.png)

1. Dal menu a discesa Segmentazione, digita **Preferred** e seleziona **Preferred Language**. Fare clic su **Salva**.

   ![](assets/image2015-3-9-8-3a44-3a32.png)

1. Seleziona un segmento dalla struttura. Digita il messaggio di annullamento dell’abbonamento in tale lingua.

   ![](assets/image2015-3-9-8-3a45-3a43.png)

1. Copia e incolla lo stesso token: `{{system.unsubscribeLink}}` nel campo **Collega URL** . Fare clic su **Inserisci**.

   ![](assets/image2015-3-9-8-3a47-3a4.png)

1. Ripeti per tutti i segmenti. Quindi, torna a Design Studio, fai clic sul menu a discesa **Azioni frammento** e fai clic su **Approva**.

   ![](assets/image2015-3-9-8-3a47-3a34.png)

   Fantastico. Quasi lì.

## Usa snippet in un&#39;e-mail {#use-snippet-in-an-email}

1. All’interno dell’editor e-mail, fai clic sull’elemento modificabile . Quindi fai clic sull&#39;icona a forma di ingranaggio e seleziona **Sostituisci con snippet**. Se selezioni un elemento snippet modificabile, fai clic sull&#39;icona a forma di ingranaggio e seleziona **Modifica**.

   ![](assets/4.1.png)

1. Trova e seleziona il tuo frammento dal menu a discesa e fai clic su **Salva**.

   ![](assets/image2015-3-9-8-3a50-3a16.png)

1. Per eseguire il test, fai clic su **Indietro**...

   ![](assets/4.3.png)

1. ...quindi la scheda **Dinamico**.

   ![](assets/4.4.png)

1. Fai clic sulle diverse lingue per visualizzare la modifica dello snippet.

   ![](assets/4.5.png)

   >[!TIP]
   >
   >Naturalmente, puoi modificare il resto dell’e-mail anche per la lingua dinamica. Mentre ti trovi, procedi con la stessa tecnica nella pagina di annullamento dell’abbonamento.

## Personalizzazione della pagina di annullamento dell’abbonamento con contenuto dinamico {#customizing-your-unsubscribe-page-with-dynamic-content}

Se desideri che le persone accedano a una pagina di annullamento dell’abbonamento nella lingua preferita, puoi utilizzare il contenuto dinamico nella pagina di destinazione e nella pagina di conferma.

1. Passare a Design Studio.

   ![](assets/ds.png)

1. Digita _Annulla sottoscrizione_ nel campo di ricerca. Troverai le tue pagine Annulla sottoscrizione.

   ![](assets/image2015-3-9-8-3a51-3a53.png)

1. Fare clic su **Modifica bozza**.

   ![](assets/image2015-3-9-8-3a52-3a23.png)

1. Seleziona **Segmento per**.

   ![](assets/image2015-3-9-8-3a52-3a57.png)

1. Trova il segmento Lingua preferita . Fare clic su **Salva**.

   ![](assets/image2015-3-9-8-3a53-3a54.png)

   Modifica il contenuto per ogni pagina di destinazione, approva e sei pronto a partire!

   >[!NOTE]
   >
   >Ulteriori informazioni su [contenuto dinamico](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) e su tutte le operazioni interessanti che puoi eseguire.
