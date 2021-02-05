---
unique-page-id: 1147328
description: Bounts rigidi e morbidi in e-mail - Marketo Docs - Documentazione prodotto
title: Punti rigidi e morbidi nell'e-mail
translation-type: tm+mt
source-git-commit: 615ddd6ffdb3873baa159d440db7b24f3a07e6b0
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---


# Punti rigidi e morbidi nell&#39;e-mail {#hard-and-soft-bounces-in-email}

Un rimbalzo duro può rendere non valido l&#39;indirizzo e-mail di una persona quando un server di posta elettronica dice a Marketo che l&#39;e-mail della persona non può essere recapitata. Un rimbalzo morbido significa che qualcosa è andato storto nel consegnare l&#39;e-mail alla persona; questo viene automaticamente risolto e a volte può richiedere giorni. I rimbalzi rigidi e morbidi sono costituiti da [categorie multiple](https://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838).

## Classificazione rimbalzi {#bounce-classification}

Ci sono 5 stringhe di persona in Marketo correlate alla consegna delle e-mail con problemi.

1. **E-mail sospesa**  - Impostata su True quando si verifica un certo tipo di rimbalzo rigido.
1. **Causa**  sospensione e-mail - Ci possono essere molti motivi. Questo campo cerca di spiegare la causa.
1. **E-mail sospesa a**  - Quando si verifica il rimbalzo offensivo, Marketo sospenderà la spedizione alla persona per 24 ore da questa marca temporale.
1. **E-mail non valida**  - Impostata su True quando si verifica un certo tipo di rimbalzo rigido.
1. **Causa**  non valida e-mail - Motivo del rimbalzo rigido.

>[!NOTE]
>
>Dopo che una persona ha raggiunto lo stato **email sospesa**, non c&#39;è modo di cancellare la casella di controllo email sospesa. Tuttavia, la persona sarà ancora disponibile alla posta 24 ore dopo la sospensione iniziale.
>
>Quando una persona è contrassegnata come **email non valido**, può essere reimpostata solo manualmente (cosa che si consiglia di fare solo se si sa per certo che il suo indirizzo e-mail è valido) deselezionando la casella &quot;E-mail non valida&quot; nella scheda Informazioni persona del record.

>[!PREREQUISITES]
>
>Seguite [questi passaggi](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) per creare un report sulle prestazioni dell&#39;e-mail che genererà dati di rimbalzo.

Dopo aver creato il report sulle prestazioni dell&#39;e-mail, lo schermo dovrebbe essere simile al seguente:

![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>I filtri anti-spam a volte generano dei rimbalzi duri. Questi &quot;falsi positivi&quot; non indicano la validità effettiva dell&#39;indirizzo e-mail della persona.
