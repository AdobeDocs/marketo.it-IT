---
unique-page-id: 2359663
description: Impostare un valore campo modulo nascosto - Documenti Marketo - Documentazione del prodotto
title: Impostare un valore per un campo modulo nascosto
exl-id: acec7de1-8567-42c0-a6ce-a91b0bf69f41
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# Impostare un valore per un campo modulo nascosto {#set-a-hidden-form-field-value}

I campi nascosti vengono in genere compilati in modo dinamico. Non vengono mostrati alla persona che compila il modulo. Ecco come impostare il valore.

>[!PREREQUISITES]
>
>[Impostare un campo modulo come nascosto](/help/marketo/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.md)

## Selezionare il campo {#select-the-field}

1. Nel modulo, selezionare il campo nascosto e fare clic su **Modifica** per **Riempimento automatico**.

   ![](assets/autofill.png)

## Usa valore predefinito {#use-default-value}

Selezionando Usa valore predefinito è possibile codificare un valore specifico da utilizzare sempre durante l’invio del modulo. Inserisci il valore predefinito e fai clic su Salva.

![](assets/image2014-9-15-13-3a5-3a27.png)

## Parametro URL {#url-parameter}

Se si desidera acquisire i parametri URL (stringhe di query) dalla pagina in cui si trova la persona durante la compilazione del modulo, è possibile utilizzare **Parametri URL** per compilare il campo nascosto.

>[!NOTE]
>
>I parametri sono un po&#39; tecnologici, vero? Ma una volta che le ottieni, sono potenti. Questo [Pagina Wikipedia sulle stringhe di query](https://en.wikipedia.org/wiki/Query_string) è in qualche modo utile.

1. Seleziona **Parametro URL** per **Ottieni tipo di valore**.

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. Inserisci il **Nome parametro** e fai clic su **Salva**.

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>È possibile immettere un valore predefinito nel caso in cui il parametro URL non sia trovato.

## Valore cookie {#cookie-value}

Se i dati vengono memorizzati nei cookie, puoi utilizzare **Valore cookie** per raccogliere i dati durante l’invio del modulo.

1. Seleziona **Valore cookie** per **Ottieni valore da**.

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. Immetti il nome del parametro del cookie desiderato e fai clic su **Salva**.

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >È possibile immettere un valore predefinito nel caso in cui il parametro/cookie non sia trovato.

## Parametro referrer {#referrer-parameter}

Se si desidera acquisire i dati dalla pagina di origine del visitatore prima di compilare il modulo, è possibile utilizzare **Parametro referrer**.

1. Imposta **Ottieni valore da** a **Parametro referrer**.

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. Inserisci il **Nome parametro** dall’URL del referente e fai clic su **Salva**.

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >È possibile immettere un **Valore predefinito** nel caso in cui il parametro referrer non sia stato trovato.

1. Fai clic su **Fine**.

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. Fai clic su **Approva e chiudi**.

   ![](assets/image2014-9-15-13-3a10-3a43.png)
