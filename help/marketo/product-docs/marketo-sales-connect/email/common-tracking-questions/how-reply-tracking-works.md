---
unique-page-id: 14352482
description: Come funziona il tracciamento delle risposte - Documenti Marketo - Documentazione del prodotto
title: Come funziona il tracciamento delle risposte
exl-id: 8d087014-99b7-47ba-9f08-95b13bc16438
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---

# Come funziona il tracciamento delle risposte {#how-reply-tracking-works}

Il tracciamento della risposta viene eseguito guardando un ID messaggio presente in ogni e-mail inviata. Ogni e-mail contiene un ID messaggio univoco che ci consente di ottenere uno dei migliori risultati di tracciamento delle risposte.

>[!PREREQUISITES]
>
>**Connessione con server e-mail:** È necessario collegare la rete di vendita alla Posta in arrivo in modo da sapere quando è arrivata una nuova risposta. Avrai bisogno del tuo account Sales Connect [connesso a Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md). Se utilizzi Outlook, sarà necessario integrare con [server di scambio](https://toutapp.com/next#settings/exchange_settings).

Se Sales Connect non è in grado di tenere traccia della risposta del potenziale cliente all&#39;e-mail, non sarà in grado di interrompere una campagna in base al rilevamento delle risposte o al registro che risponde a Salesforce.  Cosa intendiamo per indirizzo e-mail che può rispondere?

Ciò significa che se invii un&#39;e-mail a flynn@flynnsarcade.com e risponde con kevinf@flynnsarcade.com, saremo in grado di tenere traccia della risposta. Inoltre, se invii un&#39;e-mail a flynn@flynnsarcade.com e CC alan@encom.com e Alan ti scrive di nuovo, rileverà anche la risposta e terminerà la campagna.
