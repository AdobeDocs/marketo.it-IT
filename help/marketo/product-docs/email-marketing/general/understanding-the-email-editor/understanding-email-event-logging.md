---
unique-page-id: 1147356
description: Informazioni sulla registrazione degli eventi e-mail - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni sulla registrazione degli eventi e-mail
exl-id: 107d7f4a-ad38-44e4-95d8-760539aacede
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 1%

---

# Informazioni sulla registrazione degli eventi e-mail {#understanding-email-event-logging}

Quando si inviano le e-mail, Marketo registra diversi punti dati nei registri attività della persona. Ecco quelli di base.

| Evento | Descrizione |
|---|---|
| Inviato | Viene registrato ogni volta che un’e-mail viene inviata dai server Marketo, indipendentemente dal fatto che venga effettivamente consegnata. Le e-mail non recapitate vengono ancora registrate come &quot;Inviate&quot;. |
| Consegnato | Viene registrato ogni volta che un messaggio e-mail viene accettato dal server di posta del destinatario. Ciò non significa che abbia evitato i filtri anti-spam. Può essere presente solo 1 consegna per ogni e-mail inviata. |
| Rifiuto rigido | Alcuni mancati recapiti permanenti sono il risultato di blocchi di spam, quindi non proveremo a inviare un’e-mail a quella persona per 24 ore in alcuna campagna. Altre mancate consegne permanenti, come caselle in entrata inesistenti, non verranno mai più inviate via e-mail alla persona da alcuna campagna. |
| Rimbalzo morbido | Viene registrato quando la risposta di un server non è chiara, la cassetta postale è piena o si verificano problemi generali del server. Queste persone vengono sottoposte a una logica di ripetizione dei tentativi per 24-36 ore per una potenziale consegna futura. Ciò non esclude la persona da altre comunicazioni. |
| Aperto | Viene registrato quando un destinatario visualizza un’e-mail con immagini NON bloccate. Viene registrato un solo evento aperto per e-mail, per persona, per campagna avanzata. Se aprono la stessa e-mail dalla casella in entrata due volte, non verrà registrata più di una volta. |
| Clic effettuato | Viene registrato ogni volta che un URL decorato dell’e-mail viene caricato nel browser (il risultato è stato clic sul collegamento). Di solito si tratta del clic del destinatario, ma può anche essere un taglia/incolla. |
| Annulla l&#39;iscrizione | Viene registrato quando una persona fa clic sul collegamento di annullamento dell’abbonamento di un’e-mail e invia il modulo di annullamento dell’abbonamento. |

>[!CAUTION]
>
>Se la stessa e-mail viene inviata due volte alla stessa persona dalla stessa campagna, il **Aperto** l&#39;evento verrà registrato al massimo 1 volta.
