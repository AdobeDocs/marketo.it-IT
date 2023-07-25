---
unique-page-id: 14352482
description: Funzionamento del tracciamento delle risposte - Documentazione di Marketo - Documentazione del prodotto
title: Funzionamento del tracciamento delle risposte
exl-id: 8d087014-99b7-47ba-9f08-95b13bc16438
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---

# Funzionamento del tracciamento delle risposte {#how-reply-tracking-works}

Il tracciamento delle risposte viene eseguito osservando un ID messaggio presente in ogni e-mail inviata. Ogni e-mail contiene un ID messaggio univoco che ci consente di avere alcuni dei migliori tracciamenti delle risposte in giro.

>[!PREREQUISITES]
>
>**Connessione con il server e-mail:** Sales Connect deve essere collegato alla tua casella in entrata in modo da sapere quando è arrivata una nuova risposta. È necessario disporre dell&#39;account Sales Connect [connesso a Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md). Se si utilizza Outlook, sarà necessario eseguire l&#39;integrazione con [server exchange](https://toutapp.com/next#settings/exchange_settings).

Se Sales Connect non riesce a tenere traccia della risposta del potenziale cliente all&#39;e-mail, non potrà interrompere una campagna basata sul rilevamento delle risposte o registrare la risposta a Salesforce.  Cosa significa che un indirizzo e-mail può rispondere?

Ciò significa che se invii un’e-mail a flynn@flynnsarcade.com e lui risponde con kevinf@flynnsarcade.com, saremo in grado di tenere traccia della risposta. Inoltre, se invii un’e-mail a flynn@flynnsarcade.com e CC alan@encom.com e Alan ti risponde, la risposta verrà rilevata e la campagna verrà terminata.
