---
unique-page-id: 2359663
description: Impostare un valore per il campo Modulo nascosto - Documentazione di Marketo - Documentazione del prodotto
title: Impostare un valore per il campo modulo nascosto
exl-id: acec7de1-8567-42c0-a6ce-a91b0bf69f41
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# Impostare un valore per il campo modulo nascosto {#set-a-hidden-form-field-value}

I campi nascosti vengono in genere compilati in modo dinamico. Non vengono mostrate alla persona che compila il modulo. Di seguito viene illustrato come impostare il valore.

>[!PREREQUISITES]
>
>[Impostare un campo modulo come nascosto](/help/marketo/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.md)

## Seleziona il campo {#select-the-field}

1. Nel modulo, seleziona il campo nascosto e fai clic su **Modifica** per **Riempimento automatico**.

   ![](assets/autofill.png)

## Usa valore predefinito {#use-default-value}

Selezionando Usa valore predefinito è possibile codificare un valore specifico da utilizzare sempre durante l&#39;invio del modulo. Immettete il valore predefinito e fate clic su Salva (Save).

![](assets/image2014-9-15-13-3a5-3a27.png)

## Parametro URL {#url-parameter}

Se desideri acquisire i parametri URL (stringhe di query) dalla pagina in cui si trova la persona durante la compilazione del modulo, puoi utilizzare **Parametri URL** per compilare il campo nascosto.

>[!NOTE]
>
>I parametri sono piuttosto tecnologici, vero? Una volta ottenuti, però, sono potenti. Questo [Pagina Wikipedia sulle stringhe di query](https://en.wikipedia.org/wiki/Query_string) è in qualche modo utile.

1. Seleziona **Parametro URL** per **Ottieni tipo di valore**.

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. Inserisci il **Nome parametro** e fai clic su **Salva**.

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>Se il parametro URL non viene trovato, puoi immettere un valore predefinito.

## Valore cookie {#cookie-value}

Se memorizzi i dati nei cookie, puoi utilizzare **Valore cookie** per raccogliere i dati quando il modulo viene inviato.

1. Seleziona **Valore cookie** per **Ottieni valore da**.

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. Inserisci il nome del parametro cookie desiderato e fai clic su **Salva**.

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >Se il parametro o il cookie non viene trovato, puoi immettere un valore predefinito.

## Parametro referrer {#referrer-parameter}

Per acquisire i dati dalla pagina di provenienza del visitatore prima di compilare il modulo, puoi utilizzare **Parametro referrer**.

1. Imposta **Ottieni valore da** a **Parametro referrer**.

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. Inserisci il **Nome parametro** che desideri acquisire dall’URL del referente e fai clic su **Salva**.

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >È possibile immettere un valore **Valore predefinito** nel caso in cui il parametro referrer non venga trovato.

1. Clic **Fine**.

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. Clic **Approva e chiudi**.

   ![](assets/image2014-9-15-13-3a10-3a43.png)
