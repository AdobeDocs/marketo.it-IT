---
unique-page-id: 1146958
description: Invia avviso - Documenti Marketo - Documentazione del prodotto
title: Invia avviso
exl-id: 2016e2e7-0361-4bb2-8740-819e21fbd15b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 1%

---

# Invia avviso {#send-alert}

## Panoramica {#overview}

Marketo può inviare un avviso via e-mail con informazioni personali a chiunque: il proprietario del venditore, un partner o qualcun altro. Utilizza la **Invia avviso** passaggio di flusso.

![](assets/one-1.png)

## Utilizzo {#usage}

1. Trova e seleziona l’e-mail che desideri inviare.

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >L’avviso e-mail deve contenere tutte le informazioni di intestazione e deve essere nel **Approvato** stato.

1. Fai clic sull’icona di anteprima per assicurarti di aver selezionato l’e-mail corretta.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Assicurati di utilizzare il **Invia informazioni avviso** token nell&#39;e-mail.

1. Selezionare il destinatario dell’avviso. È possibile scegliere Proprietario vendite o Proprietario account.

   ![](assets/four-2.png)

1. Facoltativamente, aggiungi qualsiasi altro indirizzo e-mail desiderato (separato da una virgola o da un punto e virgola).

   ![](assets/five.png)

   >[!TIP]
   >
   >Nelle campagne di attivazione, puoi utilizzare i token in **Ad altre e-mail** quali `{{lead.Territory Owner}}` o `{{my.Alert Recipient}}` purché i valori siano indirizzi e-mail validi. Token in **Ad altre e-mail** non funziona in una campagna batch.

Tutto qui! Ora sai come utilizzare il **Invia avviso** passaggio di flusso.

>[!MORELIKETHIS]
>
>[Creare un messaggio e-mail](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md)
