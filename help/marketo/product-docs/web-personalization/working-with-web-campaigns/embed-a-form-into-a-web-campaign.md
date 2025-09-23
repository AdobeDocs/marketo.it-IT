---
unique-page-id: 10095554
description: Incorporare un modulo in una campagna web - Documentazione di Marketo - Documentazione del prodotto
title: Incorporare un modulo in una campagna web
exl-id: 41e60ae6-9a40-444f-8a55-47fc6ef6c5fb
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 8%

---

# Incorporare un modulo in una campagna web {#embed-a-form-into-a-web-campaign}

Scopri come incorporare un modulo di Marketo in una campagna web (finestra di dialogo, nella zona o widget).

1. Fai clic con il pulsante destro del mouse su un modulo approvato. Seleziona **[!UICONTROL Embed Code]**.

   ![](assets/image2015-12-16-10-3a58-3a39.png)

1. Copia il Codice.

   ![](assets/image2015-12-16-11-3a16-3a24.png)

1. In [!DNL Web Personalization], vai a **[!UICONTROL Web Campaigns]**.

   ![](assets/web-campaigns-hand-7.jpg)

1. Fai clic su **[!UICONTROL Create New Campaign]**.

   ![](assets/create-new-web-campaign-hand-1.jpg)

1. Nell’Editor Rich Text, fai clic sull’icona HTML.

   ![](assets/five-1.png)

1. Incolla il codice da incorporare del modulo in [!UICONTROL HTML Source Editor]. Fai clic su **[!UICONTROL Update]**.

   ![](assets/six-1.png)

1. Il modulo non verrà visualizzato nella vista dell’editor, ma puoi visualizzarlo in anteprima per vedere come verrà riprodotto in una campagna.

1. Fare clic su **[!UICONTROL Launch]** per avviare la campagna.

   >[!NOTE]
   >
   >Eventuali modifiche ai campi del modulo devono essere effettuate nell’ambito delle attività di marketing di Marketo in Modifica bozza del modulo.

## Tre modi per aggiungere un&#39;immagine di sfondo a un modulo {#three-ways-to-add-a-background-image-to-a-form}

Per aggiungere un&#39;immagine di sfondo al modulo è possibile:

* Modificare il CSS del tema di un modulo
* Modificare i colori della finestra di dialogo o del widget in Imposta campagna
* Aggiungi codice CSS allo script

Per modificare il CSS di un tema modulo, consulta [questo articolo](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md).

Per modificare i colori della finestra di dialogo o del widget in Imposta campagna:

1. Nell’Editor Rich Text, seleziona un tipo di campagna Finestra di dialogo e uno stile di finestra di dialogo, il colore dell’intestazione e il colore di sfondo per personalizzare i colori di sfondo del modulo. Fai clic su **[!UICONTROL Save]**.

   ![](assets/image2015-12-29-18-3a28-3a31.png)

1. Di seguito è riportato un esempio di come si presenta uno stile di finestra di dialogo Rifilo moderno con un&#39;intestazione viola chiaro e un colore di sfondo.

   ![](assets/image2015-12-29-18-3a27-3a31.png)

Per aggiungere codice CSS allo script:

1. Nell’Editor Rich Text, fai clic sull’icona HTML.

   ![](assets/image2015-12-29-17-3a56-3a13.png)

1. Incolla il codice da incorporare del modulo con il codice di stile di sfondo in [!UICONTROL HTML Source Editor]. Fai clic su **[!UICONTROL Update]**.

   ![](assets/image2015-12-29-18-3a1-3a15.png)

1. Fare clic su **[!UICONTROL Preview]** per vedere come verrà eseguito il rendering in una campagna (il modulo non verrà visualizzato nella visualizzazione editor). Di seguito è riportato un esempio di come viene eseguito il rendering del codice del modulo in una campagna con un’immagine di sfondo.

   ![](assets/image2015-12-29-18-3a20-3a35.png)

>[!MORELIKETHIS]
>
>* [Modifica il CSS di un tema modulo](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md)
>* [Mostra messaggio di ringraziamento senza una pagina di destinazione di completamento](https://developers.marketo.com/blog/show-thank-you-message-without-a-follow-up-landing-page/)
>* [Forms 2.0](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/forms-api-reference)
