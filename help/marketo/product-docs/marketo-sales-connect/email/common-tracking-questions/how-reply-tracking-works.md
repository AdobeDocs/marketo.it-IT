---
unique-page-id: 14352482
description: Come funziona il tracciamento delle risposte - Documenti Marketo - Documentazione del prodotto
title: Come funziona il tracciamento delle risposte
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---


# Come funziona il tracciamento delle risposte {#how-reply-tracking-works}

Il tracciamento delle risposte viene effettuato osservando un ID messaggio presente in ogni e-mail inviata. Ogni e-mail contiene un ID messaggio univoco che ci consente di ottenere il miglior tracciamento delle risposte.

>[!NOTE]
>
>**Prerequisiti**
>
>**Connessione con il server e-mail:** È necessario collegare il reparto vendite alla inbox in modo da sapere quando è arrivata una nuova risposta. Dovrai avere il tuo account di vendita Connect [collegato a Gmail](http://docs.marketo.com/x/kYMOAQ). Se si utilizza Outlook, sarà necessario integrare il server [di](http://toutapp.com/next#settings/exchange_settings)Exchange.

Se Sales Connect non è in grado di tenere traccia della risposta del cliente potenziale all&#39;e-mail, non sarà in grado di interrompere una campagna in base al rilevamento delle risposte o al registro che risponde a Salesforce.  Cosa intendiamo per indirizzo email che può rispondere?

Questo significa che se ricevi un&#39;e-mail [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#783217162b16170f3830170d0b1d2b0c190a13561b1715) e risponde con [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#c08aafae93aeafb78094a8a58ea9a7a8b4b397a1b4a3a8eea3afad), saremo in grado di monitorare la risposta. Inoltre, se invii tramite e-mail [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#450f2a2b162b2a32050d2a303620163124372e6b262a28) e CC [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#3e5f525f507e5b505d5153105d5153), e Alan ti riscrive, verrà anche rilevata la risposta e la fine della campagna.
