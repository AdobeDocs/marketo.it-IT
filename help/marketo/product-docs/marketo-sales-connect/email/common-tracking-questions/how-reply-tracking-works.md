---
unique-page-id: 14352482
description: Come funziona il tracciamento delle risposte - Documenti Marketo - Documentazione del prodotto
title: Come funziona il tracciamento delle risposte
translation-type: tm+mt
source-git-commit: 073b73255d49f859c32c8b4793e6798f02f7a5c4
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# Funzionamento del tracciamento delle risposte {#how-reply-tracking-works}

Il tracciamento della risposta viene eseguito guardando un ID messaggio presente in ogni e-mail inviata. Ogni e-mail contiene un ID messaggio univoco che ci consente di ottenere uno dei migliori risultati di tracciamento delle risposte.

>[!PREREQUISITES]
>
>**Connessione con Email Server:** è necessario collegare Sales Connect alla Posta in arrivo in modo da sapere quando è arrivata una nuova risposta. Sarà necessario che il tuo account di vendita Connect [sia collegato a Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md). Se utilizzi Outlook, sarà necessario eseguire l&#39;integrazione con il [server di scambio](https://toutapp.com/next#settings/exchange_settings).

Se Sales Connect non è in grado di tenere traccia della risposta del potenziale cliente all&#39;e-mail, non sarà in grado di interrompere una campagna in base al rilevamento delle risposte o al registro che risponde a Salesforce.  Cosa intendiamo per indirizzo e-mail che può rispondere?

Ciò significa che se invii un&#39;e-mail a flynn@flynnsarcade.com e risponde con kevinf@flynnsarcade.com, saremo in grado di tenere traccia della risposta. Inoltre, se invii un&#39;e-mail a flynn@flynnsarcade.com e CC alan@encom.com e Alan ti scrive di nuovo, rileverà anche la risposta e terminerà la campagna.
