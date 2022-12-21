---
unique-page-id: 42762825
description: Utilizzo di azioni in serie in Salesforce Lightning - Documenti Marketo - Documentazione del prodotto
title: Utilizzo di azioni in serie in Salesforce Lightning
exl-id: 72022507-6568-4cc2-b3b5-c1703a1493ad
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Utilizzo di azioni in serie in Salesforce Lightning {#using-bulk-actions-in-salesforce-lightning}

Scopri come eseguire azioni in blocco, ad esempio aggiungere lead a una campagna, inviare un messaggio e-mail in blocco o inviare i lead da Salesforce a Sales Connect.

>[!PREREQUISITES]
>
>Aggiorna la versione più recente del pacchetto Sales Connect e installa i pulsanti di azione collettiva nella visualizzazione lead/contatti. [Fai clic qui per le istruzioni](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf).

>[!NOTE]
>
>Prima di seguire i passaggi seguenti, assicurati di aver effettuato l&#39;accesso al tuo account Marketo Sales Connect.

## E-mail in blocco {#bulk-email}

1. In Salesforce, fai clic sul pulsante **Lead** , quindi scegli l’elenco dei lead desiderati.

   ![](assets/one-6.png)

   >[!NOTE]
   >
   >Se ti trovi già nell’elenco che utilizzerai, dovrai eseguirlo nuovamente scegliendo dal menu a discesa per assicurarti che vengano visualizzati i pulsanti di azione di massa MSC. Questo è il comportamento di Salesforce che non può essere modificato.

1. Fai clic sull’elenco a discesa della freccia (all’estrema destra dello schermo) e seleziona **Email con MSC**.

   ![](assets/two-6.png)

1. Verrà visualizzata un&#39;e-mail MSC. Include le seguenti funzionalità:

   a) Il campo &quot;A&quot; mostra &quot;Tutte le entrate&quot;, corrispondente all’elenco di lead scelto nella vista Elenco lead\
   b) Questo elenco è visibile nel pannello a sinistra denominato &quot;Composizione in blocco&quot; - è possibile aggiungere/rimuovere i destinatari qui\
   c. Puoi scegliere un modello o creare un tuo indirizzo e-mail\
   d. Puoi inviare l’e-mail immediatamente o pianificare l’invio in un secondo momento

   ![](assets/three-5.png)

## Aggiungi a Campaign {#add-to-campaign}

1. In Salesforce, fai clic sul pulsante **Lead** , quindi scegli l’elenco dei lead desiderati.

   ![](assets/four-4.png)

1. Fai clic sull’elenco a discesa della freccia (all’estrema destra dello schermo) e seleziona **Aggiungi alla campagna MSC**.

   ![](assets/five-4.png)

1. Verrà visualizzato un pop-up &quot;Aggiungi persone alla tua campagna&quot;. Fai clic su **Successivo** e passa attraverso il flusso tipico della campagna per attivare una campagna MSC.

   ![](assets/six-1.png)

## Invia a Marketo Sales Connect {#push-to-marketo-sales-connect}

1. In Salesforce, fai clic sul pulsante **Lead** , quindi scegli l’elenco dei lead desiderati.

   ![](assets/seven-2.png)

1. Fai clic sull’elenco a discesa della freccia (all’estrema destra dello schermo) e seleziona **Spingi a MSC**.

   ![](assets/eight-2.png)

1. Viene aperta una nuova scheda denominata &quot;Salesforce Bridge&quot;. Fai clic sul pulsante **Procedi al gruppo →** pulsante .

   ![](assets/nine-2.png)

1. Verrai inviato al tuo account MSC dove vedrai un gruppo creato con data/ora. Riceverai una notifica al termine della sincronizzazione e il gruppo includerà i lead sincronizzati da Salesforce.

   ![](assets/ten-1.png)

>[!NOTE]
>
>È possibile seguire gli stessi passaggi per utilizzare azioni in blocco anche nella visualizzazione elenco contatti.

>[!MORELIKETHIS]
>
>* [Invio di e-mail tramite e-mail di gruppo](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [Composizione di e-mail in blocco con Seleziona e Invia](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)

