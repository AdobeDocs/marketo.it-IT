---
unique-page-id: 1146958
description: Invia avviso - Documenti Marketo - Documentazione prodotto
title: Invia avviso
translation-type: tm+mt
source-git-commit: 4a0bd2efe99284807a46d07ffef0070d9a303631
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---


# Invia avviso {#send-alert}

## Panoramica {#overview}

Marketo può inviare un avviso via e-mail con informazioni sulle persone a chiunque, il proprietario della vendita, un partner o qualcun altro. Utilizzare il passaggio di flusso **Invia avviso**.

![](assets/one-1.png)

## Utilizzo {#usage}

1. Individuate e selezionate il messaggio e-mail da inviare.

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >L&#39;avviso e-mail deve contenere tutte le informazioni di intestazione e deve trovarsi nello stato **Approvato**.

1. Potete fare clic sull’icona di anteprima per verificare di aver selezionato l’e-mail corretta.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Assicurarsi di utilizzare il token **Invia informazioni avviso** nell&#39;e-mail.

1. Seleziona il destinatario dell’avviso. È possibile scegliere Proprietario vendita o Proprietario account.

   ![](assets/four-2.png)

1. Facoltativamente, potete aggiungere altri indirizzi e-mail (separati da virgola o punto e virgola).

   ![](assets/five.png)

   >[!TIP]
   >
   >Nelle campagne di attivazione, è possibile utilizzare i token in **Alle altre e-mail** come `{{lead.Territory Owner}}` o `{{my.Alert Recipient}}` purché i valori siano indirizzi e-mail validi. I token in **Ad altre e-mail** non funzioneranno in una campagna batch.

È tutto! Ora è possibile utilizzare il passaggio di flusso **Invia avviso**.

>[!MORELIKETHIS]
>
>[Creare un messaggio e-mail](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md)
