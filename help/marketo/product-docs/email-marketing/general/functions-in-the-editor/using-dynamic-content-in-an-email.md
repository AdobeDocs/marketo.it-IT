---
unique-page-id: 2950617
description: Utilizzo di contenuti dinamici in un’e-mail - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzo di contenuti dinamici in un messaggio e-mail
exl-id: a1178f76-6760-4a4a-9510-f129ee6a9032
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Utilizzo di contenuti dinamici in un messaggio e-mail {#using-dynamic-content-in-an-email}

>[!PREREQUISITES]
>
>[Creare una segmentazione](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

Utilizza il contenuto dinamico nelle e-mail per inviare informazioni di destinazione ai lead.

>[!NOTE]
>
>L’utilizzo di variabili all’interno di contenuto dinamico in un messaggio e-mail è supportato solo quando si utilizzano le campagne Trigger. È **non** supportate quando si utilizzano campagne batch.

## Aggiungi segmentazione {#add-segmentation}

1. Vai a **Attività di marketing**.

   ![](assets/login-marketing-activities.png)

1. Seleziona l’e-mail e fai clic su **Modifica bozza**.

   ![](assets/1.2.png)

1. In questo esempio stiamo rendendo dinamica la riga oggetto. Fai clic nel campo Oggetto, quindi fai clic su **Rendi dinamico** pulsante.

   ![](assets/1.3.png)

   >[!NOTE]
   >
   >Puoi anche rendere dinamico un elemento all’interno dell’e-mail. A questo scopo, seleziona l’area, fai clic sull’icona a forma di ingranaggio e seleziona **Rendi dinamico** (o [Sostituisci con snippet](/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/create-a-snippet.md), a seconda di quello che stai facendo).

1. Inserisci il nome della segmentazione, selezionalo e fai clic su **Salva**.

   ![](assets/1.4.png)

   La segmentazione e i relativi segmenti vengono visualizzati nella scheda Dinamica a destra.

   ![](assets/1.5.png)

## Applicare contenuti dinamici {#apply-dynamic-content}

>[!CAUTION]
>
>Il numero di elementi di contenuto dinamico consentito non è illimitato. Anche se non esiste un limite di numero specifico (può variare in base alla combinazione di contenuti), l’utilizzo eccessivo del contenuto dinamico può influire negativamente sulle prestazioni dell’e-mail. È consigliabile mantenere la quantità di elementi di contenuto dinamico utilizzati al di sotto di 20 per e-mail.

1. Fai clic sui segmenti e aggiungi l’oggetto.

![](assets/2.1.png)

1. Ripeti per ogni segmento.

   ![](assets/2.2.png)

>[!TIP]
>
>Crea un’e-mail predefinita prima di applicare il contenuto ai vari segmenti.

>[!CAUTION]
>
>Le modifiche al blocco di contenuto del segmento predefinito vengono applicate a tutti i segmenti.

Dolce! Ora puoi inviare e-mail flessibili al pubblico di destinazione.

>[!MORELIKETHIS]
>
>* [Anteprima di un’e-mail con contenuto dinamico](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md)
>* [Utilizzare il contenuto dinamico in una pagina di destinazione](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/use-dynamic-content-in-a-free-form-landing-page.md)
