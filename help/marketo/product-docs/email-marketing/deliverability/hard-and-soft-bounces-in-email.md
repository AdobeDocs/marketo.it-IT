---
unique-page-id: 1147328
description: Mancati recapiti permanenti e non permanenti nelle e-mail - Documentazione di Marketo - Documentazione di prodotto
title: Mancati recapiti permanenti e non permanenti nelle e-mail
exl-id: 53298562-76b6-473a-bf9f-2bec682f4d35
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Mancati recapiti permanenti e non permanenti nelle e-mail {#hard-and-soft-bounces-in-email}

Un messaggio non recapitato può rendere non valido l’indirizzo e-mail di una persona quando un server di posta comunica a Marketo che l’e-mail della persona non può essere consegnata. Un mancato recapito non permanente indica che si è verificato un errore durante la consegna dell’e-mail alla persona. L’errore si risolve automaticamente e a volte può richiedere alcuni giorni. I mancati recapiti permanenti e non permanenti sono costituiti da [più categorie](https://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838).

## Classificazione per mancato recapito {#bounce-classification}

In Marketo sono presenti 5 stringhe di persone correlate alla consegna di e-mail con problemi.

1. **E-mail sospesa** : impostato su True quando si verifica un determinato tipo di mancati recapiti permanenti.
1. **Causa e-mail sospesa** - Le ragioni possono essere molteplici. Questo campo cerca di spiegare la causa.
1. **E-mail sospesa alle** - Quando si verifica il mancato recapito, Marketo sospenderà l’invio di e-mail alla persona per 24 ore da questa marca temporale.
1. **E-mail non valida** : impostato su True quando si verifica un determinato tipo di mancati recapiti permanenti.
1. **Causa e-mail non valida** - Il motivo dell’hard bounce.

>[!NOTE]
>
>Dopo che una persona raggiunge **e-mail sospesa** stato, non è possibile deselezionare la casella di controllo e-mail sospesa. Tuttavia, la persona sarà ancora disponibile per la posta 24 ore dopo la sospensione iniziale.
>
>Quando una persona è contrassegnata come **e-mail non valida**, possono essere reimpostate solo manualmente (operazione che consigliamo di eseguire solo se si è certi che l’e-mail sia valida) deselezionando la casella &quot;E-mail non valida&quot; nella scheda Informazioni persona del record.

>[!PREREQUISITES]
>
>Segui [questi passaggi](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) per creare un rapporto sulle prestazioni delle e-mail che genererà i dati non recapitati.

Dopo aver creato il rapporto sulle prestazioni delle e-mail, lo schermo dovrebbe essere simile al seguente:

![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>I filtri anti-spam a volte creano mancati recapiti permanenti. Questi &quot;falsi positivi&quot; non sono un’indicazione della vera validità dell’indirizzo e-mail della persona.
