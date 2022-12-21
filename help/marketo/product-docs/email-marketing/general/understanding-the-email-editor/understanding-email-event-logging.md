---
unique-page-id: 1147356
description: Informazioni sulla registrazione degli eventi e-mail - Documenti Marketo - Documentazione del prodotto
title: Informazioni sulla registrazione degli eventi e-mail
exl-id: 107d7f4a-ad38-44e4-95d8-760539aacede
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 1%

---

# Informazioni sulla registrazione degli eventi e-mail {#understanding-email-event-logging}

Quando invii e-mail, Marketo registra diversi punti dati nei registri attività della persona. Ecco quelli di base.

| Evento | Descrizione |
|---|---|
| Inviato | Viene registrato ogni volta che un’e-mail viene inviata dai server Marketo, indipendentemente dal fatto che sia effettivamente consegnata. Le e-mail rimbalzate vengono comunque registrate come &quot;Inviate&quot;. |
| Consegnato | Viene registrato ogni volta che un’e-mail viene accettata dal server di posta del destinatario. Questo non significa che ha evitato i filtri anti-spam. Per ogni e-mail inviata può essere presente solo una consegna. |
| duro rimbalzato | Alcuni rimbalzi duri sono il risultato di blocchi di spam, quindi non cercheremo di inviare a quella persona per 24 ore in alcuna campagna. Altri rimbalzi duri come caselle in entrata inesistenti sono permanenti e non invieremo mai più un’e-mail alla persona da alcuna campagna. |
| Soft rimbalzato | Viene registrato quando una risposta del server non è chiara, la cassetta postale è piena o problemi generali del server. Abbiamo sottoposto queste persone a una logica di esecuzione di nuovi tentativi per 24-36 ore per una consegna potenziale futura. Questo non squalifica la persona da altri invii. |
| Aperto | Viene registrato quando un destinatario visualizza un&#39;e-mail con immagini NON bloccate. Viene registrato un solo evento aperto per e-mail, per persona, per campagna intelligente. Se aprono la stessa e-mail dalla casella in entrata due volte, non verrà registrata più di una volta. |
| Clic | Viene registrato ogni volta che un URL decorato dall’e-mail viene caricato nel browser (il risultato di fare clic sul collegamento). Di solito questo è il destinatario che fa clic, ma può anche essere un taglio/incolla. |
| Annulla l&#39;iscrizione | Viene registrato quando una persona fa clic sul collegamento di annullamento dell’abbonamento di un’e-mail e invia il modulo di annullamento dell’abbonamento. |

>[!CAUTION]
>
>Se la stessa e-mail viene inviata alla stessa persona due volte dalla stessa campagna, la **Aperto** l’evento verrà registrato al massimo 1 volta.
