---
unique-page-id: 14352482
description: Come funziona il tracciamento delle risposte - Documenti Marketo - Documentazione del prodotto
title: Come funziona il tracciamento delle risposte
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# Funzionamento del tracciamento delle risposte {#how-reply-tracking-works}

Il tracciamento delle risposte viene effettuato osservando un ID messaggio presente in ogni e-mail inviata. Ogni e-mail contiene un ID messaggio univoco che ci consente di ottenere il miglior tracciamento delle risposte.

>[!PREREQUISITES]
>
>**Connessione con Email Server:** Sales Connect deve essere connesso alla inbox in modo da sapere quando è arrivata una nuova risposta. Dovrai avere il tuo account di vendita Connect [collegato a Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-tab-for-gmail-users.md). Se usi Outlook, è necessario integrare il tuo [server di scambio](https://toutapp.com/next#settings/exchange_settings).

Se Sales Connect non è in grado di tenere traccia della risposta del cliente potenziale all&#39;e-mail, non sarà in grado di interrompere una campagna in base al rilevamento delle risposte o al registro che risponde a Salesforce.  Cosa intendiamo per indirizzo email che può rispondere?

Questo significa che se si invia un&#39;e-mail a flynn@flynnsarcade.com e risponde con kevinf@flynnsarcade.com, sarà possibile tenere traccia della risposta. Inoltre, se invii un&#39;e-mail a flynn@flynnsarcade.com e CC alan@encom.com e Alan ti riscrive, la risposta verrà rilevata e la campagna verrà terminata.
