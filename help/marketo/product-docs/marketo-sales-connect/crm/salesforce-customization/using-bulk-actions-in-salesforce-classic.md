---
unique-page-id: 42762794
description: Utilizzo di azioni in blocco in Salesforce Classic - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzo di azioni in blocco in Salesforce Classic
exl-id: f676ba65-6bc9-41e5-aa70-0f10bceedab7
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---

# Utilizzo di azioni in blocco in Salesforce Classic {#using-bulk-actions-in-salesforce-classic}

Scopri come eseguire azioni in blocco, come l’aggiunta di lead a una campagna, l’invio di un’e-mail in blocco o il push di lead da Salesforce a Sales Connect.

>[!PREREQUISITES]
>
>Aggiornare alla versione più recente del pacchetto Sales Connect e installare i pulsanti di azione collettiva nella vista lead/contatto. [Fare clic qui per le istruzioni](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf).

>[!NOTE]
>
>Prima di seguire i passaggi descritti, verificare di aver effettuato l&#39;accesso all&#39;account Marketo Sales Connect.

## E-mail in blocco {#bulk-email}

1. In Salesforce, fai clic sulla scheda **Lead**, quindi sul pulsante **Vai**.

   ![](assets/one-5.png)

1. Scegli i lead desiderati e fai clic sul pulsante **E-mail con MSC (Classic)**.

   ![](assets/two-5.png)

1. Verrà visualizzata un&#39;e-mail MSC. Include le seguenti funzionalità:

   a. Il campo &quot;A&quot; mostra &quot;Tutte le ricezioni&quot;: corrisponde all&#39;elenco dei lead scelti nella vista Elenco lead\
   b. Questo elenco è visibile nel pannello a sinistra denominato &quot;Composizione in blocco&quot;. Qui puoi aggiungere/rimuovere i destinatari\
   c. Puoi scegliere un modello o creare un messaggio e-mail personalizzato\
   d. Puoi visualizzare in anteprima i campi dinamici che verranno compilati nel messaggio e-mail\
   e. Puoi inviare l’e-mail immediatamente o pianificare l’invio in un secondo momento

   ![](assets/three-4.png)

## Aggiungi a campagna {#add-to-campaign}

1. In Salesforce, fai clic sulla scheda **Lead**, quindi sul pulsante **Vai**.

   ![](assets/four-3.png)

1. Scegli i lead desiderati e fai clic sul pulsante **Aggiungi a campagna MSC (Classic)**.

   ![](assets/five-3.png)

1. Viene visualizzata la finestra a comparsa Aggiungi persone alla campagna. Fai clic su **Avanti** e segui il flusso tipico della campagna per attivare una campagna MSC.

   ![](assets/six.png)

## Invia a Marketo Sales Connect {#push-to-marketo-sales-connect}

1. In Salesforce, fai clic sulla scheda **Lead**, quindi sul pulsante **Vai**.

   ![](assets/seven-1.png)

1. Scegli i lead desiderati e fai clic sul pulsante **Push to MSC (Classic)**.

   ![](assets/eight-1.png)

1. Si aprirà una nuova scheda denominata &quot;Salesforce Bridge&quot;. Fare clic sul pulsante **Procedi al gruppo →**.

   ![](assets/nine-1.png)

1. Verrai indirizzato al tuo account MSC, dove vedrai un gruppo creato con data/ora. Riceverai una notifica una volta completata la sincronizzazione e il gruppo includerà i lead sincronizzati da Salesforce.

   ![](assets/ten.png)

>[!NOTE]
>
>È possibile seguire gli stessi passaggi per utilizzare azioni in blocco anche nella visualizzazione elenco contatti.

>[!MORELIKETHIS]
>
>* [Invio di e-mail tramite e-mail gruppo](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [Composizione di e-mail in blocco con Seleziona e invia](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)
