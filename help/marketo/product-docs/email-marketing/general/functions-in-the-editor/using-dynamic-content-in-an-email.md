---
unique-page-id: 2950617
description: Utilizzo di contenuti dinamici in un’e-mail - Documenti Marketo - Documentazione del prodotto
title: Utilizzo di contenuti dinamici in un’e-mail
exl-id: a1178f76-6760-4a4a-9510-f129ee6a9032
source-git-commit: 076d781fc8d967ee6f63ed2023e75c94e5aa1e55
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Utilizzo di contenuti dinamici in un’e-mail {#using-dynamic-content-in-an-email}

>[!PREREQUISITES]
>
>[Creare una segmentazione](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

Utilizza il contenuto dinamico nelle e-mail per inviare ai lead informazioni mirate.

>[!NOTE]
>
>L’utilizzo di variabili all’interno del contenuto dinamico in un messaggio e-mail è supportato solo quando si utilizzano le campagne trigger. È **not** supportato quando si utilizzano campagne batch.

## Aggiungi segmentazione {#add-segmentation}

1. Vai a **Attività di marketing**.

   ![](assets/login-marketing-activities.png)

1. Seleziona l’e-mail e fai clic su **Modifica bozza**.

   ![](assets/1.2.png)

1. In questo esempio stiamo rendendo dinamica la Linea oggetto. Fai clic nel campo Oggetto , quindi fai clic sul pulsante **Rendi dinamico** pulsante .

   ![](assets/1.3.png)

   >[!NOTE]
   >
   >Puoi anche creare un elemento all’interno dell’e-mail dinamica. A questo scopo, seleziona l’area, fai clic sull’icona a forma di ingranaggio e seleziona **Rendi dinamico** o [Sostituisci con frammento](/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/create-a-snippet.md), a seconda di quello che stai facendo).

1. Inserisci il nome Segmentazione, selezionalo e fai clic su **Salva**.

   ![](assets/1.4.png)

   La segmentazione e i relativi segmenti vengono visualizzati nella scheda Dinamico a destra.

   ![](assets/1.5.png)

## Applica contenuto dinamico {#apply-dynamic-content}

>[!CAUTION]
>
>Il numero di elementi di contenuto dinamico consentiti non è illimitato. Anche se non esiste un limite di numero specifico (che può variare in base alla combinazione di contenuto), l’utilizzo eccessivo del contenuto dinamico può influire negativamente sulle prestazioni dell’e-mail. È consigliabile mantenere la quantità di elementi di contenuto dinamico utilizzati per meno di 20 per e-mail.

1. Fai clic sui segmenti e aggiungi l’oggetto.

![](assets/2.1.png)

1. Ripeti per ogni segmento.

   ![](assets/2.2.png)

>[!TIP]
>
>Crea un’e-mail predefinita prima di applicare contenuti ai vari segmenti.

>[!CAUTION]
>
>Le modifiche al blocco di contenuto del segmento predefinito vengono applicate a tutti i segmenti.

Dolce! Ora puoi inviare e-mail flessibili al pubblico di destinazione.

>[!MORELIKETHIS]
>
>* [Visualizzare un’anteprima di un’e-mail con contenuto dinamico](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md)
>* [Utilizzare i contenuti dinamici in una pagina di destinazione](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/use-dynamic-content-in-a-free-form-landing-page.md)

