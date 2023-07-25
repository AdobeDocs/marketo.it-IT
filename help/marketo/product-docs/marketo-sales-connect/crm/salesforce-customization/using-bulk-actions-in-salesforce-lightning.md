---
unique-page-id: 42762825
description: Utilizzo di azioni in blocco in Salesforce Lightning - Documenti Marketo - Documentazione del prodotto
title: Utilizzo di azioni in blocco in Salesforce Lightning
exl-id: 72022507-6568-4cc2-b3b5-c1703a1493ad
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Utilizzo di azioni in blocco in Salesforce Lightning {#using-bulk-actions-in-salesforce-lightning}

Scopri come eseguire azioni in blocco, come l’aggiunta di lead a una campagna, l’invio di un’e-mail in blocco o il push di lead da Salesforce a Sales Connect.

>[!PREREQUISITES]
>
>Aggiornare alla versione più recente del pacchetto Sales Connect e installare i pulsanti di azione collettiva nella vista lead/contatto. [Fare clic qui per istruzioni](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf).

>[!NOTE]
>
>Prima di eseguire la procedura seguente, verificare di aver effettuato l&#39;accesso al proprio account Marketo Sales Connect.

## E-mail in blocco {#bulk-email}

1. In Salesforce, fai clic su **Lead** , quindi scegli l’elenco dei lead desiderati.

   ![](assets/one-6.png)

   >[!NOTE]
   >
   >Se sei già presente nell’elenco che utilizzerai, dovrai eseguirlo nuovamente scegliendolo dall’elenco a discesa per assicurarti che vengano visualizzati i pulsanti delle azioni in blocco MSC. Questo è un comportamento di Salesforce che non può essere modificato.

1. Fai clic sul menu a discesa della freccia (all’estrema destra dello schermo) e seleziona **E-mail con MSC**.

   ![](assets/two-6.png)

1. Verrà visualizzata un&#39;e-mail MSC. Include le seguenti funzionalità:

   a. Il campo &quot;A&quot; mostra &quot;Tutte le ricezioni&quot;, che corrisponde all&#39;elenco di lead scelti nella vista Elenco lead\
   b. Questo elenco è visibile nel pannello a sinistra denominato &quot;Composizione in blocco&quot;. Qui puoi aggiungere/rimuovere i destinatari\
   c. Puoi scegliere un modello o creare un messaggio e-mail personalizzato\
   d. Puoi inviare l’e-mail immediatamente o pianificare l’invio in un secondo momento

   ![](assets/three-5.png)

## Aggiungi a campagna {#add-to-campaign}

1. In Salesforce, fai clic su **Lead** , quindi scegli l’elenco dei lead desiderati.

   ![](assets/four-4.png)

1. Fai clic sul menu a discesa della freccia (all’estrema destra dello schermo) e seleziona **Aggiungi a campagna MSC**.

   ![](assets/five-4.png)

1. Viene visualizzata la finestra a comparsa Aggiungi persone alla campagna. Clic **Successivo** e segui il flusso tipico delle campagne per attivare una campagna MSC.

   ![](assets/six-1.png)

## Invia a Marketo Sales Connect {#push-to-marketo-sales-connect}

1. In Salesforce, fai clic su **Lead** , quindi scegli l’elenco dei lead desiderati.

   ![](assets/seven-2.png)

1. Fai clic sul menu a discesa della freccia (all’estrema destra dello schermo) e seleziona **Invia a MSC**.

   ![](assets/eight-2.png)

1. Si aprirà una nuova scheda denominata &quot;Ponte Salesforce&quot;. Fai clic su **Procedi al → di gruppo** pulsante.

   ![](assets/nine-2.png)

1. Verrai indirizzato al tuo account MSC, dove vedrai un gruppo creato con data/ora. Riceverai una notifica una volta completata la sincronizzazione e il gruppo includerà i lead sincronizzati da Salesforce.

   ![](assets/ten-1.png)

>[!NOTE]
>
>È possibile seguire gli stessi passaggi per utilizzare azioni in blocco anche nella visualizzazione elenco contatti.

>[!MORELIKETHIS]
>
>* [Invio di e-mail tramite e-mail gruppo](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [Composizione di e-mail in blocco con Seleziona e invia](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)
