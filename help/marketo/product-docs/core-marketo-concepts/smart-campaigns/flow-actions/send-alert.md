---
unique-page-id: 1146958
description: Inviare un avviso - Documentazione di Marketo - Documentazione del prodotto
title: Invia avviso
exl-id: 2016e2e7-0361-4bb2-8740-819e21fbd15b
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '153'
ht-degree: 0%

---

# Invia avviso {#send-alert}

Il Marketo Engage può inviare un avviso tramite e-mail con informazioni personali a chiunque: il proprietario dell&#39;azienda, un partner o qualcun altro. Utilizza il passaggio di flusso &quot;[!UICONTROL Invia avviso]&quot;.

![](assets/send-alert-1.png)

1. Trova e seleziona l’e-mail che desideri inviare.

   ![](assets/send-alert-2.png)

   >[!NOTE]
   >
   >L&#39;avviso e-mail deve contenere tutte le informazioni di intestazione ed essere nello stato **[!UICONTROL Approvato]**.

1. Puoi fare clic sull’icona di anteprima per assicurarti di aver selezionato l’e-mail corretta.

   ![](assets/send-alert-3.png)

   >[!NOTE]
   >
   >Assicurati di utilizzare il token &quot;[!UICONTROL Invia informazioni avviso]&quot; nel messaggio e-mail.

1. Selezionare il destinatario dell&#39;avviso. Puoi scegliere [!UICONTROL Proprietario vendite] o [!UICONTROL Proprietario account].

   ![](assets/send-alert-4.png)

1. Se necessario, aggiungi altri indirizzi e-mail, separati da virgola o punto e virgola.

   ![](assets/send-alert-5.png)

   >[!TIP]
   >
   >Nelle campagne di attivazione, puoi utilizzare i token in **[!UICONTROL Per altre e-mail]** come `{{lead.Territory Owner}}` o `{{my.Alert Recipient}}`, purché i valori siano indirizzi e-mail validi. I token in **[!UICONTROL ad altre e-mail]** non funzioneranno in una campagna batch.

>[!MORELIKETHIS]
>
>[Crea un&#39;e-mail](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md){target="_blank"}
