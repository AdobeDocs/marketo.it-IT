---
unique-page-id: 18317340
description: Controllo dell'annullamento della sottoscrizione Marketo - Documenti Marketo - Documentazione prodotto
title: Controllo annullamento sottoscrizione Marketo
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---


# Controllo annullamento sottoscrizione Marketo {#marketo-unsubscribe-check}

La funzione Marketo Unsubscription Check utilizza la connessione del team a Marketo per impedire che le e-mail arrivino a persone che non hanno effettuato l&#39;iscrizione nel sistema di gestione dei lead di Marketo. Quando un utente di vendita invia un&#39;e-mail con Sales Connect, viene effettuata una chiamata API a Marketo per verificare se l&#39;ID e-mail è stato annullato. In caso affermativo, impediremo l&#39;invio dell&#39;e-mail.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Attivarla {#turning-it-on}

1. Nell’applicazione Web, fate clic sull’icona a forma di ingranaggio e selezionate **Impostazioni**.

   ![](assets/one-2.png)

1. In Impostazioni amministratore, fai clic su **Annulla sottoscrizione**.

   ![](assets/two-3.png)

1. Fate clic su **Integrazioni**.

   ![](assets/three-3.png)

1. Nella sezione Controllo annullamento sottoscrizione marketing, fate clic sul cursore per attivare il controllo.

   ![](assets/four-2.png)

## Cose da sapere {#things-to-know}

Controllo per l&#39;annullamento della sottoscrizione di Marketo...

* Non viene conteggiato rispetto ai limiti API
* Richiede una connessione Marketo
* È un&#39;impostazione globale
* Blocca le e-mail inviate dall’applicazione Web, dai client e-mail e da Salesforce

