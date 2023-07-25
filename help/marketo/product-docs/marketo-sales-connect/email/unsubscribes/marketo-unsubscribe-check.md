---
unique-page-id: 18317340
description: Verifica annullamento iscrizione Marketo - Documentazione Marketo - Documentazione del prodotto
title: Verifica annullamento iscrizione Marketo
exl-id: b8bd5b38-a4f5-4ac7-a5ce-a155fce57998
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---

# Verifica annullamento iscrizione Marketo {#marketo-unsubscribe-check}

Il controllo per annullare l’abbonamento a Marketo utilizza la connessione del tuo team a Marketo per impedire che le e-mail arrivino a persone non abbonate nel sistema di gestione dei lead di Marketo. Quando un utente di vendita invia un’e-mail con Sales Connect, viene effettuata una chiamata API a Marketo per verificare se l’ID e-mail non è abbonato. In caso affermativo, l’e-mail non verrà inviata.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Attivazione {#turning-it-on}

1. Nell’applicazione web, fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/one-2.png)

1. In Impostazioni amministrazione, fai clic su **Annulla iscrizione**.

   ![](assets/two-3.png)

1. Clic **Integrazioni**.

   ![](assets/three-3.png)

1. Nella sezione Marketo Unsubscribe Check, fai clic sul cursore per attivare il controllo.

   ![](assets/four-2.png)

## Aspetti da considerare {#things-to-know}

Controllo per annullare l’abbonamento a Marketo...

* Non viene conteggiato rispetto ai limiti API
* Richiede la connessione a Marketo
* È un’impostazione globale
* Blocca le e-mail inviate dall’applicazione web, dai client e-mail e da Salesforce
* Registra un’e-mail non riuscita o impedisce a un utente di inviare quando tenta di inviare per tutti i flussi di lavoro (invio del plug-in e-mail, invio individuale, invio della campagna di vendita, selezione e invio multipli) ad eccezione di [raggruppa e-mail](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md), in cui impediremo l’invio silenzioso delle e-mail
