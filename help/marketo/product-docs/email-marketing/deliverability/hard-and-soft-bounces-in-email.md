---
unique-page-id: 1147328
description: Bounge rigidi e morbidi in e-mail - Marketo Docs - Documentazione del prodotto
title: Rimbalzi rigidi e morbidi nell’e-mail
exl-id: 53298562-76b6-473a-bf9f-2bec682f4d35
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Rimbalzi rigidi e morbidi nell’e-mail {#hard-and-soft-bounces-in-email}

Un messaggio non recapitato può rendere non valido l&#39;indirizzo e-mail di una persona quando un server di posta elettronica indica a Marketo che l&#39;e-mail della persona non può essere recapitata. Un messaggio non recapitato significa che si è verificato un errore nella consegna dell’e-mail alla persona; questo viene automaticamente risolto e a volte può richiedere giorni. Sia i rimbalzi rigidi che quelli morbidi consistono in [categorie multiple](https://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838).

## Classificazione non recapitata {#bounce-classification}

In Marketo sono presenti 5 stringhe di persone correlate alla consegna delle e-mail con problemi.

1. **E-mail sospesa** - Impostare su True quando si verifica un certo tipo di rimbalzo rigido.
1. **Causa sospensione e-mail** - Ci possono essere molte ragioni. Questo campo cerca di spiegare la causa.
1. **E-Mail Sospesa A** - Quando si verifica il messaggio non recapitato, Marketo sospenderà l&#39;invio alla persona per 24 ore da questa marca temporale.
1. **E-mail non valida** - Impostare su True quando si verifica un certo tipo di rimbalzo rigido.
1. **Causa non valida dell&#39;e-mail** - La ragione del rimbalzo duro.

>[!NOTE]
>
>Dopo che una persona ha raggiunto **e-mail sospesa** stato , non è possibile deselezionare la casella di controllo dell’e-mail sospesa. Tuttavia, la persona diventerà ancora disponibile 24 ore dopo la sospensione iniziale.
>
>Quando una persona è contrassegnata come **email non valida**, possono essere reimpostate solo manualmente (cosa che consigliamo di fare solo se sai che la loro e-mail è valida) deselezionando la casella &quot;E-mail non valida&quot; nella scheda Informazioni persona del record.

>[!PREREQUISITES]
>
>Segui [questi passaggi](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) per creare un rapporto sulle prestazioni di e-mail, che genererà dati non recapitati.

Dopo aver creato il rapporto sulle prestazioni delle e-mail, la schermata dovrebbe avere un aspetto simile al seguente:

![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>I filtri anti-spam a volte generano rimbalzi duri. Questi &quot;falsi positivi&quot; non sono un&#39;indicazione della vera validità dell&#39;indirizzo e-mail della persona.
