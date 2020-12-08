---
unique-page-id: 1900579
description: Disattiva tracciamento per un collegamento e-mail - Documenti Marketo - Documentazione prodotto
title: Disattiva tracciamento per un collegamento e-mail
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---


# Disattiva tracciamento per un collegamento e-mail {#disable-tracking-for-an-email-link}

A volte non si desidera attivare l’URL **di tracciamento** marketing su un collegamento presente in un messaggio e-mail. Questa funzione è utile quando la pagina di destinazione non supporta i parametri dell’URL e potrebbe causare un collegamento interrotto.

>[!NOTE]
>
>Marketo sta standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che nell&#39;abbonamento siano presenti lead/lead e persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](/help/marketo/getting-started/updates-to-marketo-terminology.md)informazioni.

1. Selezionate il messaggio e-mail e fate clic su **Modifica** **bozza**.

   ![](assets/one-7.png)

1. Fare doppio clic sulla sezione modificabile che contiene il collegamento.

   ![](assets/two-6.png)

1. Fate clic sul collegamento in questione, quindi fate clic sul pulsante **Inserisci/Modifica collegamento** .

   ![](assets/three-6.png)

1. Nella finestra a comparsa Modifica collegamento, deselezionate la casella di controllo **Traccia collegamento** .

   ![](assets/four-4.png)

1. Noterete che la casella **Includi mkt_tok** scompare. Fate clic su **Applica**.

   ![](assets/five-3.png)

   >[!TIP]
   >
   >Se si deseleziona solo **Includi mkt_tok** , il tracciamento del collegamento continuerà, ma dopo il reindirizzamento l&#39;URL di destinazione non includerà il parametro della stringa di query mkt_tok. Questo parametro viene utilizzato da Marketo Landing Pages e Munchkin per garantire il corretto tracciamento delle attività delle persone (come nel caso in cui una persona annulla la sottoscrizione da un&#39;e-mail). È consigliabile evitare di utilizzare questa funzione a meno che non si verifichino comportamenti strani sul sito Web a causa della presenza del parametro.

1. Fate clic su **Salva**.

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!TIP]
   >
   >Disabilitare il tracciamento dei clic per un collegamento in un **modello**e-mail? Utilizzate questo formato:
   >`<a class="mktNoTrack" href="http://www.mywebsite.com">This link does not have tracking</a>`\
   >Se avete bisogno di aiuto per l&#39;implementazione di questo progetto, rivolgetevi al vostro sviluppatore Web.

Bello! Ora hai disattivato il tracciamento per un collegamento.
