---
unique-page-id: 6848782
description: Rendi il tuo messaggio di annullamento della sottoscrizione dinamico per le lingue - Documenti Marketo - Documentazione prodotto
title: Rendi il tuo messaggio di annullamento della sottoscrizione dinamico per le lingue
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---


# Rendi il tuo messaggio di annullamento della sottoscrizione dinamico per le lingue {#make-your-unsubscribe-message-dynamic-for-languages}

>[!NOTE]
>
>**FYI**
>
>Marketo sta standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che nell&#39;abbonamento siano presenti lead/lead e persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

Il messaggio e il collegamento di annullamento della sottoscrizione predefiniti sono in inglese. Potete utilizzare il contenuto dinamico per visualizzarlo in lingue diverse.

>[!NOTE]
>
>Abbiamo preparato questa piccola esercitazione qui sotto per voi. Rappresenta una procedura ottimale, ma può essere eseguita in altri modi.

1. Preparare i dati
1. [Create un](../../../../product-docs/administration/field-management/create-a-custom-field-in-marketo.md)campo personalizzato denominato &quot;Lingua preferita&quot;. (Configuratelo in CRM se desiderate che questo campo sia sincronizzato).

   >[!TIP]
   >
   >In futuro, utilizzare questo campo quando si [crea un modulo](../../../../product-docs/demand-generation/forms/creating-a-form/create-a-form.md) per acquisire le preferenze della lingua.

1. Crea segmentazione
1. Vai al **database**.
** ![](assets/db.png)

   **

1. Nel menu a discesa **Nuovo** , fai clic su **Nuova segmentazione**.

   ![](assets/two.png)

1. Denominate la segmentazione **Preferred Language (Lingua** preferita). Fate clic su **Aggiungi segmento**. Digita una lingua.

   ![](assets/image2015-3-9-8-3a33-3a44.png)

   >[!NOTE]
   >
   >Il segmento predefinito è Inglese.

1. Continua ad aggiungere segmenti fino a quando tutte le tue lingue non saranno rappresentate. Fate clic su **Crea**.

   ![](assets/image2015-3-9-8-3a38-3a5.png)

1. Selezionare un segmento.

   ![](assets/image2015-3-9-8-3a38-3a17.png)

1. Passate alla scheda Elenco **** avanzato. Immettere **Preferred Language** nel campo di ricerca. Trascinate e rilasciate il filtro sul quadro.

   ![](assets/six.png)

1. Impostare la lingua corrispondente appropriata.

   ![](assets/seven.png)

1. Ripetere questa operazione per tutte le lingue. Quindi, seleziona il menu a discesa Azioni **di** segmentazione e fai clic su **Approva**.

   ![](assets/image2015-3-9-8-3a39-3a36.png)

1. Creare uno snippet
1. Andate a **Design Studio**.

   ![](assets/ds.png)

1. Nel menu a discesa **Nuovo** , fate clic su **Nuovo snippet**.

   ** ![](assets/ten.png)

   **

1. Denominate lo snippet **Cancella sottoscrizione**. Fate clic su **Crea**.

   ![](assets/image2015-3-9-8-3a40-3a54.png)

1. Digitate il messaggio predefinito per l’annullamento della sottoscrizione, evidenziatelo e fate clic sull’icona del collegamento ipertestuale.

   ![](assets/image2015-3-9-8-3a41-3a47.png)

1. Copiate e incollate questo token: **`{{system.unsubscribeLink}}`** nel campo URL **** collegamento. Fate clic su **Inserisci**.

   ![](assets/image2015-3-9-8-3a43-3a17.png)

1. Selezionare **Segmento per** nella sezione Segmentazione.

   ![](assets/image2015-3-9-8-3a44-3a16.png)

1. Dal menu a discesa Segmentazione, digitate **Preferred (Preferito** ) e selezionate **Preferred Language (Lingua** preferita). Fate clic su **Salva**.

   ![](assets/image2015-3-9-8-3a44-3a32.png)

1. Selezionare un segmento dalla struttura ad albero. Digitate il messaggio di annullamento dell’iscrizione in tale lingua.

   ![](assets/image2015-3-9-8-3a45-3a43.png)

1. Copiate e incollate lo stesso token: **`{{system.unsubscribeLink}}`** nel campo URL **** collegamento. Fate clic su **Inserisci**.

   ![](assets/image2015-3-9-8-3a47-3a4.png)

1. Ripetete la procedura per tutti i segmenti. Quindi, tornate a Design Studio, fate clic sul menu a discesa Azioni **frammento e fate clic su** Approva ****.

   ![](assets/image2015-3-9-8-3a47-3a34.png)

   Fantastico. Quasi lì.

1. Utilizzare lo snippet in un messaggio e-mail
1. All’interno dell’editor e-mail, fate clic sull’elemento modificabile. Fate clic sull’icona a forma di ingranaggio e selezionate **Sostituisci con snippet**. Se selezionate un elemento snippet modificabile, fate clic sull’icona a forma di ingranaggio e selezionate **Modifica**.

   ![](assets/4.1.png)

1. Trova e seleziona lo snippet dal menu a discesa e fai clic su **Salva**.

   ![](assets/image2015-3-9-8-3a50-3a16.png)

1. Per eseguire il test out, fare clic su **Indietro**...

   ![](assets/4.3.png)

1. ...quindi la scheda **Dinamico** .

   ![](assets/4.4.png)

1. Fate clic sulle diverse lingue per visualizzare la modifica dello snippet.

   ![](assets/4.5.png)

   >[!TIP]
   >
   >Ovviamente, puoi modificare anche il resto dell&#39;e-mail per la lingua dinamica. Anche se vi trovate, effettuate la stessa tecnica nella pagina di annullamento della sottoscrizione.

1. Personalizzazione della pagina di annullamento della sottoscrizione con contenuti dinamici

   Se desiderate che le persone arrivino a una pagina di annullamento della sottoscrizione nella lingua desiderata, potete utilizzare il contenuto dinamico nella pagina di destinazione e nella pagina di conferma.

   Passare a Design Studio.

   ![](assets/ds.png)

   Digitate Annulla sottoscrizione nel campo di ricerca. Dovresti trovare le tue pagine di annullamento della sottoscrizione.

   ![](assets/image2015-3-9-8-3a51-3a53.png)

   Fate clic su Modifica bozza.

   ![](assets/image2015-3-9-8-3a52-3a23.png)

   Seleziona Segmento per.

   ![](assets/image2015-3-9-8-3a52-3a57.png)

   Trova il segmento Lingua preferita. Fate clic su Salva.

   ![](assets/image2015-3-9-8-3a53-3a54.png)

   Modifica il contenuto per ogni pagina di destinazione, approva e sei pronto!

   >[!NOTE]
   >
   >**Tubo profondo**
   >
   >
   >Scopri di più sul contenuto [](../../../../product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) dinamico e su tutte le attività interessanti che puoi realizzare.

