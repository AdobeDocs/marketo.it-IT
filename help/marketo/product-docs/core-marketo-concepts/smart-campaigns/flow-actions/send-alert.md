---
unique-page-id: 1146958
description: Inviare un avviso - Documentazione di Marketo - Documentazione del prodotto
title: Invia avviso
exl-id: 2016e2e7-0361-4bb2-8740-819e21fbd15b
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 2%

---

# Invia avviso {#send-alert}

Marketo Engage può inviare un messaggio e-mail di notifica con le informazioni personali a chiunque: il proprietario, un partner o un altro utente. Utilizza il passaggio di flusso &quot;[!UICONTROL Send Alert]&quot;.

![](assets/send-alert-1.png)

1. Trova e seleziona l’e-mail che desideri inviare.

   ![](assets/send-alert-2.png)

   >[!NOTE]
   >
   >L&#39;avviso e-mail deve contenere tutte le informazioni di intestazione ed essere nello stato **[!UICONTROL Approved]**.

1. Puoi fare clic sull’icona di anteprima per assicurarti di aver selezionato l’e-mail corretta.

   ![](assets/send-alert-3.png)

   >[!NOTE]
   >
   >Assicurarsi di utilizzare il token &quot;[!UICONTROL Send Alert Info]&quot; nel messaggio e-mail.

1. Selezionare il destinatario dell&#39;avviso. È possibile scegliere [!UICONTROL Sales Owner] o [!UICONTROL Account Owner].

   ![](assets/send-alert-4.png)

1. Se necessario, aggiungi altri indirizzi e-mail, separati da virgola o punto e virgola.

   ![](assets/send-alert-5.png)

   >[!TIP]
   >
   >Nelle campagne di attivazione è possibile utilizzare i token in **[!UICONTROL To Other Emails]**, ad esempio `{{lead.Territory Owner}}` o `{{my.Alert Recipient}}`, purché i valori siano indirizzi e-mail validi. I token in **[!UICONTROL To Other Emails]** non funzioneranno in una campagna batch.

>[!MORELIKETHIS]
>
>[Crea un&#39;e-mail](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md){target="_blank"}
