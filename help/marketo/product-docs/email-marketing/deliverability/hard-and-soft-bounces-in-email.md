---
unique-page-id: 1147328
description: Bounts rigidi e morbidi in e-mail - Marketo Docs - Documentazione prodotto
title: Punti rigidi e morbidi nell'e-mail
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---


# Punti rigidi e morbidi nell&#39;e-mail {#hard-and-soft-bounces-in-email}

Un rimbalzo duro può rendere non valido l&#39;indirizzo e-mail di una persona quando un server di posta elettronica dice a Marketo che l&#39;e-mail della persona non può essere recapitata. Un rimbalzo morbido significa che qualcosa è andato storto nel consegnare l&#39;e-mail alla persona; questo viene automaticamente risolto e a volte può richiedere giorni. I rimbalzi rigidi e morbidi sono costituiti da [più categorie](http://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838).

>[!NOTE]
>
>**FYI**
>
>Marketo sta ora standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che l&#39;iscrizione contenga lead/lead e la persona/persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

## Classificazione rimbalzo {#bounce-classification}

Ci sono 5 stringhe di persona in Marketo correlate alla consegna delle e-mail con problemi.

1. **E-mail sospesa** - Impostata su True quando si verifica un certo tipo di rimbalzo rigido.
1. **Causa** e-mail sospesa - Ci possono essere molti motivi. Questo campo cerca di spiegare la causa.
1. **E-mail sospesa a **- Quando si verifica il rimbalzo offensivo, Marketo sospenderà la spedizione alla persona per 24 ore da questa marca temporale.
1. **E-mail non valida** - Impostata su True quando si verifica un certo tipo di rimbalzo rigido.
1. **Causa** non valida e-mail - Motivo del rimbalzo rigido.

>[!NOTE]
>
>Quando una persona raggiunge lo stato di sospensione **dell’** e-mail, non è possibile deselezionare la casella di controllo dell’e-mail sospesa. Tuttavia, la persona sarà ancora disponibile alla posta 24 ore dopo la sospensione iniziale.
>
>Quando una persona è contrassegnata come **e-mail non valida**, può essere reimpostata solo manualmente (cosa che consigliamo di fare solo se si sa per certo che la sua e-mail è valida) deselezionando la casella &quot;E-mail non valida&quot; nella scheda Informazioni persona del record.

>[!NOTE]
>
>**Prerequisiti**
>
>Segui [questi passaggi](../../../product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) per creare un report sulle prestazioni dell&#39;e-mail, che genererà dati di rimbalzo.

Dopo aver creato il report sulle prestazioni dell&#39;e-mail, lo schermo dovrebbe essere simile al seguente: ![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>I filtri anti-spam a volte generano dei rimbalzi duri. Questi &quot;falsi positivi&quot; non indicano la validità effettiva dell&#39;indirizzo e-mail della persona.

