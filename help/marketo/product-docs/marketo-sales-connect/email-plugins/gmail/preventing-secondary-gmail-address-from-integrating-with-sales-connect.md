---
unique-page-id: 14352546
description: Impedire l'integrazione dell'indirizzo Gmail secondario con Sales Connect - Marketo Docs - Documentazione del prodotto
title: Impedire l'integrazione dell'indirizzo Gmail secondario con Sales Connect
exl-id: a84fe53b-0ec8-400c-8747-be496c68a8e3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Impedire l&#39;integrazione dell&#39;indirizzo Gmail secondario con Sales Connect {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Integrazione di Gmail non riuscita (perché la mia e-mail personale di invio di Gmail) {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

Il motivo più comune per una connessione Gmail non funzionante è un&#39;integrazione accidentale con l&#39;account personale di un utente. Questo può accadere quando un utente fa clic su &quot;Connetti&quot; o quando cerca di inviare un&#39;e-mail dal proprio account personale. Questo può essere molto invitante da fare perché l&#39;opzione esiste quando si accede al tuo account Gmail nella stessa istanza di Chrome del tuo lavoro e-mail.

## Perché Sales Connect cerca addirittura di integrarsi con il mio Gmail personale? {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

Sales Connect si integra con Gmail tramite un&#39;estensione installata nel browser Chrome. Ogni volta che l’estensione rileva un’istanza di Gmail aperta, offre un’opzione per integrarla. Per evitare un&#39;integrazione con il tuo account Gmail personale, ti consigliamo una delle tre cose...

Accedi Come Un Altro Utente Chrome (Consigliato)

Fai clic su [questo link](https://support.google.com/chrome/answer/2364824?hl=en) per scoprire come creare un altro profilo Chrome.

**Pro**: L’accesso come un altro utente aprirà una nuova istanza di Chrome. Questa istanza è una nuova finestra di Chrome e nessuna delle tue vecchie estensioni esisterà in questa. Inoltre, mantiene i cookie in modo da non dover sempre accedere al tuo Gmail.

**Contro**: Devono essere aperte due finestre di Chrome.

Usa un altro browser

**Pro:** L&#39;utilizzo di un altro browser Internet (IE o Firefox) che non dispone dell&#39;estensione installata impedirà che ciò si verifichi.

**Contro**: L&#39;utilizzo di più browser può essere fastidioso.

Utilizzare Una Finestra In Incognito

**Pro:** Una finestra in incognito è come aprire una versione nuda di Chrome. Ciò significa che non avrà nessuna delle estensioni installate e che Sales Connect non sarà presente per la connessione.

**Contro**: Dovrai accedere a Gmail ogni volta che inizi la tua giornata, e di nuovo se chiudi accidentalmente la finestra.
