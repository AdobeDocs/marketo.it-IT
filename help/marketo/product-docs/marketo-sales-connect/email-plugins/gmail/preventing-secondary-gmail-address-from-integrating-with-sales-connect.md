---
unique-page-id: 14352546
description: Impedire l'integrazione dell'indirizzo Gmail secondario con Sales Connect - Documenti Marketo - Documentazione del prodotto
title: Impedire l'integrazione dell'indirizzo Gmail secondario con Sales Connect
exl-id: a84fe53b-0ec8-400c-8747-be496c68a8e3
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Impedire l&#39;integrazione dell&#39;indirizzo Gmail secondario con Sales Connect {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Integrazione Gmail interrotta (perché il mio Gmail personale invia e-mail) {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

Il motivo più comune per una connessione Gmail interrotta è un’integrazione accidentale con l’account personale di un utente. Ciò può verificarsi quando un utente fa clic su &quot;Connetti&quot; o quando tenta di inviare un’e-mail dal proprio account personale. Potrebbe essere molto invitante, perché l’opzione è disponibile quando accedi al tuo account Gmail nella stessa istanza di Chrome dell’e-mail aziendale.

## Perché Sales Connect cerca persino di integrarsi con il mio Gmail personale? {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

Sales Connect si integra con Gmail tramite un&#39;estensione installata nel browser Chrome. Ogni volta che l’estensione rileva un’istanza di Gmail aperta, offre un’opzione per integrarla. Per evitare un’integrazione con il tuo account Gmail personale, ti consigliamo una delle tre cose seguenti:

Accedi Come Altro Utente Chrome (Consigliato)

Fai clic su [questo collegamento](https://support.google.com/chrome/answer/2364824?hl=en) per scoprire come creare un altro profilo Chrome.

**Pro**: l&#39;accesso come altro utente aprirà una nuova istanza di Chrome. Questa istanza è una nuova finestra di Chrome e nessuna delle vecchie estensioni esisterà in questa. Inoltre, conserva i cookie in modo da non dover accedere al tuo Gmail ogni volta.

**Contro**: devono essere aperte due finestre di Chrome.

Usa un altro browser

**Pro:** l&#39;utilizzo di un altro browser Internet (IE o Firefox) in cui non è installata l&#39;estensione impedirà che ciò accada.

**Contro**: l&#39;utilizzo di più browser può essere fastidioso.

Utilizzare Una Finestra In Incognito

**Pro:** una finestra in incognito è simile all&#39;apertura di una versione nuda di Chrome. Ciò significa che non avrà installato nessuna delle tue estensioni e Sales Connect non sarà disponibile per la connessione.

**Contro**: dovrai accedere a Gmail ogni volta che inizi la tua giornata e di nuovo se chiudi accidentalmente la finestra.
