---
unique-page-id: 6848782
description: Rendi il tuo messaggio di annullamento della sottoscrizione dinamico per le lingue - Documenti Marketo - Documentazione prodotto
title: Rendi il tuo messaggio di annullamento della sottoscrizione dinamico per le lingue
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---


# Rendi il tuo messaggio di annullamento della sottoscrizione dinamico per le lingue {#make-your-unsubscribe-message-dynamic-for-languages}

Il messaggio e il collegamento di annullamento della sottoscrizione predefiniti sono in inglese. Potete utilizzare il contenuto dinamico per visualizzarlo in lingue diverse.

>[!NOTE]
>
>Abbiamo preparato questa piccola esercitazione qui sotto per voi. Rappresenta una procedura ottimale, ma può essere eseguita in altri modi.

## Preparare i dati {#prepare-your-data}

1. [Create un ](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) campo personalizzato denominato &quot;Lingua preferita&quot;. (Configuratelo in CRM se desiderate che questo campo sia sincronizzato).

   >[!TIP]
   >
   >In futuro, utilizzare questo campo quando si [crea un modulo](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) per acquisire le preferenze per la lingua.

## Crea segmentazione {#create-segmentation}

1. Accedere al **Database**.

   ![](assets/db.png)

1. Nel menu a discesa **New**, fare clic su **New Segmentation** (Nuova segmentazione).

   ![](assets/two.png)

1. Denominate la segmentazione **Lingua preferita**. Fare clic su **Aggiungi segmento**. Digita una lingua.

   ![](assets/image2015-3-9-8-3a33-3a44.png)

   >[!NOTE]
   >
   >Il segmento predefinito è Inglese.

1. Continua ad aggiungere segmenti fino a quando tutte le tue lingue non saranno rappresentate. Fare clic su **Crea**.

   ![](assets/image2015-3-9-8-3a38-3a5.png)

1. Selezionare un segmento.

   ![](assets/image2015-3-9-8-3a38-3a17.png)

1. Passate alla scheda **Smart List**. Immettere **Lingua preferita** nel campo di ricerca. Trascinate e rilasciate il filtro sul quadro.

   ![](assets/six.png)

1. Impostare la lingua corrispondente appropriata.

   ![](assets/seven.png)

1. Ripetere questa operazione per tutte le lingue. Quindi, selezionate il menu a discesa **Azioni segmentazione** e fate clic su **Approva**.

   ![](assets/image2015-3-9-8-3a39-3a36.png)

## Creare uno snippet {#create-a-snippet}

1. Andate a **Design Studio**.

   ![](assets/ds.png)

1. Nel menu a discesa **New**, fare clic su **New Snippet**.

   ![](assets/ten.png)

1. Denominate lo snippet **Annulla sottoscrizione a messaggio**. Fare clic su **Crea**.

   ![](assets/image2015-3-9-8-3a40-3a54.png)

1. Digitate il messaggio predefinito per l’annullamento della sottoscrizione, evidenziatelo e fate clic sull’icona del collegamento ipertestuale.

   ![](assets/image2015-3-9-8-3a41-3a47.png)

1. Copiate e incollate questo token: `{{system.unsubscribeLink}}` nel campo **Collega URL**. Fare clic su **Inserisci**.

   ![](assets/image2015-3-9-8-3a43-3a17.png)

1. Selezionare **Segment By** nella sezione Segmentazione.

   ![](assets/image2015-3-9-8-3a44-3a16.png)

1. Dal menu a discesa Segmentazione, digitare **Preferred** e selezionare **Preferred Language**. Fare clic su **Salva**.

   ![](assets/image2015-3-9-8-3a44-3a32.png)

1. Selezionare un segmento dalla struttura ad albero. Digitate il messaggio di annullamento dell’iscrizione in tale lingua.

   ![](assets/image2015-3-9-8-3a45-3a43.png)

1. Copiate e incollate lo stesso token: `{{system.unsubscribeLink}}` nel campo **Collega URL**. Fare clic su **Inserisci**.

   ![](assets/image2015-3-9-8-3a47-3a4.png)

1. Ripetete la procedura per tutti i segmenti. Quindi, tornare a Design Studio, fare clic sul menu a discesa **Azioni snippet**, quindi fare clic su **Approva**.

   ![](assets/image2015-3-9-8-3a47-3a34.png)

   Fantastico. Quasi lì.

## Utilizza snippet in un&#39;e-mail {#use-snippet-in-an-email}

1. All’interno dell’editor e-mail, fate clic sull’elemento modificabile. Fate clic sull&#39;icona dell&#39;ingranaggio e selezionate **Sostituisci con snippet**. Se state selezionando un elemento snippet modificabile, fate clic sull&#39;icona a forma di ingranaggio e selezionate **Edit**.

   ![](assets/4.1.png)

1. Trova e seleziona il frammento dal menu a discesa e fai clic su **Salva**.

   ![](assets/image2015-3-9-8-3a50-3a16.png)

1. Per eseguire il test out, fare clic su **Indietro**...

   ![](assets/4.3.png)

1. ...quindi la scheda **Dynamic**.

   ![](assets/4.4.png)

1. Fate clic sulle diverse lingue per visualizzare la modifica dello snippet.

   ![](assets/4.5.png)

   >[!TIP]
   >
   >Ovviamente, puoi modificare anche il resto dell&#39;e-mail per la lingua dinamica. Anche se vi trovate, effettuate la stessa tecnica nella pagina di annullamento della sottoscrizione.

## Personalizzazione della pagina di annullamento della sottoscrizione con contenuto dinamico {#customizing-your-unsubscribe-page-with-dynamic-content}

Se desiderate che le persone arrivino a una pagina di annullamento della sottoscrizione nella lingua desiderata, potete utilizzare il contenuto dinamico nella pagina di destinazione e nella pagina di conferma.

1. Passare a Design Studio.

   ![](assets/ds.png)

1. Digitate _Annulla sottoscrizione_ nel campo di ricerca. Dovresti trovare le tue pagine di annullamento della sottoscrizione.

   ![](assets/image2015-3-9-8-3a51-3a53.png)

1. Fare clic su **Modifica bozza**.

   ![](assets/image2015-3-9-8-3a52-3a23.png)

1. Selezionare **Segmento per**.

   ![](assets/image2015-3-9-8-3a52-3a57.png)

1. Trova il segmento Lingua preferita. Fare clic su **Salva**.

   ![](assets/image2015-3-9-8-3a53-3a54.png)

   Modifica il contenuto per ogni pagina di destinazione, approva e sei pronto!

   >[!NOTE]
   >
   >Scopri di più su [contenuti dinamici](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) e su tutte le cose interessanti che puoi fare.
