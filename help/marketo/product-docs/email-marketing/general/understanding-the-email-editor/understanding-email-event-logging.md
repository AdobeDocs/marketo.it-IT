---
unique-page-id: 1147356
description: Registrazione eventi e-mail - Documenti Marketo - Documentazione prodotto
title: Informazioni sulla registrazione degli eventi tramite e-mail
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---


# Informazioni sulla registrazione degli eventi tramite e-mail {#understanding-email-event-logging}

Quando si inviano e-mail, Marketo registra diversi punti dati nei registri attività della persona. Ecco quelli di base.

>[!NOTE]
>
>**FYI**
>
>Marketo sta ora standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che l&#39;iscrizione contenga lead/lead e la persona/persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

| Evento | Descrizione |
|---|---|
| Inviato | Viene registrato ogni volta che un&#39;e-mail viene inviata dai server Marketo, indipendentemente dal fatto che sia effettivamente consegnata. I messaggi e-mail con bacheca vengono ancora registrati come &quot;Inviati&quot;. |
| Consegnato | Viene registrato ogni volta che un&#39;e-mail viene accettata dal server di posta del destinatario. Ciò non significa che ha evitato i filtri anti-spam. Per ogni e-mail inviata è possibile ricevere solo 1 invio. |
| Bloccato duro | Alcuni rimbalzi duri sono il risultato di blocchi di spam, quindi non proveremo a mandare email a quella persona per 24 ore in nessuna campagna. Altri rimbalzi duri come inbox inesistenti sono permanenti e non invieremo mai più email alla persona da nessuna campagna. |
| Soft Bounce | Viene registrato quando una risposta del server non è chiara, la cassetta postale è piena o problemi generali del server. Abbiamo sottoposto queste persone a una logica di tentativi per 24-36 ore per una possibile consegna futura. Ciò non esclude la persona da altri invii. |
| Aperto | È registrato quando un destinatario visualizza un&#39;e-mail con immagini NON bloccate. Viene registrato un solo evento aperto per e-mail, per persona, per campagna intelligente. Se aprono la stessa e-mail dalla propria inbox due volte, non verrà registrata più di una volta. |
| Clic | Viene registrato ogni volta che un URL decorato dall’e-mail viene caricato nel browser (il risultato di fare clic sul collegamento). In genere si tratta del clic del destinatario, ma può anche essere un taglio/incolla. |
| Annulla sottoscrizione | Viene registrato quando una persona fa clic sul collegamento di annullamento della sottoscrizione di un&#39;e-mail e invia il modulo di annullamento della sottoscrizione. |

>[!CAUTION]
>
>Se la stessa e-mail viene inviata due volte alla stessa persona dalla stessa campagna, l&#39;evento **Open** verrà registrato al massimo 1 volta.

