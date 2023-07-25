---
unique-page-id: 1147352
description: Inviare un messaggio e-mail di esempio - Documentazione di Marketo - Documentazione del prodotto
title: Invia e-mail di esempio
exl-id: b8f845e8-5c5e-463d-9d60-9c8103cec5ac
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# Invia e-mail di esempio {#send-a-sample-email}

È facile e veloce inviare campioni di un’e-mail. Per inviare un messaggio e-mail con contenuto dinamico, consulta [Anteprima di un’e-mail con contenuto dinamico](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md).

>[!NOTE]
>
>È necessario disporre di **Database di Access - Eseguire azioni a flusso singolo** autorizzazione per l’invio di e-mail di esempio.

## Invia e-mail di esempio {#send-a-sample-email-1}

1. Trova e seleziona l’e-mail. Fai clic su **Azioni e-mail** a discesa e selezionare **Invia esempio**.\
   ![](assets/one-281-29.jpg)

   >[!NOTE]
   >
   >I miei token vengono risolti nel valore appropriato per il programma dell’e-mail.

1. Inserisci uno o più indirizzi e-mail per la consegna. Per più indirizzi e-mail, utilizza le virgole per separarli. Clic **Invia** al termine.

   ![](assets/two.png)

   >[!IMPORTANT]
   >
   >Se immetti più indirizzi e-mail, questi saranno tutti visibili a ogni destinatario. Il primo indirizzo immesso sarà il destinatario principale e ogni indirizzo e-mail successivo sarà un destinatario CC.

   >[!TIP]
   >
   >Se desideri risolvere i token come una persona specifica, scegli tale persona nel **elenco a discesa della persona** nel passaggio 2.

## Invia un&#39;e-mail di esempio durante la modifica {#send-a-sample-email-while-editing}

1. Trova l’e-mail, selezionala e fai clic su **Modifica bozza** scheda.

   ![](assets/three-281-29.jpg)

1. Clic **Azioni e-mail**, seleziona **Invia esempio**.

   ![](assets/four.png)

1. Immetti un indirizzo e-mail per la consegna e fai clic su **Invia**.

   ![](assets/two.png)

   >[!NOTE]
   >
   >Il campo trigger è applicabile solo a coloro che utilizzano [scripting e-mail](https://developers.marketo.com/documentation/velocity-script/).

## Inviare un messaggio e-mail di esempio basato su un segmento {#send-a-sample-email-based-on-a-segment}

>[!PREREQUISITES]
>
>[Applicare la segmentazione all’e-mail](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/using-dynamic-content-in-an-email.md).

1. Trova l’e-mail, selezionala e fai clic su **Modifica bozza** scheda.

   ![](assets/three-281-29.jpg)

1. Clic **Anteprima**.

   ![](assets/1.png)

1. Fai clic su **Visualizza per** a discesa e selezionare **Segmentazione**.

   ![](assets/2.png)

1. Viene visualizzato un elenco a discesa con le segmentazioni disponibili. Fai clic su di esso e seleziona quello desiderato.

   ![](assets/3.png)

1. Utilizza le frecce per scorrere le opzioni (in questo caso abbiamo modificato dinamicamente l’oggetto).

   ![](assets/4.png)

1. Clic **Invia esempio** per ricevere un’e-mail di test del segmento in azione.

   ![](assets/5.png)

   >[!TIP]
   >
   >Puoi anche inviare un’e-mail di esempio basata su un segmento nella modalità di modifica dell’e-mail. Fai clic su **Azioni e-mail** a discesa, seleziona **Invia esempio**, quindi scegli il segmento.

Campionare i contenuti prima di lanciare una campagna è molto importante. Misura due volte, taglia una volta!
