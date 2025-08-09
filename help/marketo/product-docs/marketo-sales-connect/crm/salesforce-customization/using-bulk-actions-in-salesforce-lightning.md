---
unique-page-id: 42762825
description: 'Utilizzo di azioni in blocco in Salesforce Lightning: documenti Marketo: documentazione del prodotto'
title: Utilizzo di azioni in blocco in Salesforce Lightning
exl-id: 72022507-6568-4cc2-b3b5-c1703a1493ad
feature: Marketo Sales Connect
source-git-commit: 8364c0ebe19bce0d837a96283bea31d593ef4171
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# Utilizzo di azioni in blocco in [!DNL Salesforce Lightning] {#using-bulk-actions-in-salesforce-lightning}

Scopri come eseguire azioni in blocco, come l’aggiunta di lead a una campagna, l’invio di un’e-mail in blocco o il push di lead da [!DNL Salesforce] a [!DNL Sales Connect].

>[!PREREQUISITES]
>
>Eseguire l&#39;aggiornamento alla versione più recente del pacchetto [!DNL Sales Connect] e installare i pulsanti di azione collettiva nella visualizzazione lead/contatti.
>* [Istruzioni in inglese] (assets/SF+Guide+for+Lightning-EN)
>* [Istruzioni in giapponese] (assets/SF+Guide+for+Lightning-JA)

>[!NOTE]
>
>Prima di eseguire la procedura seguente, verificare di aver effettuato l&#39;accesso al proprio account [!DNL Marketo Sales Connect].

## E-mail in blocco {#bulk-email}

1. In [!DNL Salesforce], fai clic sulla scheda **[!UICONTROL Leads]**, quindi scegli l&#39;elenco dei lead desiderati.

   ![](assets/one-6.png)

   >[!NOTE]
   >
   >Se sei già presente nell’elenco che utilizzerai, dovrai eseguirlo nuovamente scegliendolo dall’elenco a discesa per assicurarti che vengano visualizzati i pulsanti delle azioni in blocco MSC. Questo è il comportamento [!DNL Salesforce] che non può essere modificato.

1. Fare clic sull&#39;elenco a discesa della freccia (all&#39;estrema destra dello schermo) e selezionare **[!UICONTROL Email with MSC]**.

   ![](assets/two-6.png)

1. Verrà visualizzata un&#39;e-mail MSC. Include le seguenti funzionalità:

   a. Il campo &quot;[!UICONTROL To]&quot; mostra &quot;Tutte le ricezioni&quot; - corrisponde all&#39;elenco di lead scelti nella visualizzazione elenco lead
b. Questo elenco è visibile nel pannello a sinistra denominato &quot;Composizione in blocco&quot;. Qui puoi aggiungere/rimuovere i destinatari
c. Puoi scegliere un modello o creare un messaggio e-mail personalizzato
d. Puoi inviare l’e-mail immediatamente o pianificare l’invio in un secondo momento

   ![](assets/three-5.png)

## Aggiungi a campagna {#add-to-campaign}

1. In [!DNL Salesforce], fai clic sulla scheda **[!UICONTROL Leads]**, quindi scegli l&#39;elenco dei lead desiderati.

   ![](assets/four-4.png)

1. Fare clic sull&#39;elenco a discesa della freccia (all&#39;estrema destra dello schermo) e selezionare **[!UICONTROL Add to MSC Campaign]**.

   ![](assets/five-4.png)

1. Verrà visualizzato un pop-up &quot;[!UICONTROL Add People to Your Campaign]&quot;. Fai clic su **[!UICONTROL Next]** e segui il flusso tipico delle campagne per attivare una campagna MSC.

   ![](assets/six-1.png)

## Invia a [!DNL Marketo Sales Connect] {#push-to-marketo-sales-connect}

1. In [!DNL Salesforce], fai clic sulla scheda **[!UICONTROL Leads]**, quindi scegli l&#39;elenco dei lead desiderati.

   ![](assets/seven-2.png)

1. Fare clic sull&#39;elenco a discesa della freccia (all&#39;estrema destra dello schermo) e selezionare **[!UICONTROL Push to MSC]**.

   ![](assets/eight-2.png)

1. Verrà aperta una nuova scheda denominata &quot;[!DNL Salesforce] Bridge&quot;. Fare clic sul pulsante **[!UICONTROL Proceed to Group]→**.

   ![](assets/nine-2.png)

1. Verrai indirizzato al tuo account MSC, dove vedrai un gruppo creato con data/ora. Riceverai una notifica una volta completata la sincronizzazione e il gruppo includerà i lead sincronizzati da [!DNL Salesforce].

   ![](assets/ten-1.png)

>[!NOTE]
>
>È possibile seguire gli stessi passaggi per utilizzare azioni in blocco anche nella visualizzazione elenco contatti.

>[!MORELIKETHIS]
>
>* [Invio di e-mail tramite e-mail gruppo](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [Composizione di e-mail in blocco con Seleziona e invia](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)
