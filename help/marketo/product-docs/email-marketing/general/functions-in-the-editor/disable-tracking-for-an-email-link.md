---
unique-page-id: 1900579
description: Disabilita tracciamento per un collegamento e-mail - Documentazione di Marketo - Documentazione del prodotto
title: Disattiva tracciamento per un collegamento e-mail
exl-id: 841ef605-1664-4457-bc83-50bbe5d44853
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Disattiva tracciamento per un collegamento e-mail {#disable-tracking-for-an-email-link}

A volte è meglio non abilitare **URL di tracciamento Marketo** su un collegamento in un messaggio e-mail. Questa funzione è utile quando la pagina di destinazione non supporta i parametri URL e può causare il mancato funzionamento del collegamento.

1. Seleziona l’e-mail e fai clic su **Modifica bozza**.

   ![](assets/one-7.png)

1. Fare doppio clic sulla sezione modificabile che contiene il collegamento.

   ![](assets/two-6.png)

1. Fai clic sul collegamento in questione, quindi fai clic su **Inserisci/Modifica collegamento** pulsante.

   ![](assets/three-6.png)

1. Nella finestra a comparsa Modifica collegamento, deseleziona **Traccia collegamento** casella di controllo.

   ![](assets/four-4.png)

1. Noterai la **Casella Includi _token** scompare. Clic **Applica**.

   ![](assets/five-3.png)

   >[!TIP]
   >
   >Deseleziona solo **Includi _token di marketing** consentirà comunque il tracciamento del collegamento, ma dopo il reindirizzamento, l’URL di destinazione non includerà il parametro della stringa di query mkt_tok. Questo parametro viene utilizzato dalle pagine di destinazione di Marketo e da Munchkin per garantire il corretto tracciamento delle attività della persona (come quando una persona annulla l’iscrizione a un’e-mail). È consigliabile evitare di utilizzare questa funzione a meno che non si verifichi un comportamento strano sul sito web a causa della presenza del parametro.

1. Clic **Salva**.

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!TIP]
   >
   >Desideri disabilitare il tracciamento dei clic per un collegamento in un messaggio e-mail **modello**? Usa questo formato:
   >`<a class="mktNoTrack" href="https://www.mywebsite.com">This link does not have tracking</a>`\
   >Se hai bisogno di aiuto per implementare questo, consulta il tuo sviluppatore web.

Bello! Hai disabilitato il tracciamento di un collegamento.
