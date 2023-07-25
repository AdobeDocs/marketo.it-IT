---
description: Verifica annullamento iscrizione Marketo - Documentazione Marketo - Documentazione del prodotto
title: Verifica annullamento iscrizione Marketo
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 0%

---

# Verifica annullamento iscrizione Marketo {#marketo-unsubscribe-check}

Il controllo per annullare l’abbonamento a Marketo utilizza la connessione del tuo team a Marketo per impedire che le e-mail arrivino a persone non abbonate nel sistema di gestione dei lead di Marketo. Quando un utente di vendita invia un’e-mail con Marketo Sales, viene effettuata una chiamata API a Marketo per verificare se l’ID e-mail non è abbonato. In caso affermativo, l’e-mail non verrà inviata.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Attivazione {#turning-it-on}

1. Fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/marketo-unsubscribe-check-1.png)

1. In Impostazioni amministrazione, fai clic su **Annulla iscrizione**.

   ![](assets/marketo-unsubscribe-check-2.png)

1. Fai clic su **Integrazioni** scheda. Nella sezione Marketo Unsubscribe Check, fai clic sul cursore per attivare il controllo.

   ![](assets/marketo-unsubscribe-check-3.png)

## Aspetti da considerare {#things-to-know}

Controllo per annullare l’abbonamento a Marketo...

* Non viene conteggiato rispetto ai limiti API
* Richiede la connessione a Marketo
* È un’impostazione globale
* Blocca le e-mail inviate dall’applicazione web, dai client e-mail e da Salesforce
