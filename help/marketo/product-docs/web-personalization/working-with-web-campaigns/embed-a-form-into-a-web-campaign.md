---
unique-page-id: 10095554
description: Incorporare un modulo in una campagna web - Documenti Marketo - Documentazione del prodotto
title: Incorporare un modulo in una campagna web
exl-id: 41e60ae6-9a40-444f-8a55-47fc6ef6c5fb
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# Incorporare un modulo in una campagna web {#embed-a-form-into-a-web-campaign}

Scopri come incorporare un modulo Marketo in una campagna web (Finestra di dialogo, Area di lavoro o Widget).

1. Fare clic con il pulsante destro del mouse su un modulo approvato. Seleziona **Codice di incorporamento**.

   ![](assets/image2015-12-16-10-3a58-3a39.png)

1. Copia il Codice.

   ![](assets/image2015-12-16-11-3a16-3a24.png)

1. In Personalizzazione web, vai a **Campagne web**.

   ![](assets/web-campaigns-hand-7.jpg)

1. Fai clic su **Crea nuova campagna**.

   ![](assets/create-new-web-campaign-hand-1.jpg)

1. Nell’Editor Rich Text, fai clic sull’icona HTML .

   ![](assets/five-1.png)

1. Incolla il codice di incorporamento del modulo nell’Editor origine di HTML. Fai clic su **Aggiorna**.

   ![](assets/six-1.png)

1. Il modulo non verrà visualizzato nella vista dell’editor, ma è possibile visualizzarlo in anteprima per vedere come verrà riprodotto in una campagna.

1. Fai clic su **Launch** per avviare la campagna.

   >[!NOTE]
   >
   >Eventuali modifiche ai campi del modulo devono essere effettuate all’interno di Attività di marketing Marketo in Modifica bozza del modulo.

## Tre modi per aggiungere un’immagine di sfondo a un modulo {#three-ways-to-add-a-background-image-to-a-form}

Per aggiungere un’immagine di sfondo al modulo, è possibile:

* Modificare il CSS di un tema del modulo
* Modificare i colori della finestra di dialogo o del widget in Imposta campagna
* Aggiungi il codice CSS allo script

Per modificare il CSS di un tema di modulo, consulta [articolo](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md).

Per modificare i colori della finestra di dialogo o del widget in Imposta campagna:

1. Nell’Editor Rich Text, selezionare un tipo di campagna Finestra di dialogo e uno stile di finestra di dialogo, un colore di intestazione e un colore di sfondo per personalizzare i colori di sfondo del modulo. Fai clic su **Salva**.

   ![](assets/image2015-12-29-18-3a28-3a31.png)

1. Ecco un esempio di come si presenta uno stile finestra di dialogo Rifila moderno con un&#39;intestazione e un colore di sfondo viola chiari.

   ![](assets/image2015-12-29-18-3a27-3a31.png)

Per aggiungere codice CSS allo script:

1. Nell’Editor Rich Text, fai clic sull’icona HTML .

   ![](assets/image2015-12-29-17-3a56-3a13.png)

1. Incollare il codice da incorporare del modulo con il codice di stile di sfondo nell’Editor origine di HTML. Fai clic su **Aggiorna**.

   ![](assets/image2015-12-29-18-3a1-3a15.png)

1. Fai clic su **Anteprima** per vedere come verrà eseguito il rendering in una campagna (il modulo non verrà visualizzato nella vista editor). Ecco un esempio del rendering del codice modulo riportato sopra in una campagna con un’immagine di sfondo.

   ![](assets/image2015-12-29-18-3a20-3a35.png)

>[!MORELIKETHIS]
>
>* [Modificare il CSS di un tema del modulo](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md)
>* [Mostra messaggio di ringraziamento senza una pagina di destinazione di follow-up](https://developers.marketo.com/blog/show-thank-you-message-without-a-follow-up-landing-page/)
>* [Forms 2.0](https://developers.marketo.com/documentation/websites/forms-2-0/)

