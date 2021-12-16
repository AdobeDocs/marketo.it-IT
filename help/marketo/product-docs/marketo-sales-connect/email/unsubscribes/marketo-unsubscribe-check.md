---
unique-page-id: 18317340
description: Controllo dell’annullamento dell’abbonamento a Marketo - Documenti Marketo - Documentazione del prodotto
title: Controllo dell’annullamento dell’abbonamento a Marketo
exl-id: b8bd5b38-a4f5-4ac7-a5ce-a155fce57998
source-git-commit: 82c75d52caf3a0320cd3e8534b3b0870cf12d660
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---

# Controllo dell’annullamento dell’abbonamento a Marketo {#marketo-unsubscribe-check}

Il controllo per l’annullamento dell’abbonamento a Marketo utilizza la connessione del tuo team a Marketo per impedire che le e-mail inviate a persone che non sono abbonate al sistema Marketo Lead Management. Quando un utente di vendita invia un&#39;e-mail con Sales Connect, viene effettuata una chiamata API a Marketo per verificare se l&#39;ID e-mail è annullato. Se lo è, impediremo l’invio dell’e-mail.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Attiva {#turning-it-on}

1. Nell’applicazione web, fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/one-2.png)

1. In Impostazioni amministratore, fai clic su **Annulla sottoscrizione**.

   ![](assets/two-3.png)

1. Fai clic su **Integrazioni**.

   ![](assets/three-3.png)

1. Nella sezione Controllo annullamento sottoscrizione Marketo , fai clic sul cursore per attivare il controllo.

   ![](assets/four-2.png)

## Cose da sapere {#things-to-know}

Controllo di annullamento sottoscrizione Marketo..

* Non viene conteggiato rispetto ai limiti delle API
* Richiede l&#39;installazione di una connessione Marketo
* È un’impostazione globale
* Blocca le e-mail inviate dall’applicazione web, dai client e-mail e da Salesforce
* Registra un&#39;e-mail non riuscita o impedisce a un utente di inviarla quando tenta di inviare per tutti i flussi di lavoro (invio del plugin e-mail, invio individuale, invio della campagna di vendita, selezione e invio multipli) tranne che per [e-mail di gruppo](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md), in cui impediremo l’invio silenzioso delle e-mail
