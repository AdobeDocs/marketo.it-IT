---
unique-page-id: 42762794
description: Utilizzo di azioni in serie in Salesforce Classic - Documenti Marketo - Documentazione del prodotto
title: Utilizzo di azioni in serie in Salesforce Classic
exl-id: f676ba65-6bc9-41e5-aa70-0f10bceedab7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Utilizzo di azioni in serie in Salesforce Classic {#using-bulk-actions-in-salesforce-classic}

Scopri come eseguire azioni in blocco, ad esempio aggiungere lead a una campagna, inviare un messaggio e-mail in blocco o inviare i lead da Salesforce a Sales Connect.

>[!PREREQUISITES]
>
>Aggiorna la versione più recente del pacchetto Sales Connect e installa i pulsanti di azione collettiva nella visualizzazione lead/contatti. [Fai clic qui per le istruzioni](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf).

>[!NOTE]
>
>Prima di seguire i passaggi descritti, assicurati di aver effettuato l&#39;accesso al tuo account Marketo Sales Connect.

## E-mail in blocco {#bulk-email}

1. In Salesforce, fai clic sul pulsante **Lead** , quindi la **Vai** pulsante .

   ![](assets/one-5.png)

1. Scegli i lead desiderati e fai clic sul pulsante **E-mail con MSC (Classic)** pulsante .

   ![](assets/two-5.png)

1. Verrà visualizzata un&#39;e-mail MSC. Include le seguenti funzionalità:

   a) Il campo &quot;A&quot; mostra &quot;Tutte le entrate&quot;, corrispondente all’elenco di lead scelto nella vista Elenco lead\
   b) Questo elenco è visibile nel pannello a sinistra denominato &quot;Composizione in blocco&quot; - è possibile aggiungere/rimuovere i destinatari qui\
   c. Puoi scegliere un modello o creare un tuo indirizzo e-mail\
   d. Puoi visualizzare in anteprima i campi dinamici che verranno compilati nell’e-mail\
   e. Puoi inviare l’e-mail immediatamente o pianificare l’invio in un secondo momento

   ![](assets/three-4.png)

## Aggiungi a Campaign {#add-to-campaign}

1. In Salesforce, fai clic sul pulsante **Lead** , quindi la **Vai** pulsante .

   ![](assets/four-3.png)

1. Scegli i lead desiderati e fai clic sul pulsante **Aggiungi alla campagna MSC (Classic)** pulsante .

   ![](assets/five-3.png)

1. Verrà visualizzato un pop-up &quot;Aggiungi persone alla tua campagna&quot;. Fai clic su **Successivo** e passa attraverso il flusso tipico della campagna per attivare una campagna MSC.

   ![](assets/six.png)

## Invia a Marketo Sales Connect {#push-to-marketo-sales-connect}

1. In Salesforce, fai clic sul pulsante **Lead** , quindi la **Vai** pulsante .

   ![](assets/seven-1.png)

1. Scegli i lead desiderati e fai clic sul pulsante **Push to MSC (Classic)** pulsante .

   ![](assets/eight-1.png)

1. Viene aperta una nuova scheda denominata &quot;Salesforce Bridge&quot;. Fai clic sul pulsante **Procedi al gruppo →** pulsante .

   ![](assets/nine-1.png)

1. Verrai inviato al tuo account MSC dove vedrai un gruppo creato con data/ora. Riceverai una notifica al termine della sincronizzazione e il gruppo includerà i lead sincronizzati da Salesforce.

   ![](assets/ten.png)

>[!NOTE]
>
>È possibile seguire gli stessi passaggi per utilizzare azioni in blocco anche nella visualizzazione elenco contatti.

>[!MORELIKETHIS]
>
>* [Invio di e-mail tramite e-mail di gruppo](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [Composizione di e-mail in blocco con Seleziona e Invia](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)

