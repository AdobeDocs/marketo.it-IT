---
unique-page-id: 1900579
description: Disabilita tracciamento per un collegamento e-mail - Documentazione di Marketo - Documentazione del prodotto
title: Disattiva tracciamento per un collegamento e-mail
exl-id: 841ef605-1664-4457-bc83-50bbe5d44853
feature: Email Editor
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# Disattiva tracciamento per un collegamento e-mail {#disable-tracking-for-an-email-link}

A volte non è necessario abilitare **URL di tracciamento Marketo** su un collegamento in un messaggio e-mail. Questa funzione è utile quando la pagina di destinazione non supporta i parametri URL e può causare il mancato funzionamento del collegamento.

Inoltre, se un&#39;e-mail è stata inviata più di 365 giorni fa **e** nessuno ha fatto clic su uno dei collegamenti negli ultimi 180 giorni, Marketo Engage elimina la route all&#39;URL dal nostro database, causando l&#39;interruzione del collegamento. Pertanto, se hai bisogno che il collegamento sia permanente, devi disabilitare il tracciamento.

1. Selezionare l&#39;indirizzo di posta elettronica e fare clic su **[!UICONTROL Edit Draft]**.

   ![](assets/one-7.png)

1. Fare doppio clic sulla sezione modificabile che contiene il collegamento.

   ![](assets/two-6.png)

1. Fare clic sul collegamento in questione, quindi sul pulsante **Inserisci/Modifica collegamento**.

   ![](assets/three-6.png)

1. Nella finestra a comparsa Modifica collegamento, deselezionare la casella di controllo **[!UICONTROL Track Link]**.

   ![](assets/four-4.png)

1. Noterai che la casella **[!UICONTROL Include mkt_tok]** scompare. Fai clic su **[!UICONTROL Apply]**.

   ![](assets/five-3.png)

   >[!TIP]
   >
   >Deselezionando solo **Includi mkt_tok** sarà comunque possibile tenere traccia del collegamento, ma dopo il reindirizzamento l&#39;URL di destinazione non includerà il parametro della stringa di query mkt_tok. Questo parametro viene utilizzato dalle pagine di destinazione di Marketo e da Munchkin per garantire il corretto tracciamento delle attività della persona (come quando una persona annulla l’iscrizione a un’e-mail). È consigliabile evitare di utilizzare questa funzione a meno che non si verifichi un comportamento strano sul sito web a causa della presenza del parametro.

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!CAUTION]
   >
   >Se vuoi disabilitare il tracciamento dei clic per un collegamento in un modello e-mail o per la [versione testuale](/help/marketo/product-docs/email-marketing/general/creating-an-email/edit-the-text-version-of-an-email.md){target="_blank"} di un&#39;e-mail, aggiungi `mktNoTrack` all&#39;*inizio* della stringa, non alla fine, come in questo esempio: `<a class="mktNoTrack" href="https://www.mywebsite.com">This link does not have tracking</a>`. In caso contrario, il collegamento potrebbe scomparire. Per assistenza nell’implementazione del codice di cui sopra, consulta il tuo sviluppatore web.
