---
unique-page-id: 14352482
description: Funzionamento del tracciamento delle risposte - Documentazione di Marketo - Documentazione del prodotto
title: Funzionamento del tracciamento delle risposte
exl-id: 8d087014-99b7-47ba-9f08-95b13bc16438
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---

# Funzionamento del tracciamento delle risposte {#how-reply-tracking-works}

Il tracciamento delle risposte viene eseguito osservando un ID messaggio presente in ogni e-mail inviata. Ogni e-mail contiene un ID messaggio univoco che ci consente di avere alcuni dei migliori tracciamenti delle risposte in giro.

>[!PREREQUISITES]
>
>**Connessione al server e-mail:** [!DNL Sales Connect] deve essere connessa alla tua casella in entrata in modo da sapere quando è arrivata una nuova risposta. Devi avere il tuo account [!DNL Sales Connect] [connesso a Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md). Se utilizzi [!DNL Outlook], dovremo integrarlo con il tuo [server Exchange](https://toutapp.com/next#settings/exchange_settings).

Se [!DNL Sales Connect] non riesce a tenere traccia della risposta del potenziale cliente all&#39;e-mail, non potrà interrompere una campagna basata sul rilevamento delle risposte o registrare la risposta a [!DNL Salesforce].  Cosa significa che un indirizzo e-mail può rispondere?

Ciò significa che se invii un’e-mail a flynn@flynnsarcade.com e lui risponde con kevinf@flynnsarcade.com, saremo in grado di tenere traccia della risposta. Inoltre, se invii un’e-mail a flynn@flynnsarcade.com e CC alan@encom.com e Alan ti risponde, la risposta verrà rilevata e la campagna verrà terminata.
