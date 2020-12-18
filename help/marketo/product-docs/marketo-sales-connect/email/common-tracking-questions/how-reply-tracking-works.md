---
unique-page-id: 14352482
description: Come funziona il tracciamento delle risposte - Documenti Marketo - Documentazione del prodotto
title: Come funziona il tracciamento delle risposte
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# Funzionamento del tracciamento delle risposte {#how-reply-tracking-works}

Il tracciamento delle risposte viene effettuato osservando un ID messaggio presente in ogni e-mail inviata. Ogni e-mail contiene un ID messaggio univoco che ci consente di ottenere il miglior tracciamento delle risposte.

>[!PREREQUISITES]
>
>**Connessione con Email Server:** Sales Connect deve essere connesso alla inbox in modo da sapere quando è arrivata una nuova risposta. Dovrai avere il tuo account di vendita Connect [collegato a Gmail](http://docs.marketo.com/x/kYMOAQ). Se usi Outlook, è necessario integrare il tuo [server di scambio](http://toutapp.com/next#settings/exchange_settings).

Se Sales Connect non è in grado di tenere traccia della risposta del cliente potenziale all&#39;e-mail, non sarà in grado di interrompere una campagna in base al rilevamento delle risposte o al registro che risponde a Salesforce.  Cosa intendiamo per indirizzo email che può rispondere?

Ciò significa che se si invia un&#39;e-mail [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#783217162b16170f3830170d0b1d2b0c190a13561b1715) e risponde con [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#c08aafae93aeafb78094a8a58ea9a7a8b4b397a1b4a3a8eea3afad), sarà possibile tenere traccia della risposta. Inoltre, se invii tramite e-mail [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#450f2a2b162b2a32050d2a303620163124372e6b262a28) e CC [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#3e5f525f507e5b505d5153105d5153) e Alan ti riscrive, verrà anche rilevata la risposta e la fine della campagna.
