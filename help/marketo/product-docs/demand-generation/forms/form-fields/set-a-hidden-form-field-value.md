---
unique-page-id: 2359663
description: Impostare un valore campo modulo nascosto - Documenti Marketo - Documentazione prodotto
title: Impostazione di un valore campo modulo nascosto
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---


# Impostazione di un valore campo modulo nascosto {#set-a-hidden-form-field-value}

In genere, i campi nascosti vengono compilati in modo dinamico. Non vengono mostrate alla persona che compila il modulo. Come impostare il valore.

>[!NOTE]
>
>**Prerequisiti**
>
>[Impostazione di un campo modulo come nascosto](set-a-form-field-as-hidden.md)

## Selezionare il campo {#select-the-field}

1. Nel modulo, selezionare il campo nascosto e fare clic su **Modifica** per la compilazione **automatica**.

   ![](assets/autofill.png)

## Usa valore predefinito {#use-default-value}

Selezionando Usa valore predefinito è possibile codificare un valore specifico da utilizzare sempre all&#39;invio del modulo. Immettete il valore predefinito e fate clic su Salva.

![](assets/image2014-9-15-13-3a5-3a27.png)

## Parametro URL {#url-parameter}

Se si desidera acquisire i parametri URL (stringhe di query) dalla pagina in cui si trova l&#39;utente durante la compilazione del modulo, è possibile utilizzare **URL** **Parameters** per compilare il campo nascosto.

>[!NOTE]
>
>I parametri sono un po&#39; tecnologici, vero? Ma una volta che li ottenete, sono potenti. Questa pagina [Wikipedia sulle stringhe](http://en.wikipedia.org/wiki/Query_string) di query è in qualche modo utile.

1. Selezionate Parametro **** URL per **Ottieni tipo** di valore.

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. Immettete il nome **del** parametro e fate clic su **Salva**.

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>Potete immettere un valore predefinito nel caso in cui il parametro URL non venga trovato.

## Valore cookie {#cookie-value}

Se si memorizzano i dati nei cookie, è possibile utilizzare **Cookie** **Value** per recuperare i dati all&#39;invio del modulo.

1. Selezionare **Cookie** **Value** per **Get** **Value** **From**.

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. Immettete il nome del parametro cookie desiderato e fate clic su **Salva**.

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >Potete immettere un valore predefinito nel caso in cui il parametro/cookie non venga trovato.

## Parametro referrer {#referrer-parameter}

Se si desidera acquisire i dati dalla pagina di origine del visitatore prima di compilare il modulo, è possibile utilizzare **Referrer** **Parameter**.

1. Impostate **Get** **Value** **From** to **Referrer** **Parameter**.

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. Immettete il nome **del** parametro da acquisire dall’URL del referente e fate clic su **Salva**.

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >Potete immettere un **valore** **predefinito** nel caso in cui il parametro del referente non venga trovato.

1. Fare clic su **Fine**.

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. Fate clic su **Approva e chiudi**.

   ![](assets/image2014-9-15-13-3a10-3a43.png)

Dolce! Stai piuttosto bene. Per saperne di più sui [moduli](http://docs.marketo.com/display/docs/forms).
