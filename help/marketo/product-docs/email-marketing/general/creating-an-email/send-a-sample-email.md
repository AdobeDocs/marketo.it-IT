---
unique-page-id: 1147352
description: Inviare un messaggio e-mail di esempio - Documentazione di Marketo - Documentazione del prodotto
title: Invia e-mail di esempio
exl-id: b8f845e8-5c5e-463d-9d60-9c8103cec5ac
feature: Email Editor
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# Invia e-mail di esempio {#send-a-sample-email}

È facile e veloce inviare campioni di un’e-mail. Per inviare un&#39;e-mail di contenuto dinamico, vedere [Anteprima di un&#39;e-mail con contenuto dinamico](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md).

>[!NOTE]
>
>Per inviare e-mail di esempio è necessario disporre dell&#39;autorizzazione **Database di Access - Esegui azioni a flusso singolo**.

## Invia e-mail di esempio {#send-a-sample-email-1}

1. Trova e seleziona l’e-mail. Fare clic sul menu a discesa **[!UICONTROL Email Actions]** e selezionare **[!UICONTROL Send Sample]**.
   ![](assets/one-281-29.jpg)

   >[!NOTE]
   >
   >I miei token vengono risolti nel valore appropriato per il programma dell’e-mail.

1. Inserisci uno o più indirizzi e-mail per la consegna. Per più indirizzi e-mail, utilizza le virgole per separarli. Al termine, fai clic su **[!UICONTROL Send]**.

   ![](assets/two.png)

   >[!IMPORTANT]
   >
   >Se immetti più indirizzi e-mail, questi saranno tutti visibili a ogni destinatario. Il primo indirizzo immesso sarà il destinatario principale e ogni indirizzo e-mail successivo sarà un destinatario CC.

   >[!TIP]
   >
   >Se desideri risolvere i token come persona specifica, scegli tale persona nel menu a discesa **persona** nel passaggio 2.

## Invia un&#39;e-mail di esempio durante la modifica {#send-a-sample-email-while-editing}

1. Trovare l&#39;e-mail, selezionarla e fare clic sulla scheda **[!UICONTROL Edit Draft]**.

   ![](assets/three-281-29.jpg)

1. Fare clic su **[!UICONTROL Email Actions]**, selezionare **[!UICONTROL Send Sample]**.

   ![](assets/four.png)

1. Immettere un indirizzo di posta elettronica per la consegna e fare clic su **[!UICONTROL Send]**.

   ![](assets/two.png)

   >[!NOTE]
   >
   >Il campo trigger è applicabile solo a coloro che utilizzano [script e-mail](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/email-scripting).

## Inviare un messaggio e-mail di esempio basato su un segmento {#send-a-sample-email-based-on-a-segment}

>[!PREREQUISITES]
>
>[Applica segmentazione all&#39;e-mail](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/using-dynamic-content-in-an-email.md).

1. Trovare l&#39;e-mail, selezionarla e fare clic sulla scheda **[!UICONTROL Edit Draft]**.

   ![](assets/three-281-29.jpg)

1. Fai clic su **[!UICONTROL Preview]**.

   ![](assets/1.png)

1. Fare clic sul menu a discesa **[!UICONTROL View By]** e selezionare **[!UICONTROL Segmentation]**.

   ![](assets/2.png)

1. Viene visualizzato un elenco a discesa con le segmentazioni disponibili. Fai clic su di esso e seleziona quello desiderato.

   ![](assets/3.png)

1. Utilizza le frecce per scorrere le opzioni (in questo caso abbiamo modificato dinamicamente l’oggetto).

   ![](assets/4.png)

1. Fai clic su **[!UICONTROL Send Sample]** per ricevere un&#39;e-mail di prova del segmento in azione.

   ![](assets/5.png)

   >[!TIP]
   >
   >Puoi anche inviare un’e-mail di esempio basata su un segmento nella modalità di modifica dell’e-mail. Fai clic sull&#39;elenco a discesa **[!UICONTROL Email Actions]**, seleziona **[!UICONTROL Send Sample]**, quindi scegli il tuo segmento.

Campionare i contenuti prima di lanciare una campagna è molto importante. Misura due volte, taglia una volta!
