---
unique-page-id: 2359663
description: Impostare un valore per il campo Modulo nascosto - Documentazione di Marketo - Documentazione del prodotto
title: Impostare un valore per il campo modulo nascosto
exl-id: acec7de1-8567-42c0-a6ce-a91b0bf69f41
feature: Forms
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 1%

---

# Impostare un valore per il campo modulo nascosto {#set-a-hidden-form-field-value}

I campi nascosti vengono in genere compilati in modo dinamico. Non vengono mostrate alla persona che compila il modulo. Di seguito viene illustrato come impostare il valore.

>[!PREREQUISITES]
>
>[Impostare un campo modulo come nascosto](/help/marketo/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.md)

## Seleziona il campo {#select-the-field}

1. Nel modulo, selezionare il campo nascosto e fare clic su **[!UICONTROL Edit]** per **[!UICONTROL Autofill]**.

   ![](assets/autofill.png)

## Usa valore predefinito {#use-default-value}

Selezionando Usa **[!UICONTROL Default Value]** è possibile codificare un valore specifico da utilizzare sempre durante l&#39;invio del modulo. Immettere **[!UICONTROL Default Value]** e fare clic su **[!UICONTROL Save]**.

![](assets/image2014-9-15-13-3a5-3a27.png)

## URL Parameter {#url-parameter}

Se desideri acquisire i parametri URL (stringhe di query) dalla pagina in cui si trova la persona durante la compilazione del modulo, puoi utilizzare **[!UICONTROL URL Parameters]** per popolare il campo nascosto.

>[!NOTE]
>
>I parametri sono piuttosto tecnologici, vero? Una volta ottenuti, però, sono potenti. Questa [pagina Wikipedia sulle stringhe di query](https://en.wikipedia.org/wiki/Query_string) è in qualche modo utile.

1. Selezionare **[!UICONTROL URL Parameter]** per **[!UICONTROL Get Value Type]**.

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. Immettere **[!UICONTROL Parameter Name]** e fare clic su **[!UICONTROL Save]**.

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>È possibile immettere **[!UICONTROL Default Value]** nel caso in cui il parametro URL non venga trovato.

## Valore cookie {#cookie-value}

Se si memorizzano i dati nei cookie, è possibile utilizzare **[!UICONTROL Cookie Value]** per raccogliere i dati al momento dell&#39;invio del modulo.

1. Selezionare **[!UICONTROL Cookie Value]** per **[!UICONTROL Get Value From]**.

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. Immettere il cookie **[!UICONTROL Parameter Name]** desiderato e fare clic su **[!UICONTROL Save]**.

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >È possibile immettere **[!UICONTROL Default Value]** nel caso in cui il parametro/cookie non sia stato trovato.

## Parametro referrer {#referrer-parameter}

Se desideri acquisire i dati dalla pagina da cui proviene il visitatore prima di compilare il modulo, puoi utilizzare **[!UICONTROL Referrer Parameter]**.

1. Imposta **[!UICONTROL Get Value From]** su **[!UICONTROL Referrer Parameter]**.

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. Immettere **[!UICONTROL Parameter Name]** che si desidera acquisire dall&#39;URL del referente e fare clic su **[!UICONTROL Save]**.

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >È possibile immettere **[!UICONTROL Default Value]** nel caso in cui il parametro referrer non sia stato trovato.

1. Fai clic su **[!UICONTROL Finish]**.

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. Fai clic su **[!UICONTROL Approve and Close]**.

   ![](assets/image2014-9-15-13-3a10-3a43.png)
