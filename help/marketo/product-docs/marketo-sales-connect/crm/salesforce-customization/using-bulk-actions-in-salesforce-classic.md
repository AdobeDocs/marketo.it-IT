---
unique-page-id: 42762794
description: Utilizzo di azioni in blocco in  [!DNL Salesforce] Classic - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzo di azioni in blocco in  [!DNL Salesforce] Classic
exl-id: f676ba65-6bc9-41e5-aa70-0f10bceedab7
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---

# Utilizzo di azioni in blocco in [!DNL Salesforce] Classic {#using-bulk-actions-in-salesforce-classic}

Scopri come eseguire azioni in blocco, come l’aggiunta di lead a una campagna, l’invio di un’e-mail in blocco o il push di lead da [!DNL Salesforce] a [!DNL Sales Connect].

>[!PREREQUISITES]
>
>Eseguire l&#39;aggiornamento alla versione più recente del pacchetto [!DNL Sales Connect] e installare i pulsanti di azione collettiva nella visualizzazione lead/contatti. [Fare clic qui per le istruzioni](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf).

>[!NOTE]
>
>Prima di seguire i passaggi descritti, verificare di aver effettuato l&#39;accesso all&#39;account Marketo Sales Connect.

## E-mail in blocco {#bulk-email}

1. In [!DNL Salesforce], fare clic sulla scheda **[!UICONTROL Leads]**, quindi sul pulsante **[!UICONTROL Go]**.

   ![](assets/one-5.png)

1. Scegliere i lead desiderati e fare clic sul pulsante **[!UICONTROL Email with MSC (Classic)]**.

   ![](assets/two-5.png)

1. Verrà visualizzata un&#39;e-mail MSC. Include le seguenti funzionalità:

   a. Il campo &quot;[!UICONTROL To]&quot; mostra &quot;[!UICONTROL All Recipients]&quot; - corrisponde all&#39;elenco di lead scelti nella visualizzazione elenco lead\
   b. L&#39;elenco è visibile nel pannello sinistro denominato &quot;[!UICONTROL Bulk Compose]&quot;. Qui è possibile aggiungere/rimuovere i destinatari\
   c. Puoi scegliere un modello o creare un messaggio e-mail personalizzato\
   d. Puoi visualizzare in anteprima i campi dinamici che verranno compilati nel messaggio e-mail\
   e. Puoi inviare l’e-mail immediatamente o pianificare l’invio in un secondo momento

   ![](assets/three-4.png)

## Aggiungi a campagna {#add-to-campaign}

1. In [!DNL Salesforce], fare clic sulla scheda **[!UICONTROL Leads]**, quindi sul pulsante **[!UICONTROL Go]**.

   ![](assets/four-3.png)

1. Scegliere i lead desiderati e fare clic sul pulsante **[!UICONTROL Add to MSC Campaign (Classic)]**.

   ![](assets/five-3.png)

1. Verrà visualizzato un pop-up &quot;[!UICONTROL Add People to Your Campaign]&quot;. Fai clic su **[!UICONTROL Next]** e segui il flusso tipico delle campagne per attivare una campagna MSC.

   ![](assets/six.png)

## Invia a Marketo Sales Connect {#push-to-marketo-sales-connect}

1. In [!DNL Salesforce], fare clic sulla scheda **[!UICONTROL Leads]**, quindi sul pulsante **[!UICONTROL Go]**.

   ![](assets/seven-1.png)

1. Scegliere i lead desiderati e fare clic sul pulsante **[!UICONTROL Push to MSC (Classic)]**.

   ![](assets/eight-1.png)

1. Verrà aperta una nuova scheda denominata &quot;[!UICONTROL Salesforce Bridge]&quot;. Fare clic sul pulsante **[!UICONTROL Proceed to Group →]**.

   ![](assets/nine-1.png)

1. Verrai indirizzato al tuo account MSC, dove vedrai un gruppo creato con data/ora. Riceverai una notifica una volta completata la sincronizzazione e il gruppo includerà i lead sincronizzati da [!DNL Salesforce].

   ![](assets/ten.png)

>[!NOTE]
>
>È possibile seguire gli stessi passaggi per utilizzare azioni in blocco anche nella visualizzazione elenco contatti.

>[!MORELIKETHIS]
>
>* [Invio di e-mail tramite e-mail gruppo](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [Composizione di e-mail in blocco con Seleziona e invia](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)
